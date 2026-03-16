# Sistema de Agendamento em Microsserviços

Projeto backend desenvolvido com **Java** e **Spring Boot**, estruturado em **arquitetura de microsserviços**, com o objetivo de simular uma aplicação mais próxima de cenários reais de mercado.

O sistema foi dividido em serviços independentes, cada um com uma responsabilidade específica, permitindo praticar conceitos como separação de responsabilidades, autenticação, integração entre serviços e organização de uma arquitetura distribuída.

---

## Objetivo do projeto

Este projeto foi desenvolvido para aprofundar conhecimentos em:

- desenvolvimento backend com Java e Spring Boot
- arquitetura de microsserviços
- autenticação e autorização
- comunicação entre serviços
- organização de aplicações em módulos independentes
- boas práticas de desenvolvimento backend
- construção de projetos mais próximos de ambientes reais

---

## Arquitetura do sistema

O sistema é composto por **4 microsserviços**, organizados em repositórios separados:

### 1. Serviço de Usuários
Responsável pelo gerenciamento e autenticação de usuários.

**Repositório:**  
[usuario] - https://github.com/pedroppaf/usuario

---

### 2. Serviço de Agendamento / Tarefas
Responsável pelo gerenciamento das tarefas e agendamentos do sistema.

**Repositório:**  
[agendador-tarefas] - https://github.com/pedroppaf/agendador-tarefas

---

### 3. Serviço de Notificação
Responsável pelo tratamento e envio de notificações dentro da arquitetura.

**Repositório:**  
[notificacao] - https://github.com/pedroppaf/notificacao

---

### 4. BFF (Backend For Frontend)
Responsável por atuar como camada intermediária entre cliente e microsserviços, centralizando e organizando chamadas.

**Repositório:**  
[bff-agendador-tarefas] - https://github.com/pedroppaf/bff-agendador-tarefas

---

## Visão geral da arquitetura

```text
Cliente
   │
   ▼
BFF (Backend For Frontend)
   │
   ├── Serviço de Usuários
   ├── Serviço de Agendamento / Tarefas
   └── Serviço de Notificação


## Tecnologias utilizadas

- Java
- Spring Boot
- Spring Security
- JWT
- PostgreSQL
- MongoDB
- Docker/ Docker Compose
- OpenFeign
- Git / GitHub
- Maven / Gradle

## Conceitos aplicados

- arquitetura de microsserviços
- separação de responsabilidades
- autenticação e autorização
- persistência de dados
- integração entre serviços
- backend for frontend (BFF)
- organização em camadas
- boas práticas de desenvolvimento
- construção de APIs REST

##Funcionalidades gerais do sistema

-gerenciamento de usuários
-autenticação e autorização
-gerenciamento de tarefas / agendamentos
-integração entre serviços
-centralização de acesso via BFF
-suporte a notificações

## Como utilizar este projeto
Cada microsserviço possui seu próprio repositório e sua própria configuração.

Para executar o sistema completo, é necessário:

- clonar os repositórios individuais
- configurar as dependências e bancos de dados necessários
- iniciar os serviços separadamente
- utilizar o BFF como ponto principal de acesso
