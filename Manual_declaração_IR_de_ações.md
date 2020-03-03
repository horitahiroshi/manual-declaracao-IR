# Manual de declaração de IR para ações.
CEI -> Extratos e Informativos -> Negociações de Ativos
	De 01/01/2019 à 31/12/2019.

Abrir Programa Gerador da Declaração (PGD).

## Declaração de ativos comprados ao longo do ano.

```
> Bens e Direitos
	> Novo
		> Código: 31 - Ações (inclusive as provenientes de linha telefônica).
		> Localização: 105 - Brasil
		> CNPJ: ###cnpj-da-empresa-do-ativo###
		> Discriminação: quantidade de ações da empresa que vc possuia no dia 31/12/2019 e o custo total.
			> Ex.: 100 AÇÕES DE FLEURY S/A, CÓDIGO DE NEGOCIAÇÃO FLRY3, CUSTO TOTAL DE R$2.193,00.
		> Situação em 31/12/2018 (R$): 0,00
		> Situação em 31/12/2019 (R$): 2193,00
```
Obs.: utilizar a soma dos valores no ato da COMPRA dos ativos!

## Declaração de ativos comprados e vendidos no decorrer do ano.

Ex.: em 2019 comprou-se 400 ações (a preço médio de R$ 24,933) de SQIA3 e vendeu-se 200 (a preço médio de R$25,200), em momentos diferentes.
```
> Bens e Direitos
	> Novo
		> Código: 31 - Ações (inclusive as provenientes de linha telefônica).
		> Localização: 105 - Brasil
		> CNPJ: cnpj_da_empresa_do_ativo
		> Discriminação: 200 AÇÕES DE SINQIA, CÓDIGO DE NEGOCIAÇÃO SQIA3, CUSTO TOTAL DE R$4.986,00.
		> Situação em 31/12/2018 (R$): 0,00
		> Situação em 31/12/2019 (R$): 4986,00
```
Obs.: Custo total passa a ser (Quantidade_comprados - Quantidade_vendidos) * Preço_médio_de_compra. Neste caso, (400 - 200) * 24,933.

Quanto ao lucro das 200 ações vendidas (200 * R$25,200 - 200 * R$24,933) = R$54,00, TAMBÉM DEVE SER DECLARADO, porém este é livre de imposto UMA VEZ QUE O LUCRO OBTIDO FOI MENOS QUE R$20.000,00.
```
> Rendimentos Isentos e Não Tributáveis
	> Novo
		> Tipo de Rendimento: 20 - Ganhos líquidos em operações no mercado à vista de ações negociadas em bolsas de valores nas alienações realizadas até R$20.000,00.
		> Tipo de Beneficiário: Titular
		> Beneficiário: beneficiário
		> Valor: valor_do_lucro_obtido
			> Ex.: 54,00
```

## Declaração de prejuízo em negociações da bolsa.

```
> Renda Variável
	> Operações Comuns / Day-Trade
		> aqui devemos preencher a soma do(s) prejuízo(s) de CADA MÊS.
		> Ex.: se ao invés de lucro, tivesse tomado prejuízo de R$ 54,00 em ABRIRL:	
			> ABR
				> Mercado à Vista
					> Mercado à vista - ações
						> Operações Comuns: -54
```
Obs.: Só vai declarar lucro nesta aba (Renda Variável) se o valor obtido tiver ultrapassado R$ 20.000,00 EM UM MÊS.

## Declaração de lucro acima de R$ 20.000,00.

```
> Renda Variável
	> Operações Comuns / Day-Trade
		> aqui devemos preencher a soma do(s) prejuízo(s) de CADA MÊS.
		> Ex.: se tivesse lucrado R$ 20.001,00 em ABRIRL em Swing-Trade (operação comum):	
			> ABR
				> Mercado à Vista
					> Mercado à vista - ações
						> Operações Comuns: 20001
```
Obs.: em >Resultados (na mesma página de Renda Variável), o próprio programa analisa todos os lucros (acima de 20k) e todos os prejuízos e calcula o quando deve ser pago de imposto.
Obs.2: Se o imposto sobre o lucro já foi pago por DARF, no mês do lucro, em >Consolidação do Mês (na mesma página), confira o valor em >Imposto a pagar; e informe o imposto pago pelo DARF em >Imposto pago. Assim não paga imposto 2 vezes.

## Declaração de proventos

### Dividendos

Ex.: WEG S.A. pagou R$ 8,23 em dividendos.
```
> Rendimentos Isentos e Não Tributáveis
	> Novo
		> Tipo de Rendimento: 09 - Lucros e dividendos recebidos
			> Tipo de Beneficiário: Titular
			> CNPJ da Fonte Pagadora: cnpj_da_empresa_pagadora
			> Nome da Fonte Pagadora: WEG S.A.
			> Valor: 8,23
```

### Juros sobre capital

Ex.: WEG S.A. pagou R$ 17,83 em juros sobre capital próprio.
```
> Rendimentos Sujeitos à Tributação Exclusiva/Definitiva
	> Novo
		> Tipo de Rendimento: 10 - Juros sobre capital próprio
			> Tipo de Beneficiário: Titular
			> CNPJ da Fonte Pagadora: cnpj_da_empresa_pagadora
			> Nome da Fonte Pagadora: WEG S.A.
			> Valor: 17,83
```

### Créditos em trânsito

Créditos em trânsito são proventos declarados pelas empresas, mas que ainda não foram repassados aos acionistas. Possuindo esse direito, devemos declarar em >Bens e Direitos.
Ex.: WEG S.A. tem créditos em trânsito de juros sobre capital próprio de R$ 14,59.
```
> Bens e Direitos
	> Novo
		> Código: 99 - Outros bens e direitos
		> Localização: 105 - Brasil
		> Discriminação: CRÉDITOS EM TRÂNSITO - JUROS SOBRE CAPITAL PRÓPRIO: nome_da_empresa_pagadora - CNPJ: cnpj_da_empresa_pagadora
		> Situação em 31/12/2019: 14,59
```

## Referência
Vídeo no canal Jovens de Negócios, disponível em: 
https://www.youtube.com/watch?v=HCaO95bpE-0