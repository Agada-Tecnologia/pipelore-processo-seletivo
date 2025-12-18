# Desafio Técnico - Desenvolvedor(a) Full Stack Next.js - Pipelore

## 🎯 Objetivo

O objetivo deste desafio é conhecer suas habilidades e entender como você resolve problemas. Procure atender aos requisitos funcionais e técnicos de forma que você possa demonstrar suas competências e todo o seu potencial.

## 📋 Descrição do Desafio

O Pipelore é um sistema de gestão de condomínios que permite aos condomínios gerenciar suas ordens de serviço de reparo.

Implemente um **cadastro de ordem de serviço de reparo** seguindo os padrões e a arquitetura do Next.js.

### Modelo de Dados

Crie uma ordem de serviço de reparo com os seguintes campos:

**Campos obrigatórios:**
- `title` (string, máx. 255 caracteres) - Título do reparo
- `description` (text) - Descrição detalhada do problema
- `location` (string) - Local do reparo (ex.: "Torre A - Apto 101", "Área comum - Piscina")
- `priority` (enum) - Prioridade: LOW, MEDIUM, HIGH, URGENT
- `status` (enum) - Status: OPEN, IN_PROGRESS, COMPLETED, CANCELLED
- `dueDate` (date) - Data prevista para conclusão
- `completedAt` (timestamp) - Data de conclusão
- `createdAt` (timestamp) - Data de criação
- `updatedAt` (timestamp) - Data de atualização

Não se preocupe em implementar uma conexão com o banco de dados, você pode usar mocks para simular as operações de leitura e escrita. Porém, se desejar, pode implementar uma conexão com o banco de dados usando SQLite ou outro banco de dados de sua preferência, bem como qualquer biblioteca de ORM (Drizzle ORM, Prisma, etc.) que você preferir.

## 🛠️ Requisitos Técnicos

### Stack obrigatória
- Next.js 15+ (App Router)
- React 19+
- TypeScript 5+

### Arquitetura

Sinta-se à vontade para implementar a arquitetura que desejar, mas recomendamos seguir as [boas práticas de desenvolvimento e arquitetura do Next.js](https://nextjs.org/docs/app/getting-started/project-structure) e do React.

## 📝 Requisitos Funcionais

### Frontend - Interface

**Listagem:**
- Tabela/cards com todas as ordens de serviço
- Filtros por status

**Cadastro:**
- Formulário com campos para cadastro de ordem de serviço

**Ações:**
- Botão "Nova Ordem"
- Editar ordem
- Deletar ordem (com confirmação)

### Backend - API REST

Implemente o seguinte endpoint, usada para simular uma integração com um sistema externo:

#### GET `/api/repair-orders/late`
- Listar todas as ordens de serviço com data prevista para conclusão já passada, ou seja, ordens de serviço atrasadas
- Esse endpoint deve retornar um array de ordens

## 🚀 Entrega

### Formato

- Repositório no seu GitHub
- **README.md** com instruções de setup e informações sobre o projeto

## 💡 Dicas

- Implemente testes unitários ou de integração se você se sentir confortável.
- Docker ou Docker Compose podem ser uma boa ideia para facilitar a execução.
- O envio de dados pode ser feito com **Server Actions**; especialmente para formulários, isso pode ser mais simples do que criar endpoints REST.
- Prefira usar **Server Components** em vez de **Client Components**. Use componentes de cliente apenas quando necessário (principalmente em partes interativas).
- **Não reinvente a roda**: use as ferramentas disponíveis e as bibliotecas que você preferir (Zod, React Hook Form, etc.).
- Nós encorajamos o uso de **IA** para auxiliar no desenvolvimento e nas decisões técnicas. Não copie e cole cegamente: entenda o que está sendo feito e encontre a solução por conta própria com o auxílio da IA.
- **Pergunte**: se tiver dúvidas, pode perguntar (simulando um ambiente real).

## 📞 Contato

Em caso de dúvidas técnicas sobre o desafio:
- Email: [email-tecnico]
- Horário: 24/7

**Boa sorte! 🚀**

Estamos ansiosos para ver sua solução e discutir suas decisões técnicas na próxima etapa.
