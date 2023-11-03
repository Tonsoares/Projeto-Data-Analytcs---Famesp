# Projeto-Data-Analytcs---Famesp

## Prevendo a Inadimplência de Clientes 

O uso de cartão de crédito é bastante comum nos dias de hoje e um uso correto dele
realmente ajuda na construção de uma boa pontuação de crédito. Quão importante é a
pontuação de crédito? Sempre que você precisa realizar uma compra a prazo, sua pontuação
de crédito é consultada e pode ser o fator decisivo na aprovação da sua compra.
No entanto, a inadimplência pode fazer com que a pontuação de crédito caia. Não apenas a pontuação de
crédito cai, como também haverá um efeito adverso sobre o limite de crédito e empréstimos
futuros de qualquer tipo.

Neste projeto, estaremos lidando com um histórico de pagamentos de clientes em
Taiwan. O conjunto de dados tem 24 atributos e um rótulo de classe e existem 30000
instâncias. Criaremos um modelo preditivo para permitir que o banco possa prever se o seu
cliente será inadimplente no próximo pagamento ou não.

## Objetivo: construir um classificador e usá-lo para prever se o cliente do cartão de
crédito será inadimplente no próximo pagamento.

Conjunto de dados: Dados bancários do repositório de Machine Learning da UCI:
## https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients

Antes de iniciar nossa análise, precisamos nos familiarizar com o conjunto de dados. O
conjunto de dados está desequilibrado, ou seja, a maioria dos rótulos de classe são não-
inadimplentes. Das 30000 instâncias, 78% são não-inadimplentes e 22% restantes são
inadimplentes.

A seguir estão os atributos presentes no conjunto de dados: ID, equilíbrio de crédito,
gênero, educação, estado civil e idade são auto-explicativos. Pay_0, Pay_2, Pay_3, Pay_4,
Pay_5, Pay_6 são o estado do pagamento nos meses de abril a setembro, respectivamente. O
status do pagamento é definido como o atraso no pagamento. Exemplo: se o valor de Pay_0 for
-1, então significa que o cliente foi devidamente pago, se o valor for 2, isso significa que o
pagamento está atrasado por dois meses. Bill_Amt1 a Bill_Amt6 são os montantes das faturas
do cartão de crédito para o mês de abril até setembro. Pay_Amt1 a Pay_Amt6 são o valor que o
cliente pagou na conta do cartão de crédito no mês de abril até setembro.
Abaixo, a tabela com uma descrição de cada um dos atributos

## Atributo Descrição
ID ID único de cada registro

Credit Balance Quantidade de crédito no cartão de crédito

Gender Sexo do cliente (masculino/feminino)

Education Nível de Escolaridade, i.e. Pos-graduado,

Graduado, Ensino Médio, Outros

Marital Status Estado Civil, i.e. casado, solteiro, outros

Age Idade do cliente

Pay_0 Status de Pagamento em Setembro

Pay_2 Status de Pagamento em Agosto

Pay_3 Status de Pagamento em Julho

Pay_4 Status de Pagamento em Junho

Pay_5 Status de Pagamento em Maio

Pay_6 Status de Pagamento em Abril

Bill_Amt1 Valor da Conta do cartão em Setembro

Bill_Amt2 Valor da Conta do cartão em Agosto

Bill_Amt3 Valor da Conta do cartão em Julho

Bill_Amt4 Valor da Conta do cartão em Junho

Bill_Amt5 Valor da Conta do cartão em Maio

Bill_Amt6 Valor da Conta do cartão em Abril

Pay_Amt1 Valor pago em Setembro

Pay_Amt2 Valor pago em Agosto

Pay_Amt3 Valor pago em Julho

Pay_Amt4 Valor pago em Junho

Pay_Amt5 Valor pago em Maio

Pay_Amt6 Valor pago em Abril

Default_payment_next_month Valor 0 ou 1 - 0 significa não-inadimplência e 1
significa inadimplência

## Link do Dashboard no Power BI: clique aqui
