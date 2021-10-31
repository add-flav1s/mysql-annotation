# Estudos de MYSQL

## Conectando ao servidor do banco de dados.

- mysql -h localhost -u root -p


## Mostrando os bancos de dados.

- SHOW DATABASES;


## Criando um banco de dados.

- CREATE DATABASE sistemaDeCadastro;


## Acessando o banco de dados criado.

- USE sistemaDeCadastro;


## Criando uma tabela no banco de dados.

- CREATE TABLE usuarios (
     nome VARCHAR(50),
     email VARCHAR(80),
     idade INT
);


## Mostrando tabelas do banco de dados.

- SHOW TABLES;


## Inserindo dados na tabela.

- INSERT INTO usuarios (nome, email, idade) VALUES (
    'Joao',
    'email@teste.com',
    9
);

- INSERT INTO usuarios (nome, email, idade) VALUES (
    'Maria',
    'email2@teste.com',
    20
);

- INSERT INTO usuarios (nome, email, idade) VALUES (
    'Andre',
    'email3@teste.com',
    32
);

- INSERT INTO usuarios (nome, email, idade) VALUES (
    'Ana',
    'email4@teste.com',
    38
);

- INSERT INTO usuarios (nome, email, idade) VALUES (
    'Flora',
    'email5@teste.com',
    25
);

- INSERT INTO usuarios (nome, email, idade) VALUES (
    'Clara',
    'email6@teste.com',
    17
);

- INSERT INTO usuarios (nome, email, idade) VALUES (
    'Victor',
    'email7@teste.com',
    17
);


## Mostrando os dados da tabela.

- SELECT * FROM usuarios;


## Especificando uma consulta no banco de dados.

- SELECT * FROM usuarios WHERE idade > 18;
- SELECT * FROM usuarios WHERE nome = 'Clara';


## Deletando dados da tabela.

- DELETE FROM usuarios WHERE idade = 17;


## Atualizando dados da tabela.

- UPDATE usuarios SET nome = 'Joaquina' WHERE nome = 'Clara';
