# Ecommerce Database Schema

Este repositório contém o esquema de banco de dados para um sistema de ecommerce. O objetivo deste projeto é criar um banco de dados relacional que suporte as operações de um ecommerce, incluindo a gestão de fornecedores, estoque, produtos, vendedores, clientes, pedidos, pagamentos e entregas.

## Objetivo

Refinar o modelo apresentado acrescentando os seguintes pontos:
- Cliente PJ e PF: Uma conta pode ser PJ ou PF, mas não pode ter as duas informações.
- Pagamento: Pode ter cadastrado mais de uma forma de pagamento.
- Entrega: Possui status e código de rastreio.

## Estrutura do Banco de Dados

### Tabelas Principais
- **Fornecedor**: Armazena informações sobre os fornecedores.
- **Estoque**: Armazena informações sobre os estoques.
- **Produto**: Armazena informações sobre os produtos.
- **Terceiro_Vendedor**: Armazena informações sobre os vendedores terceiros.
- **Cliente_PJ**: Armazena informações sobre clientes pessoa jurídica.
- **Cliente_PF**: Armazena informações sobre clientes pessoa física.
- **Pedido**: Armazena informações sobre os pedidos.
- **Pagamento**: Armazena informações sobre os pagamentos.
- **Entrega**: Armazena informações sobre as entregas.

### Relacionamentos
- **Disponibilizando_um_produto**: Relaciona fornecedores e produtos.
- **Produtos_por_Vendedor**: Relaciona vendedores terceiros e produtos.
- **Produto_has_Estoque**: Relaciona produtos e estoques.
- **Relacao_de_Produto_Pedido**: Relaciona produtos e pedidos.

## Como Utilizar

Para criar o banco de dados e as tabelas, execute o script `ecommerce-schema.sql` em seu ambiente MySQL. Certifique-se de ter as permissões adequadas para criar bancos de dados e tabelas.

```sh
mysql -u seu-usuario -p < ecommerce-schema.sql

Contribuição
Sinta-se à vontade para contribuir com este projeto. Abra um pull request com suas melhorias e ajustes.


### Passo 4: Fazer o Commit e Push

1. **Adicione os arquivos ao repositório**:

```sh
git add ecommerce-schema.sql README.md


git commit -m "Adicionar esquema de banco de dados de ecommerce e README"

Envie as mudanças para o GitHub:

git push origin main

