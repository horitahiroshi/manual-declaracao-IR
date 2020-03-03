# Manual de declaração de IR para Fundos de Investimento Imobiliário
CEI -> Extratos e Informativos -> Negociações de Ativos
	De 01/01/2019 à 31/12/2019.

Abrir Programa Gerador da Declaração (PGD).

## Declaração de todas as posições em FIIs

Ex.: compra de 7 ativos de AEFI11 a preço médio de R$ 144,17 (= R$ 1.009,19).
```
> Bens e Direitos
	> Novo
		> Código: 73 - Fundo de Investimento Imobiliário
		> Localização: 105 - Brasil
		> CNPJ: cnpj_da_empresa_pagadora (dispinível no CEI-B3)
		> Discriminação: 7 cotas de AESAPAR FND INV IMOB. Código de Negociação AEFI11. Custo total de R$ 1.019,51.
		> Situação em 31/12/2019: 1019,51
```
Obs.: valor da compra dos ativos (+ taxas de corretagem + emolumentos etc)!

## Declaração de proventos de FIIs

Todos rendimentos de FIIs são isentos de IR.

Ex.: RIO BRAVO INVEST DTVM LTDA pagou R$ 34,16 em proventos.
```
> Rendimentos Isentos e Não Tributáveis
	> Novo
		> 26 - Outros
			> CNPJ da Fotne Pagadora: cnpj_da_fonte_pagadora (pode ser do Fundo em si ou da Administradora. Conferir no informe recebido via correio.)
			> Nome da Fonte Pagadora: RIO BRAVO INVEST DTVM LTDA
			> Descrição: Rendimentso provenientes do AESAPAR FND INV IMOB - FII
			> Valor: 34,16
```

## Em caso de venda de cotas de FIIs.

Lembrando que para venda de FII, devemos preencher o DARF e pagar 20% sobre o lucro (em caso de lucro).
```
> Renda Variável
	> Operações Fundos Invest. Imob.
		> Resultado líquido do mês: inserir valor do lucro ou prejuízo que obteve na(s) venda(s) do mês.
		> Resultado negativo até o mês anterior: em JAN deve preencher o prejuízo tido em DEZ do ano anterior.
		> Imposto retido no mês: imposto automaticametne retido no ato da venda (conhecido como "dedo-duro", para acusar à Receita Federal que fizemos a venda), discriminado na nota de corretagem como IRRF.
		> Imposto pago: informar impost já pago através do DARF. 
```

## Referência
Vídeo no canal Jovens de Negócios, disponível em: 
https://www.youtube.com/watch?v=-HrJtGU-i3M
