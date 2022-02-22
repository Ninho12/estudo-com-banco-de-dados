# Estudo de Banco de Dados

## Descrição
Um repositório para eu aprender o fundamental de banco de dados SQL e NOSQL. 

### SQL com Mysql

vou adicionar aqui os comandos basicos do SQL:

#### Criação de Banco:
> Create Database Paroquia;

#### Criação de Tabela
> Create Table Dizimistas(
>   id Integer not null primary key auto increment,
>   nome String not null,
>   sobrenome String not null,
>   sexo String not null,
>   email String not null,
>   senha String not null,
>   data_de_nascimento Date,
>   id_de_comunidade Integer not null,
>   id_de_paroquia Integer not null,
>   id_de_diocese Integer not null
> );

