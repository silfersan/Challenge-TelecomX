# Challenge-TelecomX
Este projeto tem como finalidade investigar o fenômeno de evasão de clientes (churn) em uma empresa
de telecomunicações. Por meio da análise explorátoria dos dados, buscamos compreender o perfil dos
clientes que cancelam os serviços e identificar padrões que auxiliem na redução da taxa de 
cancelamento.
A retenção de clientes é um aspecto estratégico em qualquer negócio, e compreender os fatores que
influenciam o churn possibilita a adoção de medidas preventivas.
As principais etapas realizadas foram:
Importação dos dados em formato JSON com estrutura aninhada.
Normalização das tabelas internas (cliente, plano, internet, cobrança).
Padronização dos nomes das colunas para o padrão snake_case.
Conversão de campos como charges.total de texto para valores númericos (float), com tratamento de
valores nulos.
Criação da coluna contas_diárias, obtida pela divisão de charges.monthly por 30.
Padronização da variável churn: Yes - Cancelou, No - Permaneceu.
A maioria dos clientes manteve o serviço, enquanto aproximadamente 26,6% cancelaram. Para representar 
essa proporção, foi criado um gráfico de pizza com rótulos percentuais e valores absolutos.
Foram analisados os cancelamentos em relação a diferentes variáveis, como:
Tipo de Contrato (contract): maior evasão em contratos mensais.
Forma de pagamento (paymentmethod): métodos automáticos apresentam menor taxa de cancelamento.
Outras variáveis: gender, partner, internetservice, multiplelines.
Gráficos de barras foram utilizados para exibir os percentuais de cada categoria.
Foram aplicados boxplots para comparar a distribuição de:
Tempo de contrato (tenure): clientes recentes apresentam maior chance de cancelamento.
Gasto mensal (charges.monthly): clientes com mensalidades mais altas tendem a permanecer.
Gasto total (charges.total): clientes com maior histórico de gastos apresentam menor evasão.
Também foram calculadas média, mediana e desvio padrão dessas variáveis, segmentadas por grupo de 
churn.
Conclusões
Contratos mensais estão associados a maior evasão.
Pouco tempo de vínculo é um forte indicativo de cancelamento. 
Menores gastos mensais ou totais correlacionam-se com maior churn.
Clientes que utilizam métodos automáticos de pagamento permanecem mais.
Recomendações
Oferecer benefícios e descontos para incentivar planos anuais.
Implementar ações de retenção nos primeiros meses de contrato.
Estimular o uso de formas de pagamento automáticas.
Criar campanhas direcionadas a clientes de baixo gasto total.
Monitorar clientes com pouco tempo de vínculo para ações preventivas.
A análise possibilitou identificar os perfis mais propensos a evasão e propor estratégias concretas 
para reduzir a perda de clientes.
O uso de dados como base para a tomada de decisão torna as ações mais assertivas e eficazes.
