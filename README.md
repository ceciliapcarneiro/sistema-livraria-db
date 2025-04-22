# Sistema de Banco de Dados para Livraria 📚

Este repositório contém a modelagem e os scripts SQL para um sistema de controle de produtos e pedidos de uma pequena livraria.

## Estrutura do Banco de Dados

### produtos
- `id` (INTEGER, chave primária)
- `nome` (TEXT)
- `preco` (DECIMAL)
- `estoque` (INTEGER)

### pedidos
- `id` (INTEGER, chave primária)
- `data` (DATE)
- `produto_id` (INTEGER, chave estrangeira de produtos)
- `quantidade` (INTEGER)

## Script SQL

O script `livraria.sql`:
- Cria as tabelas
- Insere 3 produtos e 3 pedidos

## Como usar

Você pode importar o script SQL em seu banco de dados local (MySQL, PostgreSQL ou SQLite) para simular a estrutura e os dados.
