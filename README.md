# SSH
#### para entrar no modo "linux" usa-se esse comando. 
#### ssh caua.vioto@10.111.9.113
#### Depois disso ele pedirá a sua senha. Apos corretamente colocado você entrará no terminal Linux.

# MariaDb / MySQL
#### para entrar no sistema de banco de dados usa-se os seguintes comandos:
#### mysql -u nome.usuario -p
#### depois coloque a senha e pronto, estará no MariaDB.

# Comandos Banco_de_Dados

#### use [DbName] ---> Entra dentro da Db, para seu manuseio.
#### show databases; ---> Mostra todas as suas Db criadas.
#### show tables; ---> Mostra as tabelas dentro do Database.
#### create database [DbName]; --->  Para criar um banco de dados novo.
#### describe [nomeTabela]; ---> para ver os campos e os tipos de dados .
#### drop table [nomeTabela]; ---> para apagar a tabela.

# Comandos de criação e alteração de tabelas!
#### DDL (Data Definition Language) ---> cuida da estrutura do banco. Ela cria ou muda tabelas e colunas. 
#### DML (Data Manipulation Language) ---> mexe nos dados de dentro dessas tabelas, como inserir ou apagar linhas 

## DML:
#### Select não altera nada no banco, apenas para visualização.
#### select * from [nomeTabela] ; ---> seleciona tudo da tabela.
#### select [coluna] as [nomeQualquer] ---> apresenta somente aquela coluna com outro nome.
#### select 2+2; ---> o select pode mostrar uma conta.
#### select 2+2 as [nome] ---> muda o titulo da tabela no qual aparece a soma

#### insert into [nomeTabela] (campo,campo2) value ('') ---> inserir alguma informação dentro da tabela. '  ' é usado para string/varchar. 

# DDL:
####   create table [nomeTabela] ( ---> criar tabelas, dentro do () colocar estrutura da tabela, informações que serão guardadas
  
###    EXEMPLO:
#### create table usuarios (

#### -> id INT AUTO_INCREMENT PRIMARY KEY, 
#### id: nome da chave
#### INT: tipo de informação (inteiro)
#### AUTO_INCREMENT: o valor é acresentado de forma automática pelo banco de dados. 
#### PRIMARY KEY: seta a chave "id" como primary key da tabela

#### -> nome VARCHAR(100),
#### nome: nome da chave.
#### VARCHAR(100): define tipo de informação, texto. 

#### ->  criado_por VARCHAR(100) DEFAULT (USER())
#### criado_por: nome da chave
#### DEFAULT (USER()): essa chave por padrão vai receber algo, User() é o usuario que está enviando.

#### -> );
#### ); :  usado para finalizar a criação da tabela do banco de dados.
