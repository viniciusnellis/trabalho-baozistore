# Baozi Store API 🥟

**Disciplina:** Desenvolvimento Web Back-End - UNINTER  
**Desenvolvedor:** Vinicius Francisco Nellis

## 📌 Sobre o Projeto
Este projeto é uma API REST desenvolvida como requisito da Atividade Prática da disciplina de Desenvolvimento Web Back-End. O sistema simula o controle básico (CRUD) de clientes, produtos e pedidos para uma loja fictícia chamada **Baozi Store**, que vende pãozinho chinês.

## 🚀 Tecnologias Utilizadas
* **Java** (JDK 17+)
* **Spring Boot** (Web, Data JPA)
* **Banco de Dados:** H2 Database (em memória)
* **Gerenciamento de Dependências:** Maven
* **Testes de API:** Postman

## ⚙️ Arquitetura do Projeto
O projeto segue o padrão MVC adaptado para APIs REST, organizado nos seguintes pacotes principais:
* `model`: Entidades de banco de dados (Cliente, Produto, Pedido).
* `repository`: Interfaces de comunicação com o banco de dados via Spring Data JPA.
* `controller`: Controladores REST que expõem os endpoints da API.

## 🔗 Endpoints da API

A API roda localmente na porta `8080`. A URL base é: `http://localhost:8080`

### Clientes (`/clientes`)
* `POST /clientes` - Cadastra um novo cliente.
* `GET /clientes` - Lista todos os clientes.
* `GET /clientes/{id}` - Consulta um cliente específico pelo ID.
* `DELETE /clientes/{id}` - Remove um cliente do sistema.

### Produtos (`/produtos`)
* `POST /produtos` - Cadastra um novo produto (ex: Baozi Tradicional de Porco).
* `GET /produtos` - Lista todos os produtos.
* `GET /produtos/{id}` - Consulta um produto específico pelo ID.
* `DELETE /produtos/{id}` - Remove um produto do sistema.

### Pedidos (`/pedidos`)
* `POST /pedidos` - Registra um novo pedido vinculando um cliente e um produto.
* `GET /pedidos` - Lista todos os pedidos.
* `GET /pedidos/{id}` - Consulta um pedido específico pelo ID.
* `DELETE /pedidos/{id}` - Remove um pedido do sistema.

## 🛠️ Como Executar o Projeto

1. Certifique-se de ter o **Java JDK** instalado na sua máquina.
2. Clone este repositório ou baixe o código-fonte.
3. Importe o projeto (pasta contendo o `pom.xml`) na sua IDE de preferência (Eclipse, IntelliJ, VS Code).
4. Aguarde o Maven baixar as dependências.
5. Execute a classe principal `BaozistoreApplication.java`.
6. A API estará disponível em `http://localhost:8080`.
7. O banco de dados H2 é em memória. Os dados são reiniciados a cada execução.
