# 🎮 DSList – Catálogo de Games com Java Spring Boot

Projeto desenvolvido durante o **Intensivão Java Spring** ministrado pelo professor **Nelio Alves (DevSuperior)**.  
A aplicação consiste em uma API REST que organiza uma lista de jogos por gênero (como RPG e Plataforma), com funcionalidades de ordenação e reordenação dos games por drag-and-drop.

---

## 🚀 Tecnologias e Ferramentas

- **Java 21**
- **Spring Boot**
- **Spring Data JPA**
- **Hibernate**
- **PostgreSQL**
- **Dbeaver((Em aula: Docker & Docker Compose)**
- **GitHub Actions (CI/CD)**
- **Insomnia (testes de API)**

---

## 📦 Funcionalidades

### ✅ Aula 1 – Fundamentos e Estrutura

- Introdução a sistemas web, arquitetura cliente-servidor, HTTP e JSON
- Estrutura de projeto Spring Boot com API REST
- Mapeamento de entidades com JPA e ORM
- Database Seeding com dados de exemplo
- Padrão de projeto em camadas:
  - `Controller`
  - `Service`
  - `Repository`
- Utilização de DTOs para transferência de dados entre camadas

### 🔄 Aula 2 – Relacionamentos e Consultas

- Mapeamento de relacionamentos N-N com classe de associação
- Uso de `@EmbeddedId` para chave composta
- Consultas customizadas usando Spring Data JPA
- Uso de **Projections** para otimização de resultados específicos

### 🐳 Aula 3 – Infraestrutura e Deploy

- Dicas de carreira: currículo e portfolio
- Criação de ambiente local com **Docker Compose**
- Processo de homologação local completo
- Deploy contínuo com **CI/CD** via GitHub Actions
- Configuração de **CORS** para acesso controlado à API

### 🖱 Aula 4 – Funcionalidade de Reordenação

- Lógica de reordenação de games na lista com **drag-and-drop**
- Atualização da ordem diretamente na memória da aplicação (simulação)

---

## 🗂 Estrutura do Projeto

dslist/
├── src/
│ ├── main/
│ │ ├── java/
│ │ │ └── com/devsuperior/dslist/
│ │ │ ├── config/
│ │ │ ├── controllers/
│ │ │ ├── dto/
│ │ │ ├── entities/
│ │ │ ├── projections/
│ │ │ ├── repositories/
│ │ │ ├── services/
│ │ │ └── DSListApplication.java
│ │ └── resources/
│ │ ├── application.properties
│ │ ├── application.test.properties
│ │ └── import.sql
│ └── test/
├── docker-compose.yml
├── pom.xml
└── README.md

---

## 🧪 Como Executar Localmente

### Pré-requisitos:
- Java 21+
- Docker e Docker Compose(Em aula)
- Git

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/dslist.git
cd dslist

# Suba o ambiente com Dbeaver(Terminal Linux(WSL))
dbeaver-ce

A API estará disponível em:
🔗 http://localhost:8080

## 📬 Endpoints Principais

| Método | Endpoint                          | Descrição                             |
|--------|-----------------------------------|----------------------------------------|
| GET    | `/games`                          | Lista todos os jogos                   |
| GET    | `/games/{id}`                     | Detalhes de um jogo específico         |
| GET    | `/lists`                          | Lista todas as categorias de jogo      |
| GET    | `/lists/{listId}/games`           | Lista de jogos por categoria           |
| POST   | `/lists/{listId}/replacement`     | Reorganiza a posição de um jogo        |


🔐 CORS
Configurado para permitir origens confiáveis durante o desenvolvimento e em produção.

💬 Aprendizados
Durante esse intensivão aprendi:

Estruturação profissional de projeto Spring REST

Práticas modernas de backend

CI/CD com GitHub Actions

Organização por camadas e boas práticas de código limpo

Como pensar a infraestrutura de um sistema backend completo

👨‍🏫 Agradecimentos
Agradeço ao professor Nelio Alves e à equipe da DevSuperior pela didática e qualidade do conteúdo!

“Não basta saber programar, é preciso saber construir sistemas bem organizados, escaláveis e profissionais.” – Nelio Alves

📄 Licença
Este projeto é de caráter educacional, licenciado sob MIT.

📌 Contato
Feito por Kevin Kilmer
🔗 LinkedIn
https://www.linkedin.com/in/kevin-kilmer-50424a28b/

---
