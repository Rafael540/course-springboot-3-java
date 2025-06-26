

## 🛠️ Projeto Spring Boot - API REST para Gestão de Pedidos

Este projeto é uma aplicação **Spring Boot** que simula um sistema de gerenciamento de **usuários**, **pedidos** e **relacionamentos entre entidades**, como em um cenário de e-commerce. A aplicação segue a arquitetura MVC e aplica boas práticas como camadas separadas (Controller, Service, Repository), injeção de dependência com Spring, e tratamento de exceções.

### ⚙️ Tecnologias Utilizadas

* **Java 17+**
* **Spring Boot**
* **Spring Web**
* **Spring Data JPA**
* **Hibernate**
* **H2 Database (em memória)**
* **Maven**

---

### 📚 Funcionalidades

* 🔍 Listagem de usuários e pedidos (`GET /users`, `GET /orders`)
* 📌 Busca por ID (`/users/{id}`, `/orders/{id}`)
* 🔗 Relacionamento entre `User` e `Order` (um-para-muitos)
* 💾 Persistência em banco H2 com console web disponível (`/h2-console`)
* 📄 Retorno dos dados em formato JSON

---

### ▶️ Como Executar Localmente

1. **Pré-requisitos**:

   * Java 17 ou superior
   * Maven
   * IDE de sua escolha (IntelliJ, Eclipse etc.)

2. **Clone o repositório**:

   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
   ```

3. **Rode a aplicação com Maven**:

   ```bash
   ./mvnw spring-boot:run
   ```

   Ou pela sua IDE, executando a classe com `@SpringBootApplication`.

4. **Acesse os endpoints**:

   * API: `http://localhost:8080/users` e `http://localhost:8080/orders`
   * Console H2: `http://localhost:8080/h2-console`

     * JDBC URL: `jdbc:h2:mem:testdb`
     * Usuário: `sa` (sem senha)

---

