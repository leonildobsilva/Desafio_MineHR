--Readme--
 
O Objetivo desse projeto é efetuar o tratamento dos dados da base_mensalizada_de_funcionarios.csv e aplicar as regras de negócio determinadas.

Foi utilizado o Databricks Community com a linguagem Pyspark para o desenvolvimento do script main.ipynb.

Os dados refinados foram exportados no arquivo export.csv encontrado nesse repositório.


Algumas particularidades: 

- Conforme a solicitação foi necessário primeiro remover os valores nulos das colunas, substuindo por dados fixos. Depois as mesmas foram formatadas com as tipagens correspondentes. Na coluna “salario” havia uma linha do tipo string que foi anulada ao ser formatada para o tipo float. Seguindo o requisito de não haver dados nulos nesta coluna, houve uma nova substuição de nulo para “0”.


- Para o desenvolvimento das regras de negócio foram criados dois scripts com as seguintes finalidades:

[TESTE EM SQL] - teste realizado em SQL para assegurar a funcionalidade dos comandos.
[APLICAÇÃO DE REGRA] - aplicação prática da regra realizando a inclusão no dataframe.

*Para rodar o script é recomendado utilizar o Databricks Community disponivel no link abaixo: 
https://community.cloud.databricks.com/login.html