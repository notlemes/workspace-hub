# Architecture — Workspace Hub

## 1. Visão Geral

O Workspace Hub será desenvolvido como uma aplicação web para consulta, gerenciamento e reserva de espaços de trabalho compartilhados.

A aplicação será estruturada de forma modular, separando os arquivos de interface, estilos, scripts e documentação.

Durante o desenvolvimento da disciplina, a aplicação utilizará tecnologias front-end e APIs para simular o armazenamento e o acesso aos dados.

---

## 2. Arquitetura Inicial

A aplicação será organizada em três partes principais:

### Interface

Responsável pela apresentação das páginas e componentes da aplicação.

Tecnologias previstas:

- HTML5
- CSS3
- Bootstrap
- Sass/SCSS

### Lógica da aplicação

Responsável pela interação com o usuário, validação dos formulários, manipulação do DOM e comunicação com APIs.

Tecnologias previstas:

- JavaScript
- jQuery
- jQuery Mask Plugin

### Dados e APIs

Responsável pelo armazenamento e consulta dos dados da aplicação.

Tecnologias previstas:

- JSON Server
- API pública ViaCEP
- Web Storage

---

## 3. Modelo de Dados

O sistema será composto inicialmente pelas seguintes entidades:

- Usuário
- Espaço
- Reserva
- Recurso

### Diagrama Entidade-Relacionamento

```mermaid
erDiagram

    USUARIO ||--o{ RESERVA : realiza
    ESPACO ||--o{ RESERVA : recebe
    ESPACO ||--o{ RECURSO : possui

    USUARIO {
        string id PK
        string nome
        string email
        string senha
        string telefone
        string cep
        string endereco
        string numero
        string complemento
        string cidade
        string estado
        string perfil
    }

    ESPACO {
        string id PK
        string nome
        string descricao
        string tipo
        int capacidade
        string localizacao
        string imagem
        boolean disponivel
    }

    RESERVA {
        string id PK
        string usuario_id FK
        string espaco_id FK
        string data
        string hora_inicio
        string hora_fim
        string status
    }

    RECURSO {
        string id PK
        string espaco_id FK
        string nome
        string descricao
        int quantidade
    }
```
