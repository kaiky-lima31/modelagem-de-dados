# Comandos SQL

```sql
Comandos usados para a modelagem física.
```

## Criar banco de dados

```sql
CREATE DATABASE exemplo_kaiky CHARACTER SET utf8mb4;
```

## Entrar no banco de dados para usá-lo

```sql
USE exemplo_kaiky; (revisar, não funcionou)
```
## Criar a tabela de fabricantes

```sql
CREATE TABLE fabricantes(
    id TINYINT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL
);
```
## Criar a tabela de produtos

```sql
CREATE TABLE produtos(
    id SMALLINT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL,
    descricao TEXT(1000) NOT NULL,
    fabricante_id TINYINT NOT NULL
);
```
## Alterando a tabelaa produtos para criar um relacionamento a partir da coluna fabricante_id, com a coluna id da tabela fabricantes

```sql
ALTER TABLE produtos
    ADD CONSTRAINT fk_produtos_fabricantes
    FOREIGN KEY(fabricante_id) REFERENCES fabricantes(id);
```