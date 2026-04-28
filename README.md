🔐 Auth API - Spring Boot + JWT

API REST de autenticação desenvolvida com Java e Spring Boot, implementando criptografia de senha e geração de tokens JWT para login seguro, seguindo boas práticas de arquitetura backend.

## 🚀 Sobre o projeto

Esta API implementa um fluxo completo de autenticação com:

- Cadastro de usuários com validação
- Criptografia de senha com BCrypt
- Autenticação segura via login
- Geração de tokens JWT com expiração
- Respostas padronizadas com DTO

Projeto estruturado seguindo princípios de separação de responsabilidades e preparado para evolução.

---
## 🧰 Tecnologias

- Java 17
- Spring Boot
- Spring Security
- Spring Data JPA
- H2 Database
- JWT (JSON Web Token)
- Maven

---
## 📁 Arquitetura

- controller → entrada da API
- dto → objetos de transferência
- model → entidades
- repository → acesso ao banco
- security → JWT e autenticação
- config → configurações

---

## 🔐 Exemplo de Login

### 📥 Pedido

```json
{
  "email": "user@email.com",
  "password": "123456"
}{
  "message": "Login OK",
  "token": "jwt_token"
}

git clone https://github.com/diegosilva636/auth-api-springboot-jwt
cd auth-api-springboot-jwt
mvn spring-boot:run
