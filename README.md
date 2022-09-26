# O-Papel-do-Banco-de-Dados-SQL-e-NoSQL-na-Engenharia-de-Dados
Conceitos, definições e insigths para compreender o Papel do Banco de Dados SQL e NoSQL na Engenharia de Dados
*Banco de Dados Relacional
Armazena e fornece acesso a informações com relações entre si, 
com consistência e sem duplicidade num sistema rígido. 
 - Tipos de Banco de Dados Relacional: MySQL,MariaDB,Oracle, Amazon Aurora
Microsoft SQL Server, PostgreSQL.
 - Empresas que usam este tipo de banco de Dados: Banco Bradesco,Lufthansa
Nokia,NASA...etc.
Um exemplo de banco de dados relacional
Este é um exemplo simples de duas tabelas que uma pequena empresa pode usar
para processar pedidos de seus produtos. A primeira tabela é de informações
do cliente, de forma que cada registro inclui o nome, o endereço, as 
informações de envio e faturamento, o número de telefone e outras 
informações de contato de um cliente. Cada bit de informação 
(cada atributo) está em sua própria coluna, e o banco de dados atribui uma
ID única (uma chave) a cada linha. Na segunda tabela -uma tabela de pedidos
do cliente - cada registro inclui o ID do cliente que fez o pedido, o 
produto solicitado, a quantidade, o tamanho e a cor selecionados e assim 
por diante - mas não o nome ou as informações de contato.
Essas duas tabelas têm apenas uma coisa em comum: a coluna ID (a chave). 
Mas por causa dessa coluna comum, o banco de dados relacional pode criar 
uma relação entre as duas tabelas. Assim, quando o aplicativo de 
processamento de pedidos da empresa envia um pedido ao banco de dados, 
o banco de dados pode ir à tabela de pedidos do cliente, obter as 
informações corretas sobre o pedido do produto e usar o ID do cliente 
dessa tabela para procurar as informações de faturamento e envio do 
cliente na tabela de informações do cliente. O warehouse poderá obter o 
produto correto, o cliente receberá a entrega do pedido oportunamente e 
a empresa receberá o pagamento.
https://www.oracle.com/br/database/what-is-a-relational-database/
*Banco de Dados Não Relacional
Armazena grandes volumes dados de forma não estruturada,não sendo 
necessáriamente ser conhecidas e não precisa ter relação entre si.
são amplamente usados em aplicativos da web em tempo real e big data, 
porque suas principais vantagens são alta escalabilidade e alta 
disponibilidade.
 - Tipos de Banco de Dados Relacional:MongoDB,Neo4j,Cassandra, Amazon DynamoDB
Memcached, Hbase.
 - Empresas que usam este tipo de banco de Dados: MTV, Facebook,Google,The New York Times..etc
https://learn.microsoft.com/pt-br/azure/architecture/data-guide/big-data/non-relational-data

Ambos são extramente importantes na Engenharia de dados, pois dependendo 
da necessidade da empresa acabam utilizando os dois tipos, nesse caso um
um complementa o outro. É preciso analisar o cenário em que a empresa está
inserida, o volume de dados que possui, a agilidade em acessar os dados
e o orçamento, com essas informações levantadas o responsável pela 
Engenharia Dados poderá definir qual tipo de Banco de Dados será mais
adequado e alcansará melhores resultdos.
