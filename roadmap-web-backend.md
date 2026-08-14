# Roadmap — Web Development Backend

> Trilha focada em **Backend Web**, com frontend suficiente para compreender e construir aplicações web completas, evoluindo para **JavaScript → TypeScript → Node.js → APIs → Bancos de Dados → Arquitetura → Cloud**.

## Objetivo

Construir uma base sólida para atuar como **Backend Developer**, inicialmente com Node.js/TypeScript, mantendo conhecimento suficiente de frontend para desenvolver interfaces, consumir APIs e eventualmente atuar como Full Stack.

---

## 1. Fundamentos da Web

- [ ] Internet x Web
- [ ] Cliente e servidor
- [ ] Browser
- [ ] DNS
- [ ] IP
- [ ] Portas
- [ ] TCP/IP — fundamentos
- [ ] URL
- [ ] HTTP
- [ ] HTTPS
- [ ] Request / Response
- [ ] Headers
- [ ] Body
- [ ] Status Codes
- [ ] Cookies
- [ ] Sessões
- [ ] JSON
- [ ] REST
- [ ] CORS

### HTTP

- [ ] GET
- [ ] POST
- [ ] PUT
- [ ] PATCH
- [ ] DELETE

### Status Codes

- [ ] 200
- [ ] 201
- [ ] 204
- [ ] 400
- [ ] 401
- [ ] 403
- [ ] 404
- [ ] 409
- [ ] 422
- [ ] 500

### Projeto

- [ ] Criar uma página HTML que consuma uma API utilizando `fetch()`

---

# 2. HTML

## Fundamentos

- [ ] Estrutura HTML
- [ ] Elementos
- [ ] Atributos
- [ ] HTML semântico
- [ ] Links
- [ ] Imagens
- [ ] Listas
- [ ] Tabelas
- [ ] Formulários
- [ ] Inputs
- [ ] Buttons
- [ ] Select
- [ ] Textarea
- [ ] Labels
- [ ] `data-*`

## HTML Semântico

- [ ] `<header>`
- [ ] `<nav>`
- [ ] `<main>`
- [ ] `<section>`
- [ ] `<article>`
- [ ] `<footer>`

### Projeto

- [ ] Criar uma página de login
- [ ] Criar uma página de cadastro
- [ ] Criar uma página de listagem
- [ ] Criar um formulário completo

---

# 3. CSS

## Fundamentos

- [ ] Seletores
- [ ] Especificidade
- [ ] Box Model
- [ ] `display`
- [ ] `position`
- [ ] Unidades
- [ ] Cores
- [ ] Fontes
- [ ] Margins
- [ ] Padding
- [ ] Borders

## Layout

- [ ] Flexbox
- [ ] CSS Grid
- [ ] Positioning

## Responsividade

- [ ] Media Queries
- [ ] Mobile First
- [ ] Viewport
- [ ] Layouts responsivos

### Objetivo

Ser capaz de construir interfaces simples e responsivas:

- [ ] Login
- [ ] Cadastro
- [ ] Dashboard
- [ ] Tabelas
- [ ] Navbar
- [ ] Cards
- [ ] Formulários

> **Não é necessário aprofundar em CSS avançado neste momento.**

---

# 4. JavaScript

## Fundamentos

- [ ] `let`
- [ ] `const`
- [ ] `var`
- [ ] Strings
- [ ] Numbers
- [ ] Booleans
- [ ] `null`
- [ ] `undefined`
- [ ] Objects
- [ ] Arrays
- [ ] Operadores
- [ ] Condicionais
- [ ] Loops

## Funções

- [ ] Function Declaration
- [ ] Function Expression
- [ ] Arrow Functions
- [ ] Parâmetros
- [ ] Return
- [ ] Escopo
- [ ] Closures

## Estruturas de Dados

- [ ] Array
- [ ] Object
- [ ] Map
- [ ] Set

## Métodos de Array

- [ ] `map()`
- [ ] `filter()`
- [ ] `reduce()`
- [ ] `find()`
- [ ] `findIndex()`
- [ ] `some()`
- [ ] `every()`
- [ ] `sort()`
- [ ] `forEach()`

## JavaScript Moderno

- [ ] Destructuring
- [ ] Spread Operator
- [ ] Rest Parameters
- [ ] Template Literals
- [ ] Optional Chaining
- [ ] Nullish Coalescing
- [ ] Modules
- [ ] `import`
- [ ] `export`

---

# 5. JavaScript Assíncrono

> Uma das partes mais importantes para trabalhar com Node.js.

- [ ] Callbacks
- [ ] Promises
- [ ] `async/await`
- [ ] `try/catch`
- [ ] `Promise.all()`
- [ ] `Promise.allSettled()`
- [ ] Event Loop
- [ ] Call Stack
- [ ] Task Queue
- [ ] Microtask Queue

### Projeto

- [ ] Consumir uma API externa
- [ ] Tratar erros de requisição
- [ ] Fazer múltiplas requisições assíncronas
- [ ] Trabalhar com loading e erros no frontend

---

# 6. JavaScript no Browser

- [ ] DOM
- [ ] Seleção de elementos
- [ ] Manipulação de elementos
- [ ] Events
- [ ] Event Listeners
- [ ] Forms
- [ ] Validação básica
- [ ] LocalStorage
- [ ] SessionStorage
- [ ] Fetch API
- [ ] JSON

### Projeto

## Task Manager

Criar uma aplicação frontend que consuma uma API:

```text
GET    /tasks
POST   /tasks
PATCH  /tasks/:id
DELETE /tasks/:id
```

---

# 7. TypeScript

> Aprender TypeScript depois de possuir uma base sólida de JavaScript.

## Tipos

- [ ] Type Annotations
- [ ] Type Inference
- [ ] `string`
- [ ] `number`
- [ ] `boolean`
- [ ] `object`
- [ ] Arrays
- [ ] Tuples
- [ ] `any`
- [ ] `unknown`
- [ ] `never`
- [ ] `null`
- [ ] `undefined`

## Type System

- [ ] `type`
- [ ] `interface`
- [ ] Union Types
- [ ] Intersection Types
- [ ] Literal Types
- [ ] Optional Properties
- [ ] Type Narrowing
- [ ] Type Guards
- [ ] `typeof`
- [ ] `keyof`

## Generics

- [ ] Generic Functions
- [ ] Generic Interfaces
- [ ] Generic Types
- [ ] Constraints

## Utility Types

- [ ] `Partial`
- [ ] `Pick`
- [ ] `Omit`
- [ ] `Record`
- [ ] `Readonly`

## Módulos

- [ ] ES Modules
- [ ] Imports
- [ ] Exports
- [ ] `tsconfig.json`

---

# 8. Node.js

## Fundamentos

- [ ] Node.js Runtime
- [ ] V8
- [ ] npm
- [ ] `package.json`
- [ ] `package-lock.json`
- [ ] Dependencies
- [ ] Dev Dependencies
- [ ] CommonJS
- [ ] ES Modules
- [ ] Environment Variables
- [ ] `process`

## APIs do Node

- [ ] `fs`
- [ ] `path`
- [ ] `events`
- [ ] Streams
- [ ] Buffers
- [ ] HTTP

## Conceitos

- [ ] Event Loop
- [ ] Async I/O
- [ ] Non-blocking I/O
- [ ] Process
- [ ] Threads — fundamentos

---

# 9. Express

> Primeiro framework de Backend para compreender claramente o funcionamento de uma API.

- [ ] Criar servidor
- [ ] Routes
- [ ] Controllers
- [ ] Middleware
- [ ] Request
- [ ] Response
- [ ] Query Parameters
- [ ] Route Parameters
- [ ] Request Body
- [ ] HTTP Status Codes
- [ ] Error Handling
- [ ] Middleware de autenticação

### Arquitetura inicial

```text
Request
   ↓
Middleware
   ↓
Route
   ↓
Controller
   ↓
Service
   ↓
Database
   ↓
Response
```

### Projeto

- [ ] Criar uma REST API completa
- [ ] CRUD
- [ ] Validação
- [ ] Tratamento de erros
- [ ] Middleware
- [ ] Paginação
- [ ] Filtros
- [ ] Ordenação

---

# 10. SQL e PostgreSQL

> SQL continua sendo uma competência central para Backend.

## SQL

- [ ] SELECT
- [ ] INSERT
- [ ] UPDATE
- [ ] DELETE
- [ ] WHERE
- [ ] ORDER BY
- [ ] GROUP BY
- [ ] HAVING
- [ ] JOINs
- [ ] Subqueries
- [ ] CTEs
- [ ] Window Functions

## Modelagem

- [ ] Entidades
- [ ] Atributos
- [ ] Chaves primárias
- [ ] Chaves estrangeiras
- [ ] Relacionamentos
- [ ] Cardinalidade
- [ ] Normalização
- [ ] Constraints

## PostgreSQL

- [ ] Instalação
- [ ] Databases
- [ ] Schemas
- [ ] Tables
- [ ] Indexes
- [ ] Views
- [ ] Transactions
- [ ] Isolation Levels
- [ ] Locks
- [ ] `EXPLAIN`
- [ ] Query Optimization — fundamentos

---

# 11. ORM — Prisma

- [ ] Instalação
- [ ] Schema
- [ ] Models
- [ ] Relations
- [ ] Migrations
- [ ] CRUD
- [ ] Queries
- [ ] Filtering
- [ ] Pagination
- [ ] Transactions
- [ ] Seed
- [ ] Integração com PostgreSQL

> **Regra:** ORM não substitui conhecimento de SQL.

```text
Prisma
   ↓
SQL
   ↓
PostgreSQL
```

---

# 12. Arquitetura de Backend

- [ ] Separation of Concerns
- [ ] Controllers
- [ ] Services
- [ ] Repositories
- [ ] DTOs
- [ ] Dependency Injection
- [ ] Layered Architecture
- [ ] Modular Architecture
- [ ] Error Handling
- [ ] Validation
- [ ] Serialization

## Boas práticas

- [ ] Clean Code
- [ ] SOLID
- [ ] DRY
- [ ] KISS
- [ ] YAGNI
- [ ] Design Patterns

---

# 13. NestJS

> Framework principal para aprofundamento em Backend Node.js/TypeScript.

- [ ] CLI
- [ ] Modules
- [ ] Controllers
- [ ] Providers
- [ ] Services
- [ ] Dependency Injection
- [ ] Pipes
- [ ] Guards
- [ ] Interceptors
- [ ] Middleware
- [ ] Exception Filters
- [ ] DTOs
- [ ] Validation
- [ ] Configuration
- [ ] Authentication
- [ ] Authorization
- [ ] Database Integration

### Projeto

- [ ] Migrar uma API Express para NestJS
- [ ] Organizar módulos
- [ ] Implementar autenticação
- [ ] Implementar autorização
- [ ] Implementar validação
- [ ] Implementar testes

---

# 14. Autenticação e Segurança

## Authentication

- [ ] Authentication x Authorization
- [ ] Sessions
- [ ] Cookies
- [ ] JWT
- [ ] Access Tokens
- [ ] Refresh Tokens
- [ ] Password Hashing
- [ ] bcrypt
- [ ] Argon2

## Authorization

- [ ] Roles
- [ ] Permissions
- [ ] RBAC
- [ ] Resource Authorization

## Web Security

- [ ] CORS
- [ ] CSRF
- [ ] XSS
- [ ] SQL Injection
- [ ] Rate Limiting
- [ ] Input Validation
- [ ] Secrets
- [ ] Environment Variables
- [ ] HTTPS
- [ ] Security Headers

---

# 15. Testes

## Tipos

- [ ] Unit Tests
- [ ] Integration Tests
- [ ] End-to-End Tests
- [ ] API Tests

## Conceitos

- [ ] Assertions
- [ ] Mocks
- [ ] Stubs
- [ ] Fixtures
- [ ] Test Doubles
- [ ] Test Pyramid

## Ferramentas

- [ ] Jest
- [ ] Supertest
- [ ] Test Database

### Projeto

- [ ] Testar Services
- [ ] Testar Controllers
- [ ] Testar Endpoints
- [ ] Testar integração com PostgreSQL
- [ ] Testar autenticação

---

# 16. Git e GitHub

> Utilizar desde o início da formação.

- [ ] `git init`
- [ ] `git clone`
- [ ] `git status`
- [ ] `git add`
- [ ] `git commit`
- [ ] `git push`
- [ ] `git pull`
- [ ] `git fetch`
- [ ] `git branch`
- [ ] `git switch`
- [ ] `git merge`
- [ ] `git rebase`
- [ ] `git stash`
- [ ] `git log`
- [ ] `git diff`

## GitHub

- [ ] Pull Requests
- [ ] Code Review
- [ ] Merge Conflicts
- [ ] Issues
- [ ] Branching Strategies
- [ ] Conventional Commits
- [ ] GitHub Actions

---

# 17. Docker

- [ ] Containers
- [ ] Images
- [ ] Dockerfile
- [ ] Docker Hub
- [ ] Volumes
- [ ] Networks
- [ ] Environment Variables
- [ ] Docker Compose
- [ ] Multi-stage Builds
- [ ] Container Health Checks

### Projeto

Criar ambiente:

```text
Docker Compose
│
├── API
├── PostgreSQL
└── Redis
```

---

# 18. Redis

- [ ] Conceito de Cache
- [ ] Keys
- [ ] Strings
- [ ] Lists
- [ ] Sets
- [ ] Hashes
- [ ] TTL
- [ ] Pub/Sub
- [ ] Sessions
- [ ] Cache
- [ ] Rate Limiting

---

# 19. Filas e Workers

## Conceitos

- [ ] Message Queue
- [ ] Producer
- [ ] Consumer
- [ ] Worker
- [ ] Retry
- [ ] Dead Letter Queue
- [ ] Idempotência
- [ ] Processamento assíncrono

## Tecnologias

- [ ] BullMQ
- [ ] Redis
- [ ] RabbitMQ

## Posteriormente

- [ ] Apache Kafka
- [ ] Event Streaming

### Projeto

```text
API
 ↓
Queue
 ↓
Worker
 ↓
Processamento
 ↓
Database / External API
```

---

# 20. Frontend — React

> Aprender apenas o suficiente para atuar como Backend/Full Stack.

## React

- [ ] Components
- [ ] Props
- [ ] State
- [ ] Events
- [ ] Hooks
- [ ] `useState`
- [ ] `useEffect`
- [ ] Forms
- [ ] Conditional Rendering
- [ ] Lists
- [ ] API Calls
- [ ] Routing

## Integração

- [ ] React + TypeScript
- [ ] React + REST API
- [ ] Authentication
- [ ] JWT/Cookies
- [ ] Error Handling
- [ ] Loading States
- [ ] TanStack Query — posteriormente

> **Não priorizar inicialmente:** Redux avançado, Next.js avançado, SSR/RSC, design systems, animações complexas e arquitetura avançada de frontend.

---

# 21. AWS

> Cloud principal para aprofundamento.

## Fundamentos

- [ ] Cloud Computing
- [ ] Regions
- [ ] Availability Zones
- [ ] IAM
- [ ] Security Groups
- [ ] VPC — fundamentos

## Serviços

- [ ] EC2
- [ ] S3
- [ ] RDS
- [ ] Lambda
- [ ] API Gateway
- [ ] CloudWatch
- [ ] ECR
- [ ] ECS
- [ ] SQS
- [ ] SNS
- [ ] DynamoDB

---

# 22. CI/CD

## GitHub Actions

- [ ] Workflows
- [ ] Jobs
- [ ] Steps
- [ ] Actions
- [ ] Secrets
- [ ] Environment Variables
- [ ] Artifacts

## Pipeline

```text
Git Push
   ↓
Lint
   ↓
Tests
   ↓
Build
   ↓
Docker
   ↓
Deploy
```

### Projeto

- [ ] Criar pipeline CI
- [ ] Executar testes automaticamente
- [ ] Executar lint
- [ ] Build automático
- [ ] Criar Docker Image
- [ ] Fazer deploy automático

---

# 23. Arquitetura Avançada

> Estudar depois de possuir experiência prática construindo APIs e sistemas.

## Arquitetura

- [ ] Modular Monolith
- [ ] Clean Architecture
- [ ] DDD
- [ ] Bounded Context
- [ ] Domain Model
- [ ] Dependency Inversion
- [ ] Design Patterns

## Sistemas Distribuídos

- [ ] Monolith
- [ ] Modular Monolith
- [ ] Microservices
- [ ] Event-Driven Architecture
- [ ] Message Brokers
- [ ] Distributed Transactions
- [ ] Eventual Consistency

## Padrões avançados

- [ ] CQRS
- [ ] Event Sourcing
- [ ] Saga Pattern
- [ ] Outbox Pattern
- [ ] Idempotency

---

# 24. Observabilidade

- [ ] Structured Logging
- [ ] Log Levels
- [ ] Metrics
- [ ] Tracing
- [ ] Health Checks
- [ ] Error Tracking
- [ ] Monitoring

## Ferramentas

- [ ] Sentry
- [ ] Prometheus
- [ ] Grafana
- [ ] OpenTelemetry

---

# 25. Tecnologias para estudar posteriormente

Estas tecnologias são relevantes, mas **não devem bloquear a entrada no mercado**:

- [ ] Kubernetes
- [ ] Terraform
- [ ] Kafka
- [ ] GraphQL
- [ ] gRPC
- [ ] Elasticsearch
- [ ] Advanced AWS
- [ ] Advanced React
- [ ] Next.js
- [ ] Service Mesh

---

# 26. Projetos do Portfólio

## Projeto 1 — REST API

### Stack

```text
Node.js
TypeScript
Express
PostgreSQL
Prisma
Jest
Docker
```

### Funcionalidades

- [ ] CRUD
- [ ] Relacionamentos
- [ ] Validação
- [ ] Paginação
- [ ] Filtros
- [ ] Ordenação
- [ ] Tratamento de erros
- [ ] Testes
- [ ] Docker

---

# Projeto 2 — Sistema Completo

Escolher um domínio realista:

- [ ] Sistema de Biblioteca
- [ ] Sistema Financeiro
- [ ] Sistema de Pedidos
- [ ] Sistema de Estoque
- [ ] Sistema de Chamados

### Requisitos

- [ ] Authentication
- [ ] Authorization
- [ ] Roles
- [ ] PostgreSQL
- [ ] Prisma
- [ ] REST API
- [ ] Validation
- [ ] Transactions
- [ ] Pagination
- [ ] Filtering
- [ ] Tests
- [ ] Docker
- [ ] Documentation

---

# Projeto 3 — Sistema Assíncrono

### Arquitetura

```text
                ┌──────────────┐
                │   Frontend   │
                └──────┬───────┘
                       │
                       ▼
                ┌──────────────┐
                │      API     │
                └──────┬───────┘
                       │
              ┌────────┴────────┐
              ▼                 ▼
        PostgreSQL            Redis
                                │
                                ▼
                             Queue
                                │
                                ▼
                             Worker
                                │
                    ┌───────────┴───────────┐
                    ▼                       ▼
               Database              External API
```

### Requisitos

- [ ] REST API
- [ ] PostgreSQL
- [ ] Redis
- [ ] Queue
- [ ] Worker
- [ ] Retry
- [ ] Idempotência
- [ ] Authentication
- [ ] Tests
- [ ] Docker
- [ ] Logging

---

# Projeto 4 — Full Stack

### Frontend

```text
React
TypeScript
```

### Backend

```text
NestJS
TypeScript
PostgreSQL
Prisma
Redis
```

### Infraestrutura

```text
Docker
GitHub Actions
AWS
```

### Funcionalidades

- [ ] Authentication
- [ ] Authorization
- [ ] Dashboard
- [ ] CRUD
- [ ] Search
- [ ] Filtering
- [ ] Pagination
- [ ] Upload
- [ ] Notifications
- [ ] Background Jobs
- [ ] Tests
- [ ] CI/CD
- [ ] Deploy

---

# 27. Marco para buscar estágio/júnior

Ao atingir este ponto, **não é necessário terminar o roadmap** para começar a procurar oportunidades.

## Backend Junior Ready

- [ ] HTML
- [ ] CSS
- [ ] JavaScript
- [ ] DOM
- [ ] Fetch
- [ ] HTTP
- [ ] TypeScript
- [ ] Node.js
- [ ] Express
- [ ] REST API
- [ ] PostgreSQL
- [ ] SQL
- [ ] Prisma
- [ ] Authentication
- [ ] Authorization
- [ ] Git/GitHub
- [ ] Jest
- [ ] Docker

### Portfólio

- [ ] 2–3 projetos completos
- [ ] README bem documentado
- [ ] API documentada
- [ ] Testes
- [ ] Docker
- [ ] GitHub organizado
- [ ] Projetos publicados/deployados

---

# 28. Evolução profissional

```text
Fundamentos
     ↓
Frontend básico
     ↓
JavaScript
     ↓
TypeScript
     ↓
Node.js
     ↓
REST APIs
     ↓
PostgreSQL
     ↓
Prisma
     ↓
Authentication
     ↓
NestJS
     ↓
Testing
     ↓
Docker
     ↓
Redis
     ↓
Queues
     ↓
AWS
     ↓
CI/CD
     ↓
Architecture
     ↓
Observability
     ↓
Distributed Systems
     ↓
Microservices
```

---

# Stack-alvo

## Linguagem

```text
JavaScript
TypeScript
```

## Backend

```text
Node.js
Express
NestJS
```

## Database

```text
PostgreSQL
Redis
```

## ORM

```text
Prisma
```

## Frontend

```text
HTML
CSS
JavaScript
React
```

## Testing

```text
Jest
Supertest
```

## DevOps

```text
Git
GitHub
Docker
GitHub Actions
```

## Cloud

```text
AWS
```

## Arquitetura

```text
REST
Clean Architecture
SOLID
DDD
Event-Driven Architecture
Microservices
```

## Mensageria

```text
BullMQ
RabbitMQ
Kafka
```

## Observabilidade

```text
Sentry
Prometheus
Grafana
OpenTelemetry
```

---

# Princípio da trilha

> **Aprender primeiro aquilo que permite construir sistemas; depois aquilo que permite construir sistemas melhores; por último aquilo que permite construir sistemas grandes.**

A prioridade é:

```text
CONSTRUIR
   ↓
ENTENDER
   ↓
TESTAR
   ↓
DEPLOYAR
   ↓
OTIMIZAR
   ↓
ESCALAR
   ↓
ARQUITETAR
```

Isso evita transformar o estudo em uma coleção de tecnologias e mantém o foco no objetivo principal: **tornar-se um desenvolvedor Backend Web capaz de construir, testar, publicar e manter aplicações reais.**
