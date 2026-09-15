# workspace-hub

# workspace-hub

**Autor** - João Pedro Lemes.

**Disciplina** - Desenvolvimento de Página Web com CSS e Framework.

**Instituição** - UTFPR.

**Projeto:** O **Workspace Hub** é uma plataforma web para consulta, gerenciamento e reserva de espaços de trabalho compartilhados.

O sistema tem como objetivo facilitar a busca por espaços disponíveis, permitindo que usuários visualizem informações sobre salas e ambientes de trabalho, consultem sua disponibilidade e realizem reservas.

O projeto utilizará tecnologias como **JavaScript, Bootstrap, jQuery, Sass, JSON Server e APIs públicas**, além de protótipos desenvolvidos utilizando o **Figma**.

# Tecnologias e Dependências

## 🔧 Bootstrap

Framework CSS utilizado para criação de interfaces responsivas e reutilização de componentes.

Será utilizado na construção dos layouts do Workspace Hub, permitindo que a aplicação seja adaptável para diferentes tamanhos de tela, como celulares, tablets e desktops.

Entre os componentes utilizados estarão:

- Navbar;
- Cards;
- Buttons;
- Forms;
- Modal;
- Alerts;
- Grid;
- Carousel.

## 🎨 Sass (SCSS)

Pré-processador CSS utilizado para organização e modularização dos estilos da aplicação.

Será utilizado para criação de variáveis, organização dos estilos e desenvolvimento de um Design System consistente para o Workspace Hub.

## 📚 JavaScript

Linguagem utilizada para implementar a lógica da aplicação e controlar a interatividade das páginas.

Será utilizada para:

- Manipulação dos dados;
- Validação de formulários;
- Controle das reservas;
- Requisições assíncronas;
- Integração com APIs;
- Manipulação do Web Storage;
- Atualização dinâmica dos elementos da página.

## 🧩 jQuery

Biblioteca JavaScript utilizada para facilitar a manipulação do DOM, tratamento de eventos e interações com os elementos da aplicação.

Será utilizada principalmente nos formulários e nos componentes interativos do Workspace Hub.

## 🎭 jQuery Mask Plugin

Plugin utilizado para aplicação de máscaras em campos de formulário.

Será utilizado para facilitar o preenchimento de informações como:

- CEP;
- Telefone.

## 🔢 UUID

Biblioteca utilizada para geração de identificadores únicos.

Será utilizada para identificar registros como:

- Usuários;
- Espaços;
- Reservas.

## 🗄️ JSON Server

Ferramenta utilizada para criação de uma API fake para o projeto.

O JSON Server será utilizado para simular o backend da aplicação e permitir o armazenamento e consulta dos dados do sistema.

Os principais recursos da API serão:

- Usuários;
- Espaços;
- Reservas;
- Recursos dos espaços.

Exemplos de operações:

- GET — consultar dados;
- POST — cadastrar dados;
- PATCH — atualizar dados;
- DELETE — remover dados.

## 📍 ViaCEP

API pública utilizada para consulta de endereços através do CEP.

No cadastro do usuário, o sistema poderá realizar uma consulta à API e preencher automaticamente informações como:

- Logradouro;
- Bairro;
- Cidade;
- Estado.

A utilização da ViaCEP também permite demonstrar a realização de requisições assíncronas para uma API pública real.

## 🎨 Figma

Ferramenta utilizada para criação dos protótipos da aplicação.

Serão desenvolvidos protótipos para diferentes tamanhos de tela, contemplando principalmente:

- Mobile;
- Desktop.

O protótipo será utilizado como referência para implementação da interface do Workspace Hub.

## 🧹 ESLint

Ferramenta utilizada para análise do código JavaScript.

O ESLint ajudará a identificar possíveis problemas e manter boas práticas durante o desenvolvimento da aplicação.

## ✨ Prettier

Formatador de código utilizado para manter um padrão de organização e formatação dos arquivos do projeto.

## 🚀 GitHub Pages

Serviço utilizado para publicação da aplicação web.

A aplicação poderá ser disponibilizada online através do GitHub Pages.

# Funcionalidades

O Workspace Hub contará inicialmente com as seguintes funcionalidades:

- Cadastro de usuários;
- Login de usuários;
- Consulta de espaços de trabalho;
- Visualização dos detalhes dos espaços;
- Consulta de disponibilidade;
- Realização de reservas;
- Cancelamento de reservas;
- Consulta das reservas realizadas;
- Cadastro de espaços;
- Gerenciamento de espaços;
- Cadastro de recursos dos espaços;
- Consulta de endereço através do CEP;
- Validação de formulários;
- Armazenamento de informações no Web Storage.

# Modelo de dados

O sistema será organizado inicialmente pelas seguintes entidades:

- Usuário;
- Espaço;
- Reserva;
- Recurso.

## Usuário

Representa as pessoas que utilizam o sistema.

Principais informações:

- ID;
- Nome;
- E-mail;
- Senha;
- Telefone;
- CEP;
- Endereço;
- Tipo de usuário.

## Espaço

Representa os espaços disponíveis para utilização.

Principais informações:

- ID;
- Nome;
- Descrição;
- Capacidade;
- Localização;
- Tipo de espaço;
- Status.

## Reserva

Representa uma reserva realizada por um usuário.

Principais informações:

- ID;
- Usuário;
- Espaço;
- Data;
- Horário inicial;
- Horário final;
- Status.

## Recurso

Representa os recursos disponíveis em cada espaço.

Exemplos:

- Wi-Fi;
- Projetor;
- Monitor;
- Ar-condicionado;
- Quadro branco;
- Tomadas.

# Relacionamentos

Um usuário pode realizar várias reservas.

Um espaço pode possuir várias reservas em diferentes períodos.

Um espaço pode possuir vários recursos.

Uma reserva pertence a um único usuário e a um único espaço.

# 📖 Checklist | Indicadores de Desempenho (ID) dos Resultados de Aprendizagem (RA)

## RA1 - Utilizar Frameworks CSS para estilização de elementos HTML e criação de layouts responsivos

- [ ] **ID 01 - Prototipa interfaces** adaptáveis para no mínimo os tamanhos de **tela mobile e desktop**, utilizando Figma.
- [ ] **ID 02 - Implementa layout responsivo** com **Framework CSS**, utilizando Bootstrap e seu sistema de Grid.
- [ ] **ID 03 - Implementa layout responsivo** com **CSS puro**, utilizando Flexbox ou Grid Layout.
- [ ] **ID 04 - Utiliza componentes prontos** de um Framework CSS, como cards, buttons, navbar, modal e carousel.
- [ ] **ID 05 - Cria layout fluido** utilizando unidades relativas como %, vw, vh, em e rem.
- [ ] **ID 06 - Aplica um Design System consistente**, utilizando cores, tipografia e padrões de componentes.
- [ ] **ID 07 - Utiliza Sass (SCSS)** com variáveis e organização modular dos estilos.
- [ ] **ID 08 - Aplica tipografia responsiva**, utilizando media queries e/ou a função clamp().
- [ ] **ID 09 - Aplica técnicas de responsividade de imagens** utilizando CSS e object-fit.
- [ ] **ID 10 - Otimiza imagens** utilizando formatos modernos como WebP e técnicas como srcset ou picture.

## RA2 - Realizar tratamento de formulários e aplicar validações customizadas no lado cliente

- [ ] **ID 11 - Implementa validação HTML nativa**, utilizando campos obrigatórios, tipos e limites de caracteres.
- [ ] **ID 12 - Aplica expressões regulares (REGEX)** para validações customizadas.
- [ ] **ID 13 - Utiliza elementos de seleção em formulários**, como checkbox, radio e select.
- [ ] **ID 14 - Implementa leitura e escrita no Web Storage**, utilizando localStorage e/ou sessionStorage.

## RA3 - Aplicar ferramentas para otimização do processo de desenvolvimento web

- [x] **ID 15 - Configura ambiente com Node.js e NPM** para gerenciamento de pacotes e dependências.
- [x] **ID 16 - Utiliza boas práticas de versionamento** no Git/GitHub, utilizando a branch main.
- [ ] **ID 17 - Mantém um README.md padronizado**, conforme template da disciplina, com checklist preenchido.
- [ ] **ID 18 - Organiza arquivos do projeto de forma modular**, seguindo uma estrutura organizada.
- [ ] **ID 19 - Configura linters e formatadores**, utilizando ESLint e Prettier.

## RA4 - Aplicar bibliotecas de funções e componentes em JavaScript para aprimorar a interatividade de páginas web

- [ ] **ID 20 - Utiliza jQuery** para manipulação do DOM e interatividade.
- [ ] **ID 21 - Integra e configura um plugin jQuery**, utilizando o jQuery Mask Plugin.

## RA5 - Efetuar requisições assíncronas para uma API fake e APIs públicas, permitindo a obtenção e manipulação de dados dinamicamente

- [ ] **ID 22 - Realiza requisições assíncronas para uma API fake**, utilizando JSON Server para persistir dados de formulários.
- [ ] **ID 23 - Realiza requisições assíncronas para uma API fake** para exibir dados dinamicamente na página.
- [ ] **ID 24 - Realiza requisições assíncronas para uma API pública real**, utilizando a API ViaCEP para consulta de endereços e tratamento de erros.

# Estrutura inicial do projeto

A estrutura inicial planejada para o projeto será:

```text
workspace-hub/
│
├── index.html
├── README.md
├── package.json
├── package-lock.json
├── .gitignore
├── db.json
│
├── docs/
│   ├── prd.md
│   └── architecture.md
│
├── src/
│   ├── css/
│   │   ├── main.scss
│   │   └── components/
│   │
│   ├── js/
│   │   ├── main.js
│   │   ├── api.js
│   │   ├── reservas.js
│   │   ├── usuarios.js
│   │   └── validacao.js
│   │
│   └── pages/
│       ├── login.html
│       ├── cadastro.html
│       ├── espacos.html
│       ├── reservas.html
│       └── perfil.html
│
└── assets/
    ├── images/
    └── icons/# workspace-hub

Checklist da Atividade 06
 - [x]Configurei minha identidade no Git
 - [x] Clonei o repositório do meu projeto
 Inicializei o NPM (package.json)
 Criei o .gitignore ignorando node_modules e .env
 Instalei Bootstrap como dependência de produção
 Instalei jQuery como dependência de produção
 Instalei UUID como dependência de produção
 Instalei JSON Server
 Instalei jQuery Mask Plugin
 Instalei Sass
 Instalei ESLint
 Instalei Prettier
 Instalei gh-pages como dependência de desenvolvimento
 Criei a estrutura inicial do projeto
 Criei o arquivo db.json
 Criei os arquivos prd.md e architecture.md
 Fiz commit e push para a branch main
```
