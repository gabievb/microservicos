# 🛠️ Microsserviços com Spring Boot - Warehouse e Storefront

## 📌 Sobre o Projeto
Este projeto foi desenvolvido como parte de um desafio da **DIO (Digital Innovation One)** com o objetivo de criar uma arquitetura de **microsserviços em Java** utilizando **Spring Boot**.  

O sistema é composto por dois microsserviços principais:  
- **Warehouse (Armazém)**: responsável pelo controle de estoque.  
- **Storefront (Vitrine)**: responsável pela interação com os clientes.  

A comunicação entre os serviços ocorre de duas formas:  
- **Síncrona (HTTP)**  
- **Assíncrona (RabbitMQ)**  

---

## 🚀 Tecnologias Utilizadas
- **Java 21**
- **Spring Boot**  
  - Spring Web  
  - Spring Data JPA  
  - Lombok  
  - DevTools  
  - H2 Database  
  - RabbitMQ  
- **Gradle** (gerenciamento de dependências)  
- **Docker** (containers para microsserviços e RabbitMQ)  

---

## ⚙️ Funcionalidades
- Criar e gerenciar produtos no **Warehouse**.  
- Consultar e comprar produtos no **Storefront**.  
- Comunicação síncrona via **REST APIs**.  
- Comunicação assíncrona via **RabbitMQ** para eventos entre microsserviços.  
- Banco de dados em memória **H2** para persistência temporária.  

---

## 🔗 Endpoints Principais

### 📦 Warehouse
- `POST /products` → Cadastrar novo produto.  
- `GET /products` → Listar produtos disponíveis.  

### 🛒 Storefront
- `GET /products` → Consultar produtos disponíveis.  
- `POST /products` → Realizar pedido de produto.  

---

## 🐳 Executando com Docker
O projeto utiliza **Docker** para facilitar a execução dos microsserviços e do RabbitMQ.  

1. **Clonar o repositório:**
   ```
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
   
   ```
2. **Subir o container com docker compose: **
   ```
   docker-compose up --build

   ```
3. **Acessos principais:**

- Warehouse API: http://localhost:8080

- Storefront API: http://localhost:8081

- RabbitMQ Management: http://localhost:15672

---

## 📖  Aprendizados

Com este projeto foi possível:

- Implementar comunicação síncrona e assíncrona entre microsserviços.

- Utilizar RabbitMQ como broker de mensageria.

- Orquestrar containers com Docker.

- Construir APIs RESTful com Spring Boot.

---

