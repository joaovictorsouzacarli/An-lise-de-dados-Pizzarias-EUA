## Análise de dados de Pizzarias dos EUA :pizza:
 
Você já se perguntou como é o mercado de pizzas nos Estados Unidos? Quais são as preferências dos consumidores, os horários de maior demanda, os tipos e tamanhos mais vendidos, o valor médio gasto por pedido e por categoria? Essas são algumas das questões que podemos responder com uma boa análise de dados, usando ferramentas como o Power BI e técnicas de ETL.
Neste artigo, vou apresentar um estudo de caso sobre um ano de vendas de uma pizzaria fictícia, baseado na base de dados da @Maven Analytics. A base de dados contém informações sobre cada pedido realizado pela pizzaria, incluindo data e hora, número do cliente, número do pedido, pizzas servidas, com detalhes sobre tipo, tamanho, quantidade, preço e ingredientes.

Para realizar a análise, vamos seguir os seguintes passos:
- ETL: sigla em inglês para Extract, Transform and Load, que significa extrair, transformar e carregar os dados. Esse é o processo de coletar os dados de diferentes fontes, limpar e padronizar os dados, aplicar regras de negócio e carregar os dados em um destino final para serem usados na análise.
"O ETL é a parte mais complexa, cara e demorada de um projeto de data warehouse. É também a parte mais crítica para o sucesso do projeto, pois determina a qualidade, a consistência e a disponibilidade dos dados para a tomada de decisão." (Kimball e Caserta, 2004, p. 3)

- Dashboard: é uma ferramenta visual que permite apresentar os resultados da análise de forma interativa e dinâmica, usando gráficos, tabelas, filtros e indicadores. Neste caso, foi usado o Power BI, uma plataforma da Microsoft que permite criar dashboards profissionais e compartilhá-los na web ou em dispositivos móveis.
"O dashboard é uma ferramenta de gestão que permite visualizar, de forma rápida e eficiente, os principais indicadores de desempenho de uma organização. Ele funciona como um painel de controle, que reúne as informações mais relevantes para a tomada de decisão e o monitoramento dos resultados." - Alberto Cairo, em O Design Funcional do Gráfico.
Vamos começar?

O primeiro passo foi extrair os dados da base de dados, que está disponível em um arquivo Excel. Para isso, utilizou o Power Query, uma ferramenta integrada ao Power BI que permite conectar-se a diferentes fontes de dados e aplicar transformações nos dados.

Base de Dados
Ao abrir o arquivo Excel no Power Query, podemos ver que ele contém três planilhas: Orders (Pedidos), Customers (Clientes) e Menu (Cardápio). Cada planilha tem um conjunto de colunas com informações relevantes para a análise. 
Antes de carregar os dados no Power BI, foi necessário fazer algumas transformações para garantir a qualidade e a consistência dos dados. Algumas das transformações que foram aplicadas:
- Remover as linhas vazias ou duplicadas
- Alterar o tipo de dado das colunas para o formato adequado (data, hora, número, texto)
- Padronizar os nomes das colunas e dos valores
- Separar os ingredientes em colunas individuais
- Criar colunas calculadas com informações adicionais, como o dia da semana, o mês, o ano e a categoria da pizza
Após aplicar as transformações necessárias em cada planilha, podemos carregar os dados no Power BI.

Dashboard
O segundo passo foi criar o dashboard no Power BI. Para isso, foi utilizado o Power BI Desktop, uma aplicação gratuita que permite criar relatórios e dashboards com recursos avançados de visualização e interação.
O objetivo do nosso dashboard é responder às questões que levantamos no início do artigo: Quais são as preferências dos consumidores, quantidade de pedidos, quantidade de vendas, ticket médio, os tipos e tamanhos mais vendidos, o valor médio gasto por pedido e por categoria?
O resultado é o seguinte dashboard:
![image](https://github.com/joaovictorsouzacarli/An-lise-de-dados-Pizzarias-EUA/assets/129809075/f22516f9-5e5c-4570-9496-f21c488d0f6e)

Com esse dashboard, podemos explorar os dados e obter insights sobre o comportamento dos clientes e o desempenho da pizzaria. Por exemplo, podemos ver que:
- A categoria mais vendida é a de pizzas classicas, seguida pelas pizzas especiais; 
- Os meses de maior venda são Julho, Março e Maio;
- O tipo de pizza mais vendido é a Hawaian, seguida pela Pepperoni;
- O tamanho de pizza mais vendido é o pequeno;
Conclusão
Neste artigo, foi mostrado como realizar uma análise de dados de uma pizzaria fictícia usando a base de dados da @Maven Analytics e o Power BI. Vimos como fazer o processo de ETL para extrair, transformar e carregar os dados, e como criar um dashboard para apresentar os resultados da análise. Com esse dashboard, podemos responder às questões que nos propusemos no início do artigo e obter insights sobre o mercado de pizzas nos Estados Unidos.

Obrigado pela leitura!

