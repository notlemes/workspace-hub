# PRD — Workspace Hub

## 1. Identificação

**Projeto:** Workspace Hub  
**Tema:** Plataforma de gerenciamento e reserva de espaços de trabalho  
**Autor:** João Pedro Lemes  
**Disciplina:** Desenvolvimento de Página Web com CSS e Framework  
**Instituição:** Universidade Tecnológica Federal do Paraná (UTFPR)

---

## 2. Descrição do Projeto

O Workspace Hub é uma aplicação web para facilitar a consulta, organização e reserva de espaços de trabalho compartilhados.

A plataforma permitirá que usuários consultem os espaços disponíveis, visualizem suas características, verifiquem informações sobre disponibilidade e realizem reservas de acordo com suas necessidades.

O sistema poderá ser utilizado em ambientes como coworkings, universidades, empresas e outros locais que disponibilizem salas de reunião, estações de trabalho ou espaços compartilhados.

O principal problema que o sistema busca resolver é a dificuldade de organizar e controlar a utilização de espaços compartilhados, centralizando informações sobre os espaços, seus recursos e as reservas realizadas.

---

## 3. Objetivos

### Objetivo geral

Desenvolver uma aplicação web que permita consultar e gerenciar espaços de trabalho e suas respectivas reservas.

### Objetivos específicos

- Permitir o cadastro e acesso de usuários.
- Apresentar os espaços disponíveis.
- Exibir informações detalhadas sobre cada espaço.
- Permitir a realização de reservas.
- Permitir a consulta das reservas realizadas.
- Permitir o cancelamento de reservas.
- Organizar informações sobre os recursos disponíveis em cada espaço.
- Facilitar a administração dos espaços cadastrados.

---

## 4. Atores do Sistema

### Visitante

Usuário que acessa a aplicação sem estar autenticado.

Pode:

- Visualizar informações gerais sobre o Workspace Hub.
- Consultar os espaços disponíveis.
- Visualizar características dos espaços.
- Acessar as páginas de login e cadastro.

### Usuário autenticado

Usuário cadastrado e autenticado na aplicação.

Pode:

- Consultar espaços.
- Visualizar detalhes dos espaços.
- Verificar disponibilidade.
- Realizar reservas.
- Consultar suas reservas.
- Cancelar suas reservas.
- Atualizar seus dados pessoais.

### Administrador

Usuário responsável pelo gerenciamento da plataforma.

Pode:

- Cadastrar espaços.
- Editar informações dos espaços.
- Remover espaços.
- Cadastrar e gerenciar recursos.
- Consultar usuários.
- Consultar e gerenciar reservas.

---

## 5. Histórias de Usuário

### Acesso e cadastro

- **US01:** Como Visitante, eu quero visualizar a página inicial do sistema para que eu possa conhecer a proposta do Workspace Hub.

- **US02:** Como Visitante, eu quero criar uma conta informando meus dados pessoais para que eu possa utilizar os recursos de reserva.

- **US03:** Como Usuário, eu quero realizar login utilizando meu e-mail e senha para que eu possa acessar minha conta.

- **US04:** Como Usuário, eu quero atualizar meus dados pessoais para que minhas informações permaneçam corretas.

### Consulta de espaços

- **US05:** Como Visitante, eu quero visualizar os espaços disponíveis para que eu possa conhecer as opções oferecidas.

- **US06:** Como Usuário, eu quero visualizar os detalhes de um espaço para que eu possa verificar sua capacidade, localização e recursos.

- **US07:** Como Usuário, eu quero filtrar os espaços por características para que eu possa encontrar um espaço adequado às minhas necessidades.

- **US08:** Como Usuário, eu quero consultar a disponibilidade de um espaço em determinada data e horário para que eu possa verificar se posso realizar uma reserva.

### Reservas

- **US09:** Como Usuário, eu quero realizar uma reserva informando o espaço, a data e o horário para que eu possa utilizar o espaço desejado.

- **US10:** Como Usuário, eu quero visualizar minhas reservas para que eu possa acompanhar os espaços que reservei.

- **US11:** Como Usuário, eu quero cancelar uma reserva para que o horário possa ficar novamente disponível.

- **US12:** Como Usuário, eu quero receber uma confirmação da reserva para que eu possa ter certeza de que a solicitação foi registrada.

### Administração

- **US13:** Como Administrador, eu quero cadastrar um novo espaço informando suas características para que ele fique disponível para os usuários.

- **US14:** Como Administrador, eu quero editar as informações de um espaço para que os dados apresentados estejam atualizados.

- **US15:** Como Administrador, eu quero remover um espaço para que espaços que não estão mais disponíveis não sejam apresentados para reserva.

- **US16:** Como Administrador, eu quero cadastrar recursos de um espaço para que os usuários saibam quais equipamentos estão disponíveis.

- **US17:** Como Administrador, eu quero consultar as reservas realizadas para que eu possa acompanhar a utilização dos espaços.

---

## 6. Regras de Negócio

### RN01 — Cadastro de usuário

Cada usuário deve possuir um identificador único e um endereço de e-mail válido.

### RN02 — Autenticação

Somente usuários cadastrados e autenticados podem realizar reservas.

### RN03 — Reserva

Uma reserva deve estar associada a um único usuário e a um único espaço.

### RN04 — Disponibilidade

Um espaço não pode possuir duas reservas para o mesmo período de data e horário.

### RN05 — Dados da reserva

Toda reserva deve possuir data, horário de início, horário de término, usuário, espaço e status.

### RN06 — Cancelamento

O usuário pode cancelar uma reserva realizada por ele.

### RN07 — Espaços

Cada espaço deve possuir informações como nome, descrição, tipo, capacidade e localização.

### RN08 — Recursos

Um espaço pode possuir diversos recursos, como projetor, monitor, quadro branco, tomadas ou outros equipamentos.

### RN09 — Administração

Somente administradores podem cadastrar, editar ou remover espaços e recursos.

---

## 7. Escopo Inicial

O escopo inicial do Workspace Hub contempla:

- Página inicial.
- Cadastro de usuário.
- Login.
- Consulta de espaços.
- Página de detalhes de um espaço.
- Consulta de disponibilidade.
- Cadastro de reservas.
- Listagem das reservas do usuário.
- Cancelamento de reservas.
- Perfil do usuário.
- Área administrativa básica para gerenciamento de espaços e recursos.
