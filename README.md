# 💸 Desafio NGBilling NGbank

API RESTful desenvolvida como parte do desafio técnico, simulando operações bancárias como criação de contas e realização de transações.

---

## 🚀 Tecnologias

- **Java 17+** (compatível com Java 23)
- **Spring Boot 3.4.6**
- **Spring Data JPA**
- **H2 Database (em memória)**
- **Lombok**
- **ModelMapper**
- **Springdoc OpenAPI (Swagger 3)**

---

## 📦 Como rodar o projeto

### ✅ Pré-requisitos

- JDK 17 ou superior
- Maven 3.8+

### 🔧 Passos

```bash
# Clone o repositório
git clone https://github.com/kaiquemribeiro/desafio-ngbilling.git

# Entre no diretório do projeto
cd desafio-ngbilling

# Compile e rode a aplicação
./mvnw spring-boot:run
```
---

## ✅ Testes

Para rodar os testes unitários:
```
./mvnw test
```

---

## 📚 Documentação da API

Após iniciar o projeto, acesse a documentação Swagger em:

📘 [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

---

## 🔁 Endpoints principais

### `POST /conta`
Cria uma nova conta bancária.

**Body exemplo:**
```json
{
  "numeroConta": 1234,
  "saldo": 1000.00
}
```

### `GET /conta=123`
Consulta os dados de uma conta pelo número da conta.

**Response exemplo:**
```json
{
  "numeroConta": 1234,
  "saldo": 1000.00
}
```

### `POST /transacao`
Realiza uma transação.

**Body exemplo:**
```json
{
  "numeroConta" : "1234",
  "formaPagamento" : "P",
  "valor" : "100.0"
}
```

**Response exemplo:**
```json
{
  "numeroConta": 1234,
  "saldo": 900.00
}
```
---

## 🧠 Boas práticas

Este projeto foi desenvolvido seguindo os princípios do SOLID:

- **S** — Princípio da Responsabilidade Única  
- **O** — Princípio do Aberto/Fechado  
- **L** — Princípio da Substituição de Liskov  
- **I** — Princípio da Segregação de Interface  
- **D** — Princípio da Inversão de Dependência

Esses princípios garantem um código mais modular, reutilizável, testável e de fácil manutenção.

---

## 📊 Badges

![Java](https://img.shields.io/badge/Java-17%2B-blue)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.4.6-brightgreen)


