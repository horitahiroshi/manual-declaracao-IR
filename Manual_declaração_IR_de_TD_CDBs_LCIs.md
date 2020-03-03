# Manual de declaração de IR para investimentos em Renda Fixa
CEI -> Extratos e Informativos -> Negociações de Ativos
	De 01/01/2019 à 31/12/2019.

Abrir Programa Gerador da Declaração (PGD).

## Declaração de aplicações de Tesouro Direto

```
> Bens e Direitos
	> Novo
		> Código: 45 - Aplicação de renda fixa (CDB, RDB e outros)
		> Localização: 105 - Brasil
		> CNPJ: cnpj_da_instituição_financeira_por_onde_investiu
		> Discriminação: de forma breve, descrever todos investimentos de renda fixa aplicados na instituição.
			> Ex.: Títulos do Tesouro Direto: LFT com vencimento em 01/03/2023 no valor de R$2.104,62; NTN-B com vencimento em 15/05/2035 no valor de R$1.002,73.
		> Siutação em 31/12/2018 (R$): somatória dos valores no ano anterior.
		> Situação em 31/12/2019 (R$): somatória dos valores.
```

## Declaração de aplicações de CDB

```
> Bens e Direitos
	> Novo
		> Código: 45 - Aplicação de renda fixa (CDB, RDB e outros)
		> Localização: 105 - Brasil
		> CNPJ: cnpj_da_instituição_financeira_por_onde_investiu
		> Discriminação: de forma breve, descrever todos investimentos de renda fixa aplicados na instituição.
			> Ex.: Aplicações em Renda Fixa Privada: CDB emitido pelo Banco Maxima no valor de R$1.000,0; CDB emitido pelo Banco Maxima no valor de R$1.023,00.
		> Siutação em 31/12/2018 (R$): somatória dos valores no ano anterior.
		> Situação em 31/12/2019 (R$): somatória dos valores.
```

## Declaração de aplicações de Fundo de Investimento

```
> Bens e Direitos
	> Novo
		> Código: 72 - Fundo de Longo Prazo e Fundo de Investimentos em Direitos Creditório...
		> Localização: 105 - Brasil
		> CNPJ: cnpj_da_instituição_financeira_por_onde_investiu
		> Discriminação: exatamento o nome do(s) fundo(s) e quanto foi investido em cada um.
			> Ex.: Fundo de Renda Fixa: BRASIL PLURAL HIGH YIELD FIRF CP no valor de R$2.461,36.
		> Siutação em 31/12/2018 (R$): somatória dos valores no ano anterior.
		> Situação em 31/12/2019 (R$): somatória dos valores.
```

## Declaração de dinheiro parado em Conta Corrente

```
> Bens e Direitos
	> Novo
		> Código: 61 - Depósito bancário em conta corrente no País.
		> Localização: 105 - Brasil
		> CNPJ: cnpj_da_instituição_financeira_por_onde_investiu
		> Discriminação: exatamento o nome do(s) fundo(s) e quanto foi investido em cada um.
			> Ex.: Saldo na Corretora Clear
		> Agência (sem DV): número_da_sua_agência
		> Conta: número_da_sua_conta	> DV: seu_dígito_de_verificação
		> Siutação em 31/12/2018 (R$): somatória dos valores no ano anterior.
		> Situação em 31/12/2019 (R$): somatória dos valores.
```

## Declaração dos rendimentos

### Rendimentos sujeitos a tributação exclusiva - Valores em Reais

Rendimento dos títulos do TD, CDBs, LCs e dos Fundos, que já têm o imposto descontado na fonte.
```
> Rendimentos Sujeitos à Tributação Exclusiva/Definitiva
	> Novo
		> Tipo de Rendimento: 06 - Rendimento de aplicações financeiras
		> CNPJ: cnpj_da_instituição_financeira_por_onde_investiu
		> Nome da Fonte Pagadora: nome_da_instituição_financeira_por_onde_investiu
		> Valor: valor_do_rendimento (conforme Informe de Rendimento da instituição)
```
Obs.: Em caso de investimentos que não informa rendimento (R$0,00) por não ter atingido a data de vencimento, não precisa declarar!

### Rendimentos isentos e não tributáveis

No informe da instituição por onde investiu, no caso de rendimentos isentos e não tributáveis, pode ser declarado a somatória de todos os valores de rendimento.
```
> Rendimentos Isentos e Não Tributáveis
	> CNPJ da Fonte Pagadora: cnpj_da_instituição_financeira_por_onde_investiu
	> Nome da Fonte Pagadora: nome_da_instituição_financeira_por_onde_investiu
	> Valor: valor_dos_rendimentos (conforme Informe de Rendimento da instituição)
```

## Referência
Vídeo no canal Jovens de Negócios, disponível em: 
https://www.youtube.com/watch?v=cnrcsmbn8gw
