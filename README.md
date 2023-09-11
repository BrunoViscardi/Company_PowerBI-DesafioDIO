# Company_PowerBI-DesafioDIO

Após criar uma instância na Azure, o banco de dados foi criado com referência ao disponibilizado pelo Desafio no software MySQL. Dessa forma, os dados foram obtidos e incorporados no Power BI. 

No Power BI, os dados foram transformados com auxílio do Editor Power Query. Verificou-se os cabeçalhos, tipos de dados de cada coluna e a existência de nulos. Além disso, os dados complexos de “Adress” da tabela “Employee” foram separados (por delimitador “-“) em novas colunas: “Rua”, “Número”, “Cidade” e “Estado”. 
 
Ainda no Power Query, foi realizado a criação de novas tabelas. A primeira delas foi a mescla das tabelas “employee” e “departament” com a função “mesclar consultas como novas” selecionando o tipo de “junção externa esquerda” com base no “DNo” e eliminando as colunas desnecessárias.

Nessa mesma perspectiva, criou-se uma nova tabela contendo os colaboradores e seus respectivos gerentes. Para tal, foi realizado a mescla das tabelas “employee” e “employee” combinando o “super_ssn” com o “ssn”. O nome e sobrenome dos colaboradores foram incorporados a uma única coluna, assim as colunas “Fname”, “Mnit” e “Lname” foram selecionadas e com a opção “mesclar colunas” combinadas em uma nova coluna “Nome”.

A ultima tabela (consulta) criada foi a mescla dos nomes dos departamentos e a localização desses, obtendo uma combinação única departamento-local. Para tal foi mesclado as tabelas “departament” e “dept_locations” e em seguida realizando a junção das colunas penitentes com delimitador “-“.

Por fim, os dados de gerente e colaboradores foram agrupados pela função “agrupar por” a fim de saber quantos colaboradores existiam por gerentes. Um relatório com alguns dados foi criado.
	
	
