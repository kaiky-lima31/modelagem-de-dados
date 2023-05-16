# Comandos SQL para opereções de dados (DADOS)

## Resumo 

- C: CREATE (criar dados usando o comando INSERT)
- R: READ (ler dados usando o comando)
- U: UPDATE (atualizar dados usando o comando UPDATE)
- D: DELETE (excluir dados usando o comando DELETE)

## INSERT

### Tabela Fabricantes

```sql
INSERT INTO fabricantes (nome) VALUES('Microsoft');
INSERT INTO fabricantes (nome) VALUES('Asus');
INSERT INTO fabricantes (nome) VALUES('Dell');

INSERT INTO fabricantes (nome)
VALUES ('Apple'), ('LG'), ('Samsung'), ('Brastemp');
```

### Tabela de Produtos

```sql
INSERT INTO produtos (nome, descricao, fabricante_id) VALUES ('Ultrabook', 'Laptop de última geração com processador Intel core i9 e memória de 16 gb RAM.', 3);
```

```sql
INSERT INTO  produtos (nome, descricao, fabricante_id) VALUES ('Tablet Android', 'Tablet com a versão 13 do sistema Android, com tela de 10 polegadas e 64 GB de armazenamento.', 6);
```

```sql
INSERT INTO produtos (nome, descricao, fabricante_id) VALUES ('iPhone 13 Pro Max', 'Alta durabilidade, processador XYZ 14, 128 GB de armazenamento, 6 GB de RAM e caro pra caramba.', 4);
```

```sql
INSERT INTO produtos (nome, descricao, fabricante_id) VALUES ('Geladeira', 'Refrigerador frost-free com acesso à Internet e bla bla bla.', 7);
```

```sql
INSERT INTO produtos (nome, descricao, fabricante_id) VALUES ('Xbox 123', 'Vídeo-game de última geração.', 1);
```

```sql
INSERT INTO produtos (nome, descricao, fabricante_id) VALUES ('Ipad mini', 'Tablet Apple com tela retina de 4k', 4);
```

```sql
INSERT INTO produtos (nome, descricao, fabricante_id) VALUES ('Ultrabook', 'Equipamento com processador AMD Ryzen, 12 GB de RAM.', 2);
```
