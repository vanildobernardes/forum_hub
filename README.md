# Fórum Hub API

Este projeto é uma API RESTful para o gerenciamento de tópicos e discussões, desenvolvido como parte de um desafio promovido pela Alura em parceria com o programa Oracle Next Education. O objetivo é fornecer uma solução robusta e escalável para a gestão de conteúdo em fóruns de discussão online.

## 🚀 Tecnologias Utilizadas

- **Linguagem**: Java 17
- **Framework**: Spring Boot (versão 3.3.5)
- **Banco de Dados**: MySQL (gerenciado com Flyway para migrações)
- **Gerenciamento de Dependências**: Maven
- **Validação e Segurança**: Spring Validation e Spring Security
- **Autenticação**: JWT (JSON Web Token)
- **Documentação**: Gerada automaticamente com Springdoc OpenAPI

## 📦 Dependências Principais

A configuração completa do projeto pode ser visualizada no arquivo `pom.xml`, com destaque para as seguintes dependências:

- **Spring Boot Starter Web**: Para a criação e desenvolvimento de APIs REST.
- **Spring Boot Starter Data JPA**: Para facilitar a manipulação de dados no banco de dados.
- **Spring Boot Starter Validation**: Para validação de entradas de dados.
- **Spring Boot Starter Security**: Para configuração de autenticação e controle de acesso.
- **Flyway**: Para controle de versões e migração do banco de dados.
- **Lombok**: Para reduzir o código boilerplate e facilitar a criação de modelos e getters/setters.
- **Springdoc OpenAPI**: Para gerar a documentação interativa da API.
- **MySQL Connector**: Para conexão com o banco de dados MySQL.

## ✨ Funcionalidades

A API permite a realização das seguintes operações principais:

- **Cadastro de Tópicos**: Criação de novos tópicos com validação de unicidade para título e conteúdo da mensagem.
- **Listagem de Tópicos**: Exibição de uma lista de tópicos registrados no sistema, com suporte a paginações e ordenação.
- **Detalhamento de Tópico**: Visualização detalhada das informações de um tópico específico, identificando-o pelo seu ID.
- **Atualização e Exclusão**: Atualização de tópicos existentes com novos dados. Exclusão lógica, onde os tópicos são marcados como inativos, sem removê-los fisicamente do banco de dados.
- **Autenticação JWT**: A API garante que apenas usuários autenticados possam acessar os endpoints protegidos, utilizando tokens JWT para validação.

## 🛠️ Sugestão de Testes com Insomnia

Para realizar os testes de integração da API, recomendamos o uso da ferramenta **Insomnia**, que permite simular as requisições para os endpoints. Para uma experiência mais eficiente:

- Configure as variáveis de ambiente para facilitar a execução dos testes.
- Utilize o token JWT gerado durante a autenticação para realizar as requisições nos endpoints protegidos.

## 📚 Documentação

A documentação da API é gerada automaticamente com o Springdoc OpenAPI, proporcionando uma interface interativa para explorar os endpoints disponíveis, realizar testes e visualizar exemplos de requisições e respostas.
