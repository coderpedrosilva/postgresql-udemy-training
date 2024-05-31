# postgresql-udemy-training

-- [SEÇÃO 2]

create table cliente (
	idcliente integer not null,
	nome varchar(50) not null,
	cpf char(11),
	rg varchar(15),
	data_nascimento date,
	genero char(1),
	profissao varchar(30),
	nacionalidade varchar(30),
	logradouro varchar(30),
	numero varchar(10),
	complemento varchar(30),
	bairro varchar(30),
	municipio varchar(30),
	uf varchar(30),
	observacoes text,
	
	constraint pk_cln_idcliente primary key (idcliente)
);

insert into cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
values (1, 'Manoel', '88828383821', '32323', '2001-01-30', 'M', 'Estudante', 'Brasileira', 'Rua Joaquim Nabuco', '23', 'Casa', 'Cidade Nova', 'Porto Uniao', 'SC');

insert into cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
values (2, 'Geraldo', '12343299929', '56565', '1987-01-04', 'M', 'Engenheiro', 'Brasileira', 'Rua das Limas', '200', 'Ap', 'Centro', 'Poro Uniao', 'SC');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (3, 'Maria Oliveira', '11122233344', '123456789', '1985-07-19', 'F', 'Advogada', 'Brasileira', 'Rua das Margaridas', '123', 'Casa 2', 'Centro', 'Porto Alegre', 'RS');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (4, 'Carlos Souza', '22233344455', '234567890', '1990-03-15', 'M', 'Professor', 'Brasileiro', 'Av. das Flores', '456', 'Apto 15', 'Bela Vista', 'Florianópolis', 'SC');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (5, 'Letícia Pereira', '33344455566', '345678901', '1988-09-02', 'F', 'Médica', 'Brasileira', 'Rua dos Pinheiros', '789', 'Casa 10', 'Centro', 'Curitiba', 'PR');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (6, 'Pedro Silva', '44455566677', '456789012', '1992-12-30', 'M', 'Engenheiro', 'Brasileiro', 'Rua dos Lírios', '321', 'Apto 5', 'Jardim Botânico', 'Rio de Janeiro', 'RJ');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (7, 'Clara Mendes', '55566677788', '567890123', '1987-06-25', 'F', 'Arquiteta', 'Brasileira', 'Av. Rio Branco', '987', 'Apto 101', 'Centro', 'Belo Horizonte', 'MG');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (8, 'Lucas Almeida', '66677788899', '678901234', '1995-11-08', 'M', 'Analista de TI', 'Brasileiro', 'Rua Sete de Setembro', '555', 'Casa 7', 'Jardim América', 'Goiânia', 'GO');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (9, 'Camila Santos', '77788899900', '789012345', '1994-04-16', 'F', 'Jornalista', 'Brasileira', 'Av. Paulista', '12', 'Apto 20', 'Jardins', 'São Paulo', 'SP');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (10, 'Rafael Ferreira', '88899900011', '890123456', '1991-08-23', 'M', 'Contador', 'Brasileiro', 'Rua Augusta', '89', 'Apto 10', 'Consolação', 'São Paulo', 'SP');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (11, 'Isabela Martins', '99900011122', '901234567', '1989-05-12', 'F', 'Dentista', 'Brasileira', 'Rua da Paz', '130', 'Casa 3', 'Alto da Boa Vista', 'Recife', 'PE');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (12, 'Gustavo Dias', '00011122233', '012345678', '1993-02-02', 'M', 'Professor', 'Brasileiro', 'Rua dos Girassóis', '250', 'Casa 15', 'Vila Madalena', 'São Paulo', 'SP');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (13, 'Patrícia Lima', '11122233344', '123456789', '1986-07-01', 'F', 'Farmacêutica', 'Brasileira', 'Rua da Alegria', '320', 'Apto 5', 'Santos', 'SP');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (14, 'André Melo', '22233344455', '234567890', '1994-08-19', 'M', 'Médico', 'Brasileiro', 'Rua das Palmeiras', '76', 'Apto 12', 'Barra da Tijuca', 'Rio de Janeiro', 'RJ');

INSERT INTO cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
VALUES (15, 'Fernanda Ramos', '33344455566', '345678901', '1985-03-10', 'F', 'Psicóloga', 'Brasileira', 'Av. Brasil', '2500', 'Apto 8', 'Flamengo', 'Rio de Janeiro', 'RJ');

select * from cliente;

select nome, data_nascimento from cliente;

select nome, data_nascimento as "Data de nascimento" from cliente;

select 'CPF: ' || cpf || ' RG: ' || rg as "CPF e RG" from cliente;

select * from cliente limit 3;

select nome, data_nascimento from cliente where data_nascimento > '2000-01-01';

select nome from cliente where nome like 'C%';

select nome from cliente where nome like '%c%';

select nome, data_nascimento from cliente where data_nascimento between '1990-01-01' and '1998-01-01';

select nome, rg from cliente where rg is null;

select nome from cliente order by nome asc;

select nome from cliente order by nome desc;

-- EXERCÍCIOS - consultas simples

-- 1. O nome, o gênero e a profissão de todos os clientes, ordenado pelo nome em ordem decrescente
select nome, genero, profissao from cliente order by nome desc;

-- 2. Os clientes que tenham a letra “R” no nome
select nome from cliente where nome like '%r%';

-- 3. Os clientes que o nome inicia com a letra “C”
select nome from cliente where nome like 'C%';

-- 4. Os clientes que o nome termina com a letra “A”
select nome from cliente where nome like '%a';

-- 5. Os clientes que moram no bairro “Centro”
select nome, bairro from cliente where bairro = 'Centro';

-- 6. Os clientes que moram em complementos que iniciam com a letra “A”
select nome, complemento from cliente where complemento like 'A%';

-- 7. Somente os clientes do sexo feminino
select nome, genero from cliente where genero like 'F';

-- 8. Os clientes que não informaram o CPF
select nome, cpf from cliente where cpf is null;

-- 9. O nome e a profissão dos clientes, ordenado em ordem crescente pelo nome da profissão
select nome, profissao from cliente order by profissao asc;

-- 10. Os clientes de nacionalidade “Brasileira”
select nome, nacionalidade from cliente where nacionalidade like 'Brasileira';

-- 11. Os clientes que informaram o número da residência
select nome, numero from cliente where numero is not null;

-- 12. Os clientes que moram em Santa Catarina
select nome, uf from cliente where uf like 'SC';

-- 13. Os clientes que nasceram entre 01/01/2000 e 01/01/2002
select nome, data_nascimento from cliente where data_nascimento between '2000-01-01' and '2002-01-01';

-- 14. O nome do cliente e o logradouro, número, complemento, bairro, município e UF concatenado de todos os clientes
select 'Nome: ' || nome || ' - '  ||  'Logradouro: ' || logradouro || ' - '  || 'Numero: '  || numero  || ' - ' || 'Complemento: ' || complemento || ' - '  || 'Bairro: ' || bairro || ' - ' || 'Município: ' || municipio || ' - ' || 'UF: ' || uf from cliente;

select * from cliente;
update cliente set nome = 'Teste' where idcliente = 1;
update cliente set nome = 'Adriana', genero = 'F', numero = '241' where idcliente = 4;
insert into cliente (idcliente, nome) values (16, 'João');
delete from cliente where idcliente = 16;

-- Exercícios – comandos update e delete
-- 1. Insira os dados abaixo na tabela de clientes
insert into cliente (idcliente, nome, cpf, rg, data_nascimento, genero, profissao, nacionalidade, logradouro, numero, complemento, bairro, municipio, uf)
values
(16, 'Maicon', '12349964210', '1234', '1986-10-10', 'F', 'Empresario', null, null, null, null, null, 'Florianópolis', 'SC'),
(17, 'Getulio', null, '4631', null, 'F', 'Estudante', 'Brasileira', 'Rua Central', '349', 'Apartamento', 'Centro', 'Curitiba', 'SC'),
(18, 'Sandra', null, null, null, 'M', 'Professor', 'Italiana', null, '12', 'Bloco A', null, null, null);

-- 2. Altere os dados do cliente Maicon
select * from cliente;
-- a. O CPF para 45390569432
update cliente set cpf = '45390569432' where idcliente = 16;
-- b. O gênero para M
update cliente set genero = 'M' where idcliente = 16;
-- c. A nacionalidade para Brasileira
update cliente set nacionalidade = 'Brasileira' where idcliente = 16;
-- d. O UF para SC
update cliente set uf = 'SC' where idcliente = 16;

-- 3. Altere os dados do cliente Getúlio
select * from cliente;
-- a. A data de nascimento para 01/04/1978
update cliente set data_nascimento = '1978-01-01' where idcliente = 17;
-- b. O gênero para M
update cliente set genero = 'M' where idcliente = 17;

-- 4. Altere os dados da cliente Sandra
select * from cliente;
-- a. O gênero para F
update cliente set genero = 'F' where idcliente = 18;
-- b. A profissão para Professora
update cliente set profissao = 'Professora' where idcliente = 18;
-- c. O número para 123
update cliente set numero = '123' where idcliente = 18;

-- 5. Apague o cliente Maicon
delete from cliente where idcliente = 16;

-- 6. Apague a cliente Sandra
delete from cliente where idcliente = 18;

create table profissao (
	idprofissao integer not null,
	nome varchar(30) not null,
	
	constraint pk_prf_idprofissao primary key (idprofissao),
	constraint un_prf_nome unique (nome)
);

insert into profissao (idprofissao, nome)
values
(1, 'Estudante'),
(2, 'Engenheiro'),
(3, 'Pedreiro'),
(4, 'Jornalista'),
(5, 'Professor');

select * from profissao;

create table nacionalidade (
	idnacionalidade integer not null,
	nome varchar(30) not null,
	
	constraint pk_ncn_idnacionalidade primary key (idnacionalidade),
	constraint un_ncn_nome unique (nome)
);

insert into nacionalidade (idnacionalidade, nome)
values 
(1, 'Brasileira'),
(2, 'Italiana'),
(3, 'Norte-americana'),
(4, 'Alemã');

select * from nacionalidade;

create table complemento (
	idcomplemento integer not null,
	nome varchar(30) not null,
	
	constraint pk_cpl_idcomplemento primary key (idcomplemento),
	constraint un_cpl_nome unique (nome)
);

insert into complemento (idcomplemento, nome) values (1, 'casa');
insert into complemento (idcomplemento, nome) values (2, 'apartamento');

select * from complemento;

create table bairro (
	idbairro integer not null,
	nome varchar(30) not null,
	
	constraint k_brr_idbairro primary key (idbairro),
	constraint un_brr_nome unique (nome)
);

insert into bairro (idbairro, nome)
values 
(1, 'Cidade Nova'),
(2, 'Centro'),
(3, 'São Pedro'),
(4, 'Santa Rosa');

select * from bairro;

select * from cliente;

alter table cliente rename column profissao to idprofissao;
alter table cliente alter column idprofissao type integer;

-- Estudante -> 1, 9, 10, 12, 15, 17 
-- Engenheiro -> 2
-- Pedreiro -> 3
-- Jornalista -> 4, 5
-- Professor -> 6, 7, 8, 13
-- Null -> 11, 14

alter table cliente drop idprofissao; 
alter table cliente add idprofissao integer;
alter table cliente add constraint fk_cln_idprofissao foreign key (idprofissao) references profissao (idprofissao) 

update cliente set idprofissao = 1 where idcliente in (1, 9, 10, 12, 15, 17);
update cliente set idprofissao = 2 where idcliente = 2;
update cliente set idprofissao = 3 where idcliente = 3;
update cliente set idprofissao = 4 where idcliente in (4, 5);
update cliente set idprofissao = 5 where idcliente in (6, 7, 8, 13);
update cliente set idprofissao = null where idcliente in (11, 14);

select * from profissao;
delete from profissao where idprofissao 10;
insert into profissao (idprofissao, nome) values (10, 'Teste');

select * from cliente;
alter table cliente drop column nacionalidade;
alter table cliente add column idnacionalidade integer;
alter table cliente add constraint fk_cln_idnacionalidade foreign key (nacionalidade) references nacionalidade (idnacionalidade);
update cliente set idnacionalidade = 1 where idcliente in (1,2,3,4,6,10,11,14);
update cliente set idnacionalidade = 2 where idcliente in (5,7);
update cliente set idnacionalidade = 3 where idcliente = 8;
update cliente set idnacionalidade = 4 where idcliente in (9,13);

select * from cliente;
alter table cliente drop complemento;
alter table cliente add idcomplemento integer;
alter table cliente add constraint fk_cln_idcomplemento foreign key (idcomplemento) references complemento (idcomplemento);
select * from complemento;
update cliente set idcomplemento = 1 where idcliente in (1,4,9,13);
update cliente set idcomplemento = 1 where idcliente in (2,3,7);

select * from cliente;
alter table cliente drop bairro;
alter table cliente add idbairro integer;
alter table cliente add constraint fk_cln_idbairro foreign key (idbairro) references bairro (idbairro);

select * from bairro;
update cliente set idbairro = 1 where idcliente in (1, 12, 13);
update cliente set idbairro = 2 where idcliente in (2, 3, 6, 8, 9);
update cliente set idbairro = 3 where idcliente in (4, 5);
update cliente set idbairro = 4 where idcliente = 7;

select * from cliente;
create table uf (
	iduf integer not null,
	nome varchar(30) not null,
	sigla char(2) not null,
	
	constraint pk_ufd_idunidade_federacao primary key (iduf),
	constraint un_ufd_nome unique (nome),
	constraint un_ufd_sigla unique (sigla)
);

insert into uf (iduf, nome, sigla) values (1, 'Santa Catarina', 'SC');
insert into uf (iduf, nome, sigla) values (2, 'Paraná', 'PR');
insert into uf (iduf, nome, sigla) values (3, 'São Paulo', 'SP');
insert into uf (iduf, nome, sigla) values (4, 'Minas Gerais', 'MG');
insert into uf (iduf, nome, sigla) values (5, 'Rio Grande do Sul', 'RS');
insert into uf (iduf, nome, sigla) values (6, 'Rio de Janeiro', 'RJ');
select * from uf;

create table municipio (
	idmunicipio integer not null,
	nome varchar(30) not null,
	iduf integer not null,
	
	constraint pk_mnc_idmunicipio primary key (idmunicipio),
	constraint un_mnc_nome unique (nome),
	constraint fk_mnc_iduf foreign key (iduf) references uf (iduf)
);

insert into municipio (idmunicipio, nome, iduf) values (1, 'Porto União', 1);
insert into municipio (idmunicipio, nome, iduf) values (2, 'Canoinhas', 1);
insert into municipio (idmunicipio, nome, iduf) values (3, 'Porto Vitória', 2);
insert into municipio (idmunicipio, nome, iduf) values (4, 'General Carneiro', 2);
insert into municipio (idmunicipio, nome, iduf) values (5, 'São Paulo', 3);
insert into municipio (idmunicipio, nome, iduf) values (6, 'Rio de Janero', 6);
insert into municipio (idmunicipio, nome, iduf) values (7, 'Uberlândia', 4);
insert into municipio (idmunicipio, nome, iduf) values (8, 'Porto Alegre', 5);
insert into municipio (idmunicipio, nome, iduf) values (9, 'União da Vitória', 2);

select * from cliente;
alter table cliente drop municipio;
alter table cliente drop uf;
alter table cliente add idmunicipio integer;
alter table cliente add constraint fk_cliente_idmunicipio foreign key (idmunicipio) references municipio (idmunicipio); 

update cliente set idmunicipio = 1 where idcliente in (1, 2, 10, 11);
update cliente set idmunicipio = 2 where idcliente in (3, 12);
update cliente set idmunicipio = 3 where idcliente in (4);
update cliente set idmunicipio = 4 where idcliente in (5);
update cliente set idmunicipio = 5 where idcliente in (6, 13);
update cliente set idmunicipio = 6 where idcliente in (7);
update cliente set idmunicipio = 7 where idcliente in (8);
update cliente set idmunicipio = 8 where idcliente in (9);
update cliente set idmunicipio = 9 where idcliente in (14, 15);
select * from cliente;

create table fornecedor (
	idfornecedor integer not null,
	nome varchar(50) not null,
	
	constraint pk_frn_idfornecedor primary key (idfornecedor),
	constraint un_frn_nome unique (nome)
);

insert into fornecedor (idfornecedor, nome)
values 
(1, 'Cap. Computadores'),
(2, 'AA. Computadores'),
(3, 'BB. Máquinas');
select * from fornecedor;

create table vendedor (
	idvendedor integer not null,
	nome varchar(50) not null,
	
	constraint pk_vnd_idvendedor primary key (idvendedor),
	constraint un_vnd_nome unique (nome)
);

insert into vendedor (idvendedor, nome)
values
(1, 'André'),
(2, 'Alisson'),
(3, 'José'),
(4, 'Ailton'),
(5, 'Maria'),
(6, 'Suelem'),
(7, 'Aline'),
(8, 'Silvana');
select * from vendedor; 

create table transportadora (
	idtransportadora integer not null,
	idmunicipio integer,
	nome varchar(50) not null,
	logradouro varchar(50),
	numero varchar(10),
	
	constraint pk_trn_idtransportadora primary key (idtransportadora),
	constraint fk_trn_idmunicipio foreign key (idmunicipio) references municipio (idmunicipio),
	constraint un_trn_nome unique (nome)
);

select * from municipio;
insert into transportadora (idtransportadora, idmunicipio, nome, logradouro, numero)
values
(1, 9, 'BS. Transportes', 'Rua das LImas', '01'),
(2, 5, 'União Transportes', null, null);
select * from transportadora;

create table produto (
	idproduto integer not null,
	idfornecedor integer not null,
	nome varchar(50) not null,
	valor float not null,
	
	constraint pk_prd_idproduto primary key (idproduto),
	constraint fk_prd_idfornecedor foreign key (idfornecedor) references fornecedor (idfornecedor)
);

select * from fornecedor;

insert into produto (idproduto, idfornecedor, nome, valor)
values 
(1, 1, 'Microcomputador', 800),
(2, 1, 'Monitor', 500),
(3, 2, 'Placa mãe', 200),
(4, 2, 'HD', 150),
(5, 2, 'Placa de vídeo', 200),
(6, 3, 'Memória RAM', 100),
(7, 1, 'Gabinete', 35);

select * from produto;

create table pedido (
	idpedido integer not null,
	idcliente integer not null,
	idtransportadora integer,
	idvendedor integer not null,
	data_pedido date not null,
	valor float not null,
	
	constraint pk_pdd_idpedido primary key (idpedido),
	constraint fk_pdd_idcliente foreign key (idcliente) references cliente (idcliente),
	constraint fk_pdd_idtransportadora foreign key (idtransportadora) references transportadora (idtransportadora),
	constraint fk_pdd_idvendedor foreign key (idvendedor) references vendedor (idvendedor)
)

select * from cliente;
select * from transportadora;
select * from vendedor;
update cliente set nome = 'Manoel' where idcliente = 1;
insert into pedido (idpedido, data_pedido, valor, idcliente, idtransportadora, idvendedor)
values 
(1, '01-04-2008', 1300, 1, 1, 1),
(2, '01-04-2008', 500, 1, 1, 1),
(3, '02-04-2008', 300, 2,  2, 5),
(4, '05-04-2008', 1000, 3,  1, 7),
(5, '06-04-2008', 200, 4, 2, 6),
(6, '06-04-2008', 1985, 5, 1, 6),
(7, '06-04-2008', 800, 5, 1, 7),
(8, '06-04-2008', 175, 6, null, 7), 
(9, '07-04-2008', 1300, 7, null, 8),
(10, '10-04-2008', 200, 8, 1, 8),
(11, '15-04-2008', 300, 9, 2, 1),
(12, '20-04-2008', 500, 9, 2, 5),
(13, '20-04-2008', 350, 4, 1, 7),
(14, '23-04-2008', 300, 10, 1 , 5), 
(15, '25-04-2008', 200, 2, null, 5);

select * from pedido;

create table pedido_produto (
	idpedido integer not null,
	idproduto integer not null,
	quantidade integer not null,
	valor_unitario float not null,
	
	constraint pk_pdp_idpedidoproduto primary key (idpedido, idproduto),
	constraint fk_pdp_idpedido foreign key (idpedido) references pedido (idpedido),
	constraint fk_pdp_idproduto foreign key (idproduto) references produto (idproduto)
)

select * from produto;
select * from pedido_produto;

insert into pedido_produto (idpedido, idproduto, quantidade, valor_unitario) 
values 
(1, 1, 1, 800),
(1, 2, 1, 500),
(2, 2, 1, 500),
(3, 4, 2, 150),
(4, 1, 1, 800),
(4, 3, 1, 200),
(5, 3, 1, 200),
(6, 1, 2, 800),
(6, 7, 1, 35),
(6, 5, 1, 200),
(6, 4, 1, 150),
(7, 1, 1, 800),
(8, 7, 5, 35),
(9, 1, 1, 800),
(9, 2, 1, 800),
(10, 5, 1, 200),
(11, 5, 1, 200),
(11, 6, 1, 100),
(12, 2, 1, 800),
(13, 3, 1, 200),
(13, 4, 1, 150),
(14, 6, 3, 100),
(15, 3, 1, 200);

-- Exercícios – consultas simples

-- 1. Somente o nome de todos os vendedores em ordem alfabética.
select nome from vendedor order by nome asc; 

-- 2. Os produtos que o preço seja maior que R$200,00, em ordem crescente pelo preço.
select nome, valor from produto where valor > 200 order by valor asc;

-- 3. O nome do produto, o preço e o preço reajustado em 10%, ordenado pelo nome do produto.
select nome, valor,  valor + (valor * 10) / 100 as reajuste from produto order by nome asc;

-- 4. Os municípios do Rio Grande do Sul.
select * from uf;
select * from municipio where iduf = 5;

-- 5. Os pedidos feitos entre 10/04/2008 e 25/04/2008 ordenado pelo valor.
select * from pedido where data_pedido between '2008-04-10' and '2008-04-25' order by valor;

-- 6. Os pedidos que o valor esteja entre R$1.000,00 e R$1.500,00.
select * from pedido where valor between 100 and 500;

-- 7. Os pedidos que o valor não esteja entre R$100,00 e R$500,00.
select * from pedido where valor not between 100 and 500;

-- 8. Os pedidos do vendedor André ordenado pelo valor em ordem decrescente.
select * from vendedor;
select * from pedido where idvendedor = 1 order by valor desc;

-- 9. Os pedidos do cliente Manoel ordenado pelo valor em ordem crescente.
select * from cliente;
select * from pedido where idcliente = 1 order by valor asc;

-- 10. Os pedidos da cliente Jéssica que foram feitos pelo vendedor André.
select * from pedido where idcliente = 9 and idvendedor = 1

-- 11. Os pedidos que foram transportados pela transportadora União Transportes.
select * from transportadora;
select * from pedido where idtransportadora = 2;

-- 12. Os pedidos feitos pela vendedora Maria ou pela vendedora Aline.
select * from vendedor;
select * from pedido where idvendedor = 5 or idvendedor = 7;

-- 13. Os clientes que moram em União da Vitória ou Porto União.
select * from municipio;
select * from cliente where idmunicipio = 1 or idmunicipio = 9;

-- 14. Os clientes que não moram em União da Vitória e nem em Porto União.
select * from cliente where idmunicipio <> 1 and idmunicipio <> 9;

-- 15. Os clientes que não informaram o logradouro.
select * from cliente where logradouro is null;

-- 16. Os clientes que moram em avenidas.
select * from cliente where logradouro like 'Av%';

-- 17. Os vendedores que o nome começa com a letra S.
select * from vendedor where nome like 'S%';

-- 18. Os vendedores que o nome termina com a letra A.
select * from vendedor where nome like '%a';

-- 19. Os vendedores que o nome não começa com a letra A.
select * from vendedor where nome not like 'A%';

-- 20. Os municípios que começam com a letra P e são de Santa Catarina.
select * from uf;
select * from municipio where nome like 'P%' and iduf = 1;

-- 21. As transportadoras que informaram o endereço.
select * from transportadora where logradouro is not null;

-- 22. Os itens do pedido 01.
select * from pedido_produto where idpedido = 1;

-- 23. Os itens do pedido 06 ou do pedido 10.
select * from pedido_produto where idpedido = 6 or idpedido = 10;

-- Funções agregadas

-- average, tirar média
select avg(valor) from pedido;

-- arredondando para duas casas decimais
select cast(avg(valor) as numeric(10,2)) from pedido;

-- contar (considerando campos not null)
select count(idmunicipio) from municipio;

-- contar (independente de campos null)
select count(*) from municipio;

select * from transportadora;
select count(logradouro) from transportadora;
select count(idtransportadora) from transportadora;

select * from municipio;
select count(idmunicipio) from municipio where iduf = 2;

select max(valor) from pedido;

select min(valor), max(valor) from pedido;

select sum(valor) from pedido;

-- ao utilizar o group by é necessário usar sum ou count ou outra função para agrupar
select idcliente, sum(valor) from pedido group by idcliente order by idcliente asc;

select idcliente, sum(valor) from pedido group by idcliente having sum(valor) > 500;

-- Exercícios – funções agregadas

-- 1. A média dos valores de vendas dos vendedores que venderam mais que R$ 200,00.
select idvendedor, avg(valor) from pedido group by idvendedor having avg(valor) > 200;

-- 2. Os vendedores que venderam mais que R$ 1500,00.
select idvendedor, sum(valor) from pedido group by idvendedor having sum(valor) > 1500;

-- 3. O somatório das vendas de cada vendedor.
select idvendedor, sum(valor) from pedido group by idvendedor;

-- 4. A quantidade de municípios.
select count(idmunicipio) from municipio;

-- 5. A quantidade de municípios que são do Paraná ou de Santa Catarina.
select * from uf;
select count(idmunicipio) from municipio where iduf = 1 or iduf = 2;

-- 6. A quantidade de municípios por estado.
select iduf, count(idmunicipio) from municipio group by iduf;

-- 7. A quantidade de clientes que informaram o logradouro.
select count(idcliente) from cliente where logradouro is not null;

-- 8. A quantidade de clientes por município.
select idmunicipio, count(idcliente) from cliente group by idmunicipio;

-- 9. A quantidade de fornecedores.
select count(idfornecedor) from fornecedor;

-- 10. A quantidade de produtos por fornecedor.
select idfornecedor, count(idproduto) from produto group by idfornecedor;

-- 11. A média de preços dos produtos do fornecedor Cap. Computadores.
select * from fornecedor;
select avg(valor) from produto where idfornecedor = 1;

-- 12. O somatório dos preços de todos os produtos.
select sum(valor) from produto;

-- 13. O nome do produto e o preço somente do produto mais caro.
select nome, valor from produto order by valor desc limit 1;

-- 14. O nome do produto e o preço somente do produto mais barato.
select nome, valor from produto order by valor asc limit 1;

-- 15. A média de preço de todos os produtos.
select avg(valor) from produto;

-- 16. A quantidade de transportadoras.
select count(idtransportadora) from transportadora;

-- 17. A média do valor de todos os pedidos.
select avg(valor) from pedido;

-- 18. O somatório do valor do pedido agrupado por cliente.
select idcliente, sum(valor) from pedido group by idcliente;

-- 19. O somatório do valor do pedido agrupado por vendedor.
select idvendedor, sum(valor) from pedido group by idvendedor;

-- 20. O somatório do valor do pedido agrupado por transportadora.
select idtransportadora, sum(valor) from pedido group by idtransportadora;

-- 21. O somatório do valor do pedido agrupado pela data.
select data_pedido, sum(valor) from pedido group by data_pedido;

-- 22. O somatório do valor do pedido agrupado por cliente, vendedor e transportadora.
select idcliente, idvendedor, idtransportadora, sum(valor) from pedido group by idcliente, idvendedor, idtransportadora;

-- 23. O somatório do valor do pedido que esteja entre 01/04/2008 e 10/12/2009 e que seja maior que R$ 200,00.
select sum(valor) from pedido where data_pedido between '2008-04-01' and '2009-12-10' and valor > 200;

-- 24. A média do valor do pedido do vendedor André.
select * from vendedor;
select avg(valor) from pedido where idvendedor = 1;

-- 25. A média do valor do pedido da cliente Jéssica.
select * from cliente;
select avg(valor) from pedido where idcliente = 15;

-- 26. A quantidade de pedidos transportados pela transportadora BS. Transportes.
select * from transportadora;
select count(idpedido) from pedido where idtransportadora = 1;

-- 27. A quantidade de pedidos agrupados por vendedor.
select idvendedor, count(idpedido) from pedido group by idvendedor;

-- 28. A quantidade de pedidos agrupados por cliente.
select idcliente, count(idpedido) from pedido group by idcliente;

-- 29. A quantidade de pedidos entre 15/04/2008 e 25/04/2008.
select count(idpedido) from pedido where data_pedido between '2008-04-15' and '2008-04-25';

-- 30. A quantidade de pedidos que o valor seja maior que R$ 1.000,00.
select count(idpedido) from pedido where valor > 1000;

-- 31. A quantidade de microcomputadores vendida.
select * produto;
select sum(quantidade) from pedido_produto where idproduto = 1;

-- 32. A quantidade de produtos vendida agrupado por produto.
select idproduto, sum(quantidade) from pedido_produto group by idproduto;

-- 33. O somatório do valor dos produtos dos pedidos, agrupado por pedido.
select idpedido, sum(valor_unitario) from pedido_produto group by idpedido;

-- 34. A quantidade de produtos agrupados por pedido.
select idpedido, sum(quantidade) from pedido_produto group by idpedido; 

-- 35. O somatório do valor total de todos os produtos do pedido.
select sum(valor_unitario) from pedido_produto;

-- 36. A média dos produtos do pedido 6.
select avg(valor_unitario) from pedido_produto where idpedido = 6;

-- 37. O valor do maior produto do pedido.
select max(valor_unitario) from pedido_produto;

-- 38. O valor do menor produto do pedido.
select min(valor_unitario) from pedido_produto;

-- 39. O somatório da quantidade de produtos por pedido.
select idpedido, sum(quantidade) from pedido_produto group by idpedido;

-- 40. O somatório da quantidade de todos os produtos do pedido.
select sum(valor_unitario) from pedido_produto;

-- Relacionamentos com joins
select
	cln.nome as cliente,
	prf.nome as profissao
from
	cliente as cln
left outer join
	profissao as prf on cln.idprofissao = prf.idprofissao

select
	cln.nome as cliente,
	prf.nome as profissao
from
	cliente as cln
inner join
	profissao as prf on cln.idprofissao = prf.idprofissao

select
	cln.nome as cliente,
	prf.nome as profissao
from
	cliente as cln
right outer join
	profissao as prf on cln.idprofissao = prf.idprofissao

-- Exercícios – joins

-- 1. O nome do cliente, a profissão, a nacionalidade, o logradouro, o número, o complemento, o bairro, o município e a unidade de federação.
select
	cln.nome as cliente,
	prf.nome as profissao,
	ncn.nome as nacionalidade,
	cln.logradouro,
	cln.numero,
	cmp.nome as complemento,
	brr.nome as bairro,
	mnc.nome as municipio,
	uf.nome as estado,
	uf.sigla 
from
	cliente as cln
left outer join
	profissao as prf on cln.idprofissao = prf.idprofissao
left outer join
	nacionalidade as ncn on cln.idnacionalidade = ncn.idnacionalidade
left outer join
	complemento cmp on cln.idcomplemento = cmp.idcomplemento
left outer join 
	bairro brr on cln.idbairro = brr.idbairro
left outer join
	municipio mnc on cln.idmunicipio = mnc.idmunicipio
left outer join
	uf on mnc.iduf = uf.iduf

-- 2. O nome do produto, o valor e o nome do fornecedor.
select 
	prd.nome as produto,
	prd.valor,
	frn.nome as fornecedor
from
	produto prd
left outer join
	fornecedor frn on prd.idfornecedor = frn.idfornecedor

-- 3. O nome da transportadora e o município.
select 
	trs.nome as transportadora,
	mnc.nome as município
from 
	transportadora trs
left outer join
	municipio mnc on trs.idmunicipio = mnc.idmunicipio

-- 4. A data do pedido, o valor, o nome do cliente, o nome da transportadora e o nome do vendedor.
select
	pdd.data_pedido,
	pdd.valor,
	cln.nome as cliente,
	trn.nome as transportadora,
	vnd.nome as vendedor
from
	pedido pdd
left outer join
	cliente cln on pdd.idcliente = cln.idcliente
left outer join
	transportadora trn on pdd.idtransportadora = trn.idtransportadora
left outer join
	vendedor vnd on pdd.idvendedor = vnd.idvendedor

-- 5. O nome do produto, a quantidade e o valor unitário dos produtos do pedido.
select 
	pdt.nome as produto,
	pdp.quantidade,
	pdp.valor_unitario
from 
	pedido_produto pdp
left outer join
	produto pdt on pdp.idproduto = pdt.idproduto

-- 6. O nome dos clientes e a data do pedido dos clientes que fizeram algum pedido (ordenado pelo nome do cliente).
select
	cln.nome,
	pdd.data_pedido
from
	cliente cln
inner join
	pedido pdd on pdd.idcliente = cln.idcliente
order by
	cln.nome

-- 7. O nome dos clientes e a data do pedido de todos os clientes, independente se tenham feito pedido (ordenado pelo nome do cliente).
select
	cln.nome,
	pdd.data_pedido
from
	cliente cln
left outer join
	pedido pdd on pdd.idcliente = cln.idcliente
order by
	cln.nome

-- 8. O nome da cidade e a quantidade de clientes que moram naquela cidade.
select
	mnc.nome as municipio,
	count(cln.idcliente) as quantidade
from
	cliente cln
inner join
	municipio mnc on cln.idmunicipio = mnc.idmunicipio
group by
	mnc.nome

-- 9. O nome do fornecedor e a quantidade de produtos de cada fornecedor.
select
	frn.nome as fornecedor,
	count(pdd.idproduto)
from
	produto pdd
left outer join
	fornecedor frn on pdd.idfornecedor = frn.idfornecedor
group by
	frn.nome

-- 10.O nome do cliente e o somatório do valor do pedido (agrupado por cliente).
select 
	cln.nome as cliente,
	sum(pdd.valor) as total
from
	pedido pdd
left outer join
	cliente cln on pdd.idcliente = cln.idcliente
group by
	cln.nome

-- 11.O nome do vendedor e o somatório do valor do pedido (agrupado por vendedor).
select 
	vnd.nome as vendedor,
	sum(pdd.valor) as total
from
	pedido pdd
left outer join
	vendedor vnd on pdd.idvendedor = vnd.idvendedor
group by 
	vnd.nome

-- 12.O nome da transportadora e o somatório do valor do pedido (agrupado por transportadora).
select
	trn.nome as transportdora,
	sum(pdd.valor) as total
from
	pedido pdd
inner join
	transportadora trn on pdd.idtransportadora = trn.idtransportadora
group by
	trn.nome
	
-- 13.O nome do cliente e a quantidade de pedidos de cada um (agrupado por cliente).
select
	cln.nome as cliente,
	count(pdd.idpedido) as total
from
	pedido pdd
left outer join
	cliente cln on pdd.idcliente = cln.idcliente
group by
	cln.nome

-- 14.O nome do produto e a quantidade vendida (agrupado por produto).
select 
	pdt.nome as produto,
	sum(pdp.quantidade) as total
from 
	pedido_produto pdp
left outer join
	produto pdt on pdp.idproduto = pdt.idproduto
group by
	pdt.nome

-- 15.A data do pedido e o somatório do valor dos produtos do pedido (agrupado pela data do pedido).
select
	pdd.data_pedido,
	sum(pdp.valor_unitario) as total
from
	pedido_produto pdp
left outer join
	pedido pdd on pdp.idpedido = pdd.idpedido
group by
	pdd.data_pedido

-- 16.A data do pedido e a quantidade de produtos do pedido (agrupado pela data do pedido).
select
	pdd.data_pedido,
	sum(pdp.quantidade) as quantidade
from
	pedido_produto pdp
left outer join
	pedido pdd on pdp.idpedido = pdd.idpedido
group by
	pdd.data_pedido

-- Comandos adicionais
select * from pedido;
select 
	data_pedido, 
	extract(day from data_pedido),
	extract(month from data_pedido),
	extract(year from data_pedido)
from 
	pedido

select nome, substring(nome from 1 for 5), substring(nome, 2) from cliente

select nome, upper(nome) from cliente

select nome, cpf, coalesce(cpf, 'não informado') from cliente

select
	case sigla
		when 'PR' then 'Paraná'
		when 'SC' then 'Santa Catarina'
	else 'outros'
	end as uf
from
	uf
	
-- Exercícios – comandos adicionais

-- 1. O nome do cliente e somente o mês de nascimento. Caso a data de nascimento não esteja preenchida mostrar a mensagem “Não informado”.
select * from cliente

select 
	nome,
	coalesce(extract(month from data_nascimento), 0)
from cliente

-- 2. O nome do cliente e somente o nome do mês de nascimento (Janeiro, Fevereiro etc). Caso a data de nascimento não esteja preenchida mostrar a mensagem “Não informado”.
select
	nome,
	case extract(month from data_nascimento)
		when 1 then 'Janeiro'
		when 2 then 'Fevereiro'
		when 3 then 'Março'
		when 4 then 'Abril'
		when 5 then 'Maio'
		when 6 then 'Junho'
		when 7 then 'Julho'
		when 8 then 'Agosto'
		when 9 then 'Setembro'
		when 10 then 'Outubro'
		when 11 then 'Novembro'
		when 12 then 'Dezembro'
	else
		'Nao informado'
	end as mes
from cliente

-- 3. O nome do cliente e somente o ano de nascimento. Caso a data de nascimento não esteja preenchida mostrar a mensagem “Não informado”.
select
	nome,
	coalesce(extract(year from data_nascimento), 0)
from
	cliente
	
-- 4. O caractere 5 até o caractere 10 de todos os municípios.
select nome, substring(nome from 5 for 5) from municipio

-- 5. O nome de todos os municípios em letras maiúsculas.
select nome, upper(nome) from municipio

-- 6. O nome do cliente e o gênero. Caso seja M mostrar “Masculino”, senão mostrar “Feminino”.
select
	nome,
	case genero
		when 'M' then 'Masculino'
		when 'F' then 'Feminino'
	end as genero
from
	cliente

-- 7. O nome do produto e o valor. Caso o valor seja maior do que R$ 500,00 mostrar a mensagem “Acima de 500”, caso contrário, mostrar a mensagem “Abaixo de 500”.
select
	nome,
	valor,
	case 
		when valor >= 500 then 'Acima ou igual a 500'
	else 
		'abaixo de 500'
	end as faixa
from
	produto

-- Subconsultas

-- Selecionar a data do pedido e o valor onde o valor seja maior que a média dos
-- valores de todos os pedidos
select
	data_pedido,
	valor
from
	pedido
where
	valor > (select avg(valor) from pedido)

-- Exemplo com count
select 
	pdd.data_pedido,
	pdd.valor,
	(select sum(quantidade) from pedido_produto pdp where pdp.idpedido = pdd.idpedido) as total
from	
	pedido pdd
	
-- Exemplo com update
select * from pedido

update pedido set valor = valor + ((valor * 5) / 100) where valor > (select avg(valor) from pedido)

-- Exercícios - subconsultas

-- 1. O nome dos clientes que moram na mesma cidade do Manoel. Não deve ser mostrado o Manoel.
select
	nome,
	idmunicipio
from
	cliente
where
	idmunicipio = (select idmunicipio from cliente where nome = 'Manoel')
and
	idcliente <> 1

select * from cliente

-- 2. A data e o valor dos pedidos que o valor do pedido seja menor que a média de todos os pedidos.
select 
	data_pedido,
	valor
from
	pedido
where 
	valor < (select avg(valor) from pedido)

-- 3. A data,o valor, o cliente e o vendedor dos pedidos que possuem 2 ou mais produtos.
select 
	pdd.data_pedido,
	pdd.valor,
	cln.nome as cliente,
	vnd.nome as vendedor,
	(select sum(quantidade) from pedido_produto pdp where pdp.idpedido = pdd.idpedido)
from 
	pedido pdd
left outer join 
	cliente cln on pdd.idcliente = cln.idcliente 
left outer join
	vendedor vnd on pdd.idvendedor = vnd.idvendedor
where
	(select sum(quantidade) from pedido_produto pdp where pdp.idpedido = pdd.idpedido) >= 2

select * from pedido_produto

-- 4. O nome dos clientes que moram na mesma cidade da transportadora BSTransportes.
select 
	nome,
	idmunicipio
from 
	cliente
where idmunicipio =	(select idmunicipio from transportadora where idtransportadora = 1)

select * from transportadora

-- 5. O nome do cliente e o município dos clientes que estão localizados no mesmo município de qualquer uma das transportadoras.
select
	nome,
	idmunicipio
from
	cliente
where
	idmunicipio in (select distinct(idmunicipio) from transportadora)

select distinct(idmunicipio) from cliente

-- 6. Atualizar o valor do pedido em 5% para os pedidos que o somatório do valor total dos produtos daquele pedido seja maior que a média do valor total de todos os produtos de todos os pedidos.
update 
	pedido 
set 
	valor = valor + ((valor * 5) / 100)
where 
	(select sum(pdp.valor_unitario) from pedido_produto pdp where pdp.idpedido = pedido.idpedido) > (select avg(valor_unitario) from pedido_produto)

-- Teste
select 
	idpedido,
	(select sum(valor_unitario) from pedido_produto pdp where pdp.idpedido = pdd.idpedido)
from 
	pedido pdd

select avg(valor_unitario) from pedido_produto

select * from pedido_produto

select * from pedido

-- 7. O nome do cliente e a quantidade de pedidos feitos pelo cliente.
select
	cln.nome,
	(select count(idpedido) from pedido pdd where pdd.idcliente = cln.idcliente) as total 
from
	cliente cln

-- 8. Para revisar, refaça o exercício anterior (número 07) utilizando group by e mostrando somente os clientes que fizeram pelo menos um pedido.
select
	cln.nome as cliente,
	count(pdd.idpedido) as total
from
	pedido pdd
left outer join
	cliente cln on pdd.idcliente = cln.idcliente
group by 
	cln.nome

-- Views
drop view cliente_profissao;

create view cliente_profissao as
select 
	cln.nome as cliente,
	cln.cpf,
	prf.nome as profissao
from 
	cliente cln
left outer join
	profissao prf on cln.idprofissao = prf.idprofissao

select cliente from cliente_profissao where profissao = 'Professor'
select * from cliente_profissao

-- Exercícios views

-- 1. O nome, a profissão, a nacionalidade, o complemento, o município, a unidade de federação, o bairro, o CPF,o RG, a data de nascimento, o gênero (mostrar “Masculino” ou “Feminino”), o logradouro, o número e as observações dos clientes.
create view cliente_dados as
select
	cln.nome as cliente,
	prf.nome as profissao,
	ncn.nome as nacionalidade,
	cmp.nome as complemento,
	mnc.nome as municipio,
	uf.nome as unidade_federacao,
	brr.nome as bairro,
	cln.rg,
	cln.cpf,
	cln.data_nascimento,
	case cln.genero
		when 'M' then 'Masculino'
		when 'F' then 'Feminino'
	end as genero,
	cln.logradouro, 
	cln.numero, 
	cln.observacoes
from
	cliente cln
left outer join
	profissao prf on cln.idprofissao = prf.idprofissao
left outer join 
	nacionalidade ncn on cln.idnacionalidade = ncn.idnacionalidade
left outer join
	complemento cmp on cln.idcomplemento = cmp.idcomplemento
left outer join
	municipio mnc on cln.idmunicipio = mnc.idmunicipio
left outer join
	uf on mnc.iduf = uf.iduf
left outer join
	bairro brr on cln.idbairro = brr.idbairro
	
select * from cliente_dados;

-- 2. O nome do município e o nome e a sigla da unidade da federação.
create view municipio_uf as
select
	mnc.nome as municipio,
	uf.nome as unidade_federacao,
	uf.sigla
from
	municipio mnc
left outer join
	uf on mnc.iduf = uf.iduf

select * from municipio_uf

-- 3. O nome do produto, o valor e o nome do fornecedor dos produtos.
create view produto_fornecedor as
select 
	prd.nome as produto,
	prd.valor,
	frn.nome as fornecedor
from
	produto prd
left outer join
	fornecedor frn on prd.idfornecedor = frn.idfornecedor

-- 4. O nome da transportadora, o logradouro, o número, o nome da unidade de federação e a sigla da unidade de federação das transportadoras.
create view transportadora_uf as
select
	trn.nome as transportadora,
	trn.logradouro,
	trn.numero,
	uf.nome as unidade_federacao,
	uf.sigla
from
	transportadora trn
left outer join 
	municipio mnc on trn.idmunicipio = mnc.idmunicipio
left outer join
	uf on mnc.iduf = uf.iduf
	
select * from transportadora_uf where sigla = 'PR'

-- 5. A data do pedido, o valor, o nome da transportadora, o nome do cliente e o nome do vendedor dos pedidos.
create view dados_pedido as
select 
	pdd.data_pedido,
	pdd.valor,
	trn.nome as transportadora,
	cln.nome as cliente,
	vnd.nome as vendedor
from
	pedido pdd
left outer join
	transportadora trn on pdd.idtransportadora = trn.idtransportadora
left outer join
	cliente cln on pdd.idcliente = cln.idcliente
left outer join
	vendedor vnd on pdd.idvendedor = vnd.idvendedor

select * from dados_pedido

-- 6. O nome do produto, a quantidade, o valor unitário e o valor total dos produtos do pedido.
create view produto_pedido as
select
	prd.nome as produto,
	pdp.quantidade,
	pdp.valor_unitario
from
	pedido_produto pdp
left outer join
	produto prd on pdp.idproduto = prd.idproduto

select * from produto_pedido

-- Campos autoincremento
create table exemplo (
	idexemplo serial not null,
	nome varchar(50) not null,
	
	constraint pk_exemplo_idexemplo primary key (idexemplo)
);

insert into exemplo (nome) values ('Exemplo 1');
insert into exemplo (nome) values ('Exemplo 2');
insert into exemplo (nome) values ('Exemplo 3');
insert into exemplo (nome) values ('Exemplo 4');
insert into exemplo (nome) values ('Exemplo 5');

select * from exemplo

select max(idbairro) + 1 from bairro
create sequence bairro_id_seq minvalue 5
alter table bairro alter idbairro set default nextval('bairro_id_seq')
alter sequence bairro_id_seq owned by bairro.idbairro
insert into bairro (nome) values ('teste 1');
insert into bairro (nome) values ('teste 2');
select * from bairro

-- Exercícios sequences – auto incremento

-- 1. Criar sequências para todas as outras tabelas da base de dados

-- a. Cliente
select max(idcliente) + 1 from cliente
create sequence cliente_id_seq minvalue 18
alter table cliente alter idcliente set default nextval('cliente_id_seq')
alter sequence cliente_id_seq owned by cliente.idcliente
insert into cliente (nome) values ('Teste sequência')
select * from cliente

-- b. Complemento
select max(idcomplemento) + 1 from complemento
create sequence complemento_id_seq minvalue 3
alter table complemento alter idcomplemento set default nextval('complemento_id_seq')
alter sequence complemento_id_seq owned by complemento.idcomplemento
insert into complemento (nome) values ('Teste sequência')
select * from complemento

-- c. Fornecedor
select max(idfornecedor) + 1 from fornecedor
create sequence fornecedor_id_seq minvalue 4
alter table fornecedor alter idfornecedor set default nextval('fornecedor_id_seq')
alter sequence fornecedor_id_seq owned by fornecedor.idfornecedor
insert into fornecedor (nome) values ('Teste sequência')
select * from fornecedor

-- d. Município
select max(idmunicipio) + 1 from municipio
create sequence municipio_id_seq minvalue 10
alter table municipio alter idmunicipio set default nextval('municipio_id_seq')
alter sequence municipio_id_seq owned by municipio.idmunicipio
insert into municipio (nome, iduf) values ('Teste sequência', 1)
select * from municipio

-- e. Nacionalidade
select max(idnacionalidade) + 1 from nacionalidade
create sequence nacionalidade_id_seq minvalue 5
alter table nacionalidade alter idnacionalidade set default nextval('nacionalidade_id_seq')
alter sequence nacionalidade_id_seq owned by nacionalidade.idnacionalidade
insert into nacionalidade (nome) values ('Teste sequência')
select * from nacionalidade

-- f. Pedido
select max(idpedido) + 1 from pedido
create sequence pedido_id_seq minvalue 16
alter table pedido alter idpedido set default nextval('pedido_id_seq')
alter sequence pedido_id_seq owned by pedido.idpedido
insert into pedido (data_pedido, valor, idcliente, idvendedor) 
values (current_date, 130, 1, 1)
select * from pedido

-- g. Pedido produto (verificar se é necessário)
-- não é necessário criar

-- h. Profissão
select max(idprofissao) + 1 from profissao
create sequence profissao_id_seq minvalue 6
alter table profissao alter idprofissao set default nextval('profissao_id_seq')
alter sequence profissao_id_seq owned by profissao.idprofissao
insert into profissao (nome) values ('Teste sequência')
select * from profissao

-- i. Transportadora
select max(idtransportadora) + 1 from transportadora
create sequence transportadora_id_seq minvalue 3
alter table transportadora alter idtransportadora set default nextval('transportadora_id_seq')
alter sequence transportadora_id_seq owned by transportadora.idtransportadora
insert into transportadora (nome) values ('Teste sequência')
select * from transportadora

-- j. UF
select max(iduf) + 1 from uf
create sequence uf_id_seq minvalue 7
alter table uf alter iduf set default nextval('uf_id_seq')
alter sequence uf_id_seq owned by uf.iduf
insert into uf (nome, sigla) values ('Teste sequência', 'TE')
select * from uf

-- k. Vendedor
select max(idvendedor) + 1 from vendedor
create sequence vendedor_id_seq minvalue 9
alter table vendedor alter idvendedor set default nextval('vendedor_id_seq')
alter sequence vendedor_id_seq owned by vendedor.idvendedor
insert into vendedor (nome) values ('Teste sequência')
select * from vendedor

-- L. Produto
select max(idproduto) + 1 from produto
create sequence produto_id_seq minvalue 8
alter table produto alter idproduto set default nextval('produto_id_seq')
alter sequence produto_id_seq owned by produto.idproduto

-- Campos default
alter table pedido alter column data_pedido set default current_date;
alter table pedido alter column valor set default 0;
insert into pedido (idcliente, idvendedor) values (1, 1)
insert into pedido (idcliente, idvendedor, data_pedido, valor) 
values (1, 1, '2022-10-10', 234)
select * from pedido

-- Exercícios valores default

-- 1. Adicione valores default na tabela de produtos do pedido
-- a. Quantidade com o valor 1
-- b. Valor unitário com o valor 0
alter table pedido_produto alter column quantidade set default 1;
alter table pedido_produto alter column valor_unitario set default 0;

insert into pedido_produto (idpedido, idproduto) values (1, 3);
insert into pedido_produto (idpedido, idproduto, quantidade, valor_unitario)
values (1, 4, 5, 100)
select * from pedido_produto 

-- 2. Adicione valor default na tabela de produtos
-- a. Valor com o valor 0
alter table produto alter column valor set default 0;
insert into produto (nome, idfornecedor) values ('Teste default', 1);
insert into produto (nome, idfornecedor, valor) values ('Teste default', 1, 50);
select * from produto

-- Índices
create index idx_cln_nome on cliente (nome);

-- Exercícios índices

-- 1. Adicione índices nas seguintes tabelas e campos
-- a. Pedido – data do pedido
-- b. Produto – nome
drop index idx_pdd_data_pedido
create index idx_pdd_data_pedido on pedido (data_pedido)
create index idx_pdr_nome on produto (nome)

-- [AVALIAÇÃO]

-- [SEÇÃO 3]

-- Funções
select valor, concat('R$ ', round(cast(valor as numeric), 2)) from pedido

create function formata_moeda(valor float) returns varchar(20) language plpgsql as
$$
begin
	return concat('R$ ', round(cast(valor as numeric), 2));
end;
$$;

select valor, formata_moeda(valor) from pedido
select valor, formata_moeda(valor) from produto

create function get_nome_by_id(idc integer) returns varchar(50) language plpgsql as
$$
declare r varchar(50);
begin
	select nome into r from cliente where idcliente = idc;
	return r;
end;
$$

select data_pedido, valor, idcliente, get_nome_by_id(idcliente) from pedido

-- Exercícios funções
-- 1. Crie uma função que receba como parâmetro o ID do pedido e retorne o valor total deste pedido
drop function get_valor_pedido
create or replace function get_valor_pedido(idpdd integer) returns varchar(20) language plpgsql as
$$
begin
	return (select formata_moeda(pdd.valor) from pedido pdd where pdd.idpedido = idpdd);
end;
$$;

select get_valor_pedido(idpedido) from pedido

-- 2. Crie uma função chamada “maior”, que quando executada retorne o pedido com o maior valor
select * from pedido
select idpedido from pedido where valor = (select max(valor) from pedido)

create or replace function get_maior_pedido() returns integer language plpgsql as
$$
begin
	return (select idpedido from pedido where valor = (select max(valor) from pedido));
end
$$

select get_maior_pedido() from pedido
select get_maior_pedido();

-- Stored procedures
create procedure insere_bairro(nome_bairro varchar(50)) language sql as 
$$
	insert into bairro (nome) values (nome_bairro);
$$;

call insere_bairro('Teste procedure')
select * from bairro

-- Exercícios procedures
-- 1. Crie uma stored procedure que receba como parâmetro o ID do produto e o percentual de aumento, e reajuste o preço somente deste produto de acordo com o valor passado como parâmetro
create or replace procedure reajusta_produto(idp integer, percentual float) language sql as
$$
	update produto set valor = valor + ((valor * percentual) / 100) where idproduto = idp;
$$;
select * from produto
call reajusta_produto(1, 10)

-- 2. Crie uma stored procedure que receba como parâmetro o ID do produto e exclua da base de dados somente o produto com o ID correspondente
create or replace procedure apagar_produto(idp integer) language sql as
$$
	delete from produto where idproduto = idp;
$$;

select * from produto
call apagar_produto(9)

-- Triggers
create table bairro_auditoria (
	idbairro integer not null,
	data_criacao timestamp not null
)

create or replace function bairro_log() returns trigger language plpgsql as
$$
begin
	insert into bairro_auditoria (idbairro, data_criacao) values (new.idbairro, current_timestamp);
	return new;
end;
$$

create or replace trigger log_bairro_trigger after insert on bairro for each row execute procedure bairro_log();

call insere_bairro ('Teste 10');
call insere_bairro ('Teste 20');
call insere_bairro ('Teste 30');
select * from bairro
select * from bairro_auditoria

-- Exercícios triggers
-- 1. Crie uma tabela chamada PEDIDOS_APAGADOS
select * from pedido

create table pedidos_apagados (
	idpedido integer not null,
	idcliente integer not null,
	idtransportadora integer,
	idvendedor integer not null,
	data_pedido date not null,
	valor float not null,
	data_apagado date not null
)

alter table pedidos_apagados alter column data_apagado type timestamp

-- 2. Faça uma trigger que quando um pedido for apagado, todos os seus dados devem ser copiados para a tabela PEDIDOS_APAGADOS
create or replace function pedido_log() returns trigger language plpgsql as
$$
begin
	insert into pedidos_apagados (idpedido, idcliente, idtransportadora, idvendedor, data_pedido, valor, data_apagado)
	values (old.idpedido, old.idcliente, old.idtransportadora, old.idvendedor, old.data_pedido, old.valor, current_timestamp);
	return old;
end;
$$

create or replace trigger log_pedido_trigger before delete on pedido for each row execute procedure pedido_log();

select * from pedido

select idpedido from pedido where idpedido not in (select idpedido from pedido_produto)

delete from pedido where idpedido = 17

select * from pedidos_apagados

-- Domínios
-- Ids
create domain idcurto as smallint;
create domain idmedio as integer;
create domain idlongo as bigint;

-- Caracteres
create domain sigla as char(3);
create domain codigo as varchar(10);
create domain nome_curto as varchar(15);
create domain nome_medio as varchar(50);
create domain nome_longo as varchar(70);
create domain documento as varchar(15);
create domain tipo as char(1);
create domain texto as text;

-- Data e hora
create domain data as date;
create domain hora as time;
create domain data_hora timestamp;

-- Numéricos
create domain moeda as numeric(10,2);
create domain float_curto as numeric(6,2);
create domain float_medio as numeric(10,2);
create domain float_longo as numeric(15,2);
create domain quantidade as smallint;

drop view cliente_dados;

alter table bairro alter column nome type nome_medio;

alter table bairro_auditoria alter column data_criacao type data_hora;

drop view cliente_profissao
drop view dados_pedido

alter table cliente alter column nome type nome_longo;
alter table cliente alter column cpf type documento;
alter table cliente alter column rg type documento;
alter table cliente alter column data_nascimento type data; 
alter table cliente alter column genero type tipo;
alter table cliente alter column logradouro type nome_longo;
alter table cliente alter column numero type nome_curto;
alter table cliente alter column idprofissao type  idmedio;
alter table cliente alter column idnacionalidade type idmedio;
alter table cliente alter column idbairro type idmedio;
alter table cliente alter column idmunicipio type idmedio;
alter table cliente alter column idcomplemento type idmedio;

alter table complemento alter column nome type nome_medio;

drop view produto_fornecedor;

alter table fornecedor alter column nome type nome_medio;

drop view municipio_uf
drop view transportadora_uf

alter table municipio alter column nome type nome_medio;
alter table municipio alter column iduf type idmedio;

alter table nacionalidade alter column nome type nome_medio;

alter table pedido alter column idpedido type bigint;
alter table pedido alter column idcliente type idmedio;
alter table pedido alter column idtransportadora type idmedio;
alter table pedido alter column idvendedor type idmedio;
alter table pedido alter column data_pedido type data;
alter table pedido alter column valor type moeda;

drop view produto_pedido

alter table pedido_produto alter column idpedido type idlongo;
alter table pedido_produto alter column idproduto type idmedio;
alter table pedido_produto alter column quantidade type quantidade;
alter table pedido_produto alter column valor_unitario type moeda;

alter table pedidos_apagados alter column idpedido type idlongo;
alter table pedidos_apagados alter column idcliente type idmedio;
alter table pedidos_apagados alter column idtransportadora type idmedio;
alter table pedidos_apagados alter column idvendedor type idmedio;
alter table pedidos_apagados alter column data_pedido type data;
alter table pedidos_apagados alter column valor type moeda;

alter table produto alter column idfornecedor type idmedio;
alter table produto alter column nome type nome_medio;
alter table produto alter column valor type moeda;

alter table profissao alter column nome type nome_medio;

alter table transportadora alter column idmunicipio type idmedio;
alter table transportadora alter column nome type nome_medio;
alter table transportadora alter column logradouro type nome_longo;
alter table transportadora alter column numero type nome_curto;

alter table uf alter column nome type nome_medio;
alter table uf alter column sigla type sigla;

alter table vendedor alter column nome type nome_medio;

-- Recriar as views 

-- Usuários e permissões
create role gerente;
create role estagiario;

grant select, insert, delete, update on bairro, cliente, complemento, fornecedor, municipio, nacionalidade, pedido, pedido_produto, produto, profissao, transportadora, uf, vendedor to gerente with grant option; 
grant all on all sequences in schema public to gerente;
-- revoke

grant select on cliente_dados, dados_pedido to estagiario;

create role maria login password '123' in role gerente;
create role pedro login password '321' in role estagiario;

-- Testes em outra aba com login maria (senha 123)
select * from cliente
insert into cliente (nome) values ('Teste permissão')
delete from cliente where idcliente = 21

select * from cliente_dados

-- Testes em outra aba com login pedro (senha 321)
select * from cliente
select * from bairro
insert into bairro (nome) values ('Teste permissão')

select * from cliente_dados
select * from dados_pedido

-- Exercícios usuários e permissões

-- 1. Crie um novo papel chamado “atendente”
create role atendente;

-- 2. Defina somente permissões para o novo papel poder selecionar e incluir novos pedidos (tabelas pedido e pedido_produto). O restante do acesso deve estar bloqueado
grant select, insert on pedido, pedido_produto to atendente with grant option;
grant all on pedido_id_seq to atendente with grant option;

-- 3. Crie um novo usuário associado ao novo papel
create role joao login password '123' in role atendente;

-- 4. Realize testes (no novo login) para verificar se as permissões foram aplicadas corretamente
select * from pedido;
select * from pedido_produto;

update pedido_produto set quantidade = 2 where idpedido = 1 and idproduto = 1
insert into pedido (idcliente, idvendedor) values (1, 2)
select * from pedido;

-- Transações
create table conta (
	idconta serial not null,
	cliente nome_medio not null,
	saldo moeda not null default 0,
	
	constraint pk_cnt_idconta primary key (idconta)
)

insert into conta (cliente, saldo) values ('cliente 1', 1000);
insert into conta (cliente, saldo) values ('cliente 2', 500);

select * from conta

update conta set saldo = saldo - 100 where idconta = 1;
update conta set saldo = saldo + 100 where idconta = 2;

begin;
update conta set saldo = saldo - 100 where idconta = 1;
update conta set saldo = saldo + 100 where idconta = 2;
rollback;

begin;
update conta set saldo = saldo - 100 where idconta = 1;
update conta set saldo = saldo + 100 where idconta = 2;
commit;
