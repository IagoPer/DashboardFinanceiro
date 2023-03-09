# DashboardFinanceiro:zap:

### Dashboard Financeiro em Power BI

O Dashboard abaixo refere-se a uma base financeira que contém transações de recebimentos e pagamentos. Nele contém informações do total de Receitas, Despesas, Impostos, Lucro, Margem de Lucro e total de Transações.

No primeiro momento foi necessário realizar algumas alterações no Power Query, sendo essas o tipo de cada coluna, limpeza de dados desnecessários, desmembramento da base para criação de tabelas de dimensão afim de diminuir a quantidade de dados/informações repetitivas e melhorar o desempenho do Dashboard. Automaticamente, com o desmembramento da base foi necessário realizar o gerenciamento das relações entre a tabela fato e suas dimensões:

<img width="425" alt="Relacionamentos" src="https://user-images.githubusercontent.com/98985401/224091650-8d473b8c-1c79-4891-8724-7193890521f5.png">

Em seguida, foram criadas as medidas para cálculo da quantidade de transações e suas particularidades, total de receita, total de despesa, imposto, lucro e margem de lucro:

<img width="126" alt="Medidas" src="https://user-images.githubusercontent.com/98985401/224092448-81e6e228-cfa5-4397-b625-a46bca8a50bb.png">

No layout, foi usado o Scroller para apresentar a margem de lucro das transações vindas de determinados estados do Brasil. Cartões para apresentar o total de Receita, Despesa, Imposto e Lucro. Image Grid para visualização do logo de cada banco de acordo com uma URL disponibilizada na base. Indicador para visualização do percentual de Margem de Lucro. Elighten Data Story para apresentar o número de transações e detalhar o tipo. E por fim, o Gráfico de Cascata para apresentar o Lucro Mensal:

<img width="425" alt="Dashboard" src="https://user-images.githubusercontent.com/98985401/224092990-16f5bfc4-8ec5-4651-9683-78a4e0a4d3e4.png">

Diante das informações apresentadas podemos gerar os seguintes Insights:
  
  :heavy_check_mark: As transações de São Paulo geraram a maior margem de lucro seguido do Rio de Janeiro;
  
  :heavy_check_mark: A margem de lucro é de 37,58% sobre o valor total das receitas;
  
  :heavy_check_mark: 44,04% das transações são realizadas via PIX e 31,49% realizadas via Cartão;
  
  :heavy_check_mark: No geral o lucro mensal foi positivo, exceto nos meses de abril, junho e agosto.

Esses Insights são de grande valia, pois por meio deles podemos nos aprofundar nas informações identificando pontos que precisam de atenção, como por exemplo:
  
  :heavy_check_mark: Motivo dos meses de abril, junho e agosto não terem gerado lucro; 
  
  :heavy_check_mark: Elaborar um estudo de caso e plano de meta para alavancar as transações realizadas pela melhor forma de pagamento, afim de diminuir as taxas bancárias.

