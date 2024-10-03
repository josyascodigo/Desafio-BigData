# Desafio-BigData
Desafio  Processamento de dados em Grande Volumes

Documentação do Código
Análise de Vendas com Pandas
Descrição
Este código realiza a análise de dados de vendas a partir de um arquivo CSV. Através do uso da biblioteca pandas, o código lê os dados em blocos para evitar problemas de memória e filtra as colunas relevantes. Em seguida, ele realiza as seguintes análises:

Produto Mais Vendido: Identifica qual produto foi o mais vendido em termos de quantidade e canal de vendas.
Vendas por País e Região: Determina qual país e região tiveram o maior volume de vendas, considerando o total de receita.
Média de Vendas Mensais: Calcula a média de vendas mensais por produto, permitindo uma visão mais granular das tendências de vendas ao longo do tempo.
Os resultados são organizados em um arquivo Excel, onde cada análise é salva em uma aba separada.

Razões para Escolha
Escolhi usar pandas devido à sua facilidade de uso e robustez para manipulação de dados. A leitura em blocos é uma estratégia eficaz para trabalhar com grandes conjuntos de dados sem sobrecarregar a memória. A capacidade de agrupar e resumir dados em pandas também é uma vantagem significativa, tornando o código mais legível e eficiente para as análises desejadas.

Análise de Vendas com PySpark
Descrição
Este código utiliza a biblioteca PySpark para realizar uma análise distribuída de dados de vendas, permitindo que a aplicação lide com grandes volumes de dados de forma eficiente. As principais etapas da análise incluem:

Leitura do CSV: Carrega o arquivo CSV de forma distribuída, inferindo automaticamente os tipos de dados.
Particionamento: Reparticiona os dados pelo campo "Country" para otimizar o processamento em um ambiente distribuído.
Conversão de Tipo de Data: Transforma a coluna de data para um formato que pode ser manipulado nas análises.
Análises:
Identificação do produto mais vendido em termos de quantidade e canal.
Determinação do país e região com o maior volume de vendas.
Cálculo da média de vendas mensais por produto.
Os resultados são salvos em um arquivo Excel, com múltiplas abas para cada análise.

Razões para Escolha
Escolhi usar PySpark para esta análise devido à sua capacidade de processar dados de maneira distribuída, o que é essencial quando lidamos com grandes volumes de dados que podem exceder a memória de uma única máquina. O uso de PySpark permite não apenas uma análise mais rápida, mas também a escalabilidade, o que é vital para ambientes de Big Data. A integração com pandas para a geração do arquivo Excel facilita a apresentação dos resultados de forma organizada.
