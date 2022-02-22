# Comandos Iniciais do SQL

## INSERT

INSERT: adicionando registros a uma tabela
O comando INSERT é usado para inserir dados em uma tabela do banco. Para realizar essa ação, podemos usar a seguinte sintaxe:

>INSERT into estudantes (id, nome, curso) values (23, 'Rafael', 'Desenvolvimento de Software');

Perceba que, na sintaxe usada, a palavra “estudantes” se refere ao nome da tabela e os termos “id”, “nome” e “curso” são os campos dessa tabela que vão receber novas informações.

## UPDATE

UPDATE: atualizando os registros já inseridos
O comando UPDATE é o responsável por fazer edições em registros que já constam no banco. Essa instrução é muito importante já que ela permite corrigir ou complementar os dados, garantindo que o banco tenha sempre informações atualizadas.

A sintaxe usada nesse comando é:

>UPDATE estudantes SET nome = 'Rafael Rodrigues Maia' WHERE id = 23;

Observe que, com a instrução acima, a tabela __“estudantes”__ sofreu uma atualização, na qual o registro com id = 23 recebeu no campo “nome’’ o valor **“Rafael Rodrigues Maia”**.

## DELETE

DELETE: excluindo registros de uma tabela
Por sua vez, o comando DELETE é utilizado para excluir informações da nossa base de dados. A sintaxe para realizar essa ação é bastante simples:

>DELETE FROM estudantes WHERE id = 23;

Entenda que, após rodar esse comando, todas as informações referentes ao registro que possui id = 23 serão deletadas da tabela “estudantes”. Já, para apagar todos os registros de uma tabela de uma vez, usamos a seguinte instrução:

>DELETE FROM estudantes;

É importante explicar que o comando acima apaga apenas as informações armazenadas na tabela, ou seja, a estrutura, os índices e atributos do objeto continuam intactos no banco.

## SELECT

SELECT: retomando registros na tabela
Finalmente, o SELECT é um dos comandos SQL mais importantes, pois com ele podemos elaborar diversas consultas aos registros da nossa base de dados. É possível, por exemplo, fazer uma pesquisa que retornará todos os campos de uma tabela dessa forma:

>SELECT * FROM estudantes;

Perceba que, nessa consulta, o caractere * é usado para indicar que os dados de todas as colunas da tabela “estudantes” devem ser retornados na pesquisa. Por isso, para fazer uma consulta mais específica, os campos desejados devem ser informados da seguinte maneira:

>SELECT nome, curso FROM estudantes;

Além disso, utilizando a cláusula WHERE, podemos fazer uma consulta ainda mais refinada. Veja:

>SELECT nome FROM estudantes WHERE curso = 'Desenvolvimento de Software';

Como você deve ter notado, com o comando acima serão retornados apenas os nomes de estudantes que frequentam o curso de Desenvolvimento de Software. Ademais, caso queira uma lista ordenada, é possível utilizar a cláusula ORDER BY para que os dados sejam exibidos em ordem ascendente. Observe:

>SELECT nome FROM estudantes ORDER BY nome;


