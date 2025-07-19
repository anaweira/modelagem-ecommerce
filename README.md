# Projeto de Modelagem Conceitual de E-commerce

Este projeto faz parte do desafio proposto pela **DIO**, no qual foi solicitado o desenvolvimento de um **modelo conceitual de banco de dados** para um sistema de E-commerce, utilizando o modelo Entidade-Relacionamento (ER). A proposta foca em representar os principais elementos envolvidos em um processo de compra online, com base em requisitos previamente definidos.

---

## Objetivo

Construir um esquema conceitual capaz de representar:

- A estrutura de **clientes (PF e PJ)**
- As possíveis **formas de pagamento**
- Os **pedidos realizados**
- As **entregas associadas aos pedidos**

---

## Descrição Geral do Modelo

O modelo foi elaborado com base nos seguintes requisitos:

1. **Cliente** pode ser:
   - **Pessoa Física**, com CPF, nome e data de nascimento;
   - **Pessoa Jurídica**, com CNPJ, razão social e nome fantasia;
   - Um cliente pode ser **apenas PF ou PJ**, nunca os dois.

2. **Forma de Pagamento**:
   - O cliente pode ter **mais de uma forma de pagamento** cadastrada;
   - Relacionamento muitos-para-muitos modelado através da tabela associativa `Forma Pagamento`.

3. **Pedido**:
   - Cada pedido é vinculado a um **cliente** e a uma **forma de pagamento**;
   - Contém informações como data e valor total.

4. **Entrega**:
   - Cada pedido possui uma entrega;
   - A entrega possui **status** e **código de rastreio**.

---

## 📈 Diagrama Conceitual

> Diagrama desenvolvido no [draw.io](https://draw.io)
