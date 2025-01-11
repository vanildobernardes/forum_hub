<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Fórum Hub API</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 20px;
            background-color: #f4f4f4;
            color: #333;
        }
        h1, h2 {
            color: #0056b3;
        }
        ul {
            list-style-type: none;
            padding-left: 0;
        }
        li {
            margin-bottom: 8px;
        }
        .section-title {
            margin-top: 30px;
            color: #333;
            font-size: 1.4em;
        }
        .tech-list, .func-list {
            padding-left: 20px;
        }
    </style>
</head>
<body>

    <h1>Fórum Hub API</h1>
    <p>Este projeto é uma API RESTful para o gerenciamento de tópicos e discussões, desenvolvida como parte de um desafio promovido pela Alura em parceria com o programa Oracle Next Education. O objetivo é fornecer uma solução robusta e escalável para a gestão de conteúdo em fóruns de discussão online.</p>

    <div class="section-title">
        <h2>🚀 Tecnologias Utilizadas</h2>
    </div>
    <ul class="tech-list">
        <li><strong>Linguagem:</strong> Java 17</li>
        <li><strong>Framework:</strong> Spring Boot (versão 3.3.5)</li>
        <li><strong>Banco de Dados:</strong> MySQL (gerenciado com Flyway para migrações)</li>
        <li><strong>Gerenciamento de Dependências:</strong> Maven</li>
        <li><strong>Validação e Segurança:</strong> Spring Validation e Spring Security</li>
        <li><strong>Autenticação:</strong> JWT (JSON Web Token)</li>
        <li><strong>Documentação:</strong> Gerada automaticamente com Springdoc OpenAPI</li>
    </ul>

    <div class="section-title">
        <h2>📦 Dependências Principais</h2>
    </div>
    <p>A configuração completa do projeto pode ser visualizada no arquivo <code>pom.xml</code>, com destaque para as seguintes dependências:</p>
    <ul class="tech-list">
        <li><strong>Spring Boot Starter Web:</strong> Para a criação e desenvolvimento de APIs REST.</li>
        <li><strong>Spring Boot Starter Data JPA:</strong> Para facilitar a manipulação de dados no banco de dados.</li>
        <li><strong>Spring Boot Starter Validation:</strong> Para validação de entradas de dados.</li>
        <li><strong>Spring Boot Starter Security:</strong> Para configuração de autenticação e controle de acesso.</li>
        <li><strong>Flyway:</strong> Para controle de versões e migração do banco de dados.</li>
        <li><strong>Lombok:</strong> Para reduzir o código boilerplate e facilitar a criação de modelos e getters/setters.</li>
        <li><strong>Springdoc OpenAPI:</strong> Para gerar a documentação interativa da API.</li>
        <li><strong>MySQL Connector:</strong> Para conexão com o banco de dados MySQL.</li>
    </ul>

    <div class="section-title">
        <h2>✨ Funcionalidades</h2>
    </div>
    <p>A API permite a realização das seguintes operações principais:</p>
    <ul class="func-list">
        <li><strong>Cadastro de Tópicos:</strong> Criação de novos tópicos com validação de unicidade para título e conteúdo da mensagem.</li>
        <li><strong>Listagem de Tópicos:</strong> Exibição de uma lista de tópicos registrados no sistema, com suporte a <em>paginações</em> e <em>ordenação</em>.</li>
        <li><strong>Detalhamento de Tópico:</strong> Visualização detalhada das informações de um tópico específico, identificando-o pelo seu <strong>ID</strong>.</li>
        <li><strong>Atualização e Exclusão:</strong> <strong>Atualização</strong> de tópicos existentes com novos dados. <strong>Exclusão lógica</strong>, onde os tópicos são marcados como inativos, sem removê-los fisicamente do banco de dados.</li>
        <li><strong>Autenticação JWT:</strong> A API garante que apenas usuários autenticados possam acessar os endpoints protegidos, utilizando <strong>tokens JWT</strong> para validação.</li>
    </ul>

    <div class="section-title">
        <h2>🛠️ Sugestão de Testes com Insomnia</h2>
    </div>
    <p>Para realizar os testes de integração da API, recomendamos o uso da ferramenta <strong>Insomnia</strong>, que permite simular as requisições para os endpoints. Para uma experiência mais eficiente:</p>
    <ul class="tech-list">
        <li>Configure as <strong>variáveis de ambiente</strong> para facilitar a execução dos testes.</li>
        <li>Utilize o <strong>token JWT</strong> gerado durante a autenticação para realizar as requisições nos endpoints protegidos.</li>
    </ul>

    <div class="section-title">
        <h2>📚 Documentação</h2>
    </div>
    <p>A documentação da API é gerada automaticamente com o Springdoc OpenAPI, proporcionando uma interface interativa para explorar os endpoints disponíveis, realizar testes e visualizar exemplos de requisições e respostas.</p>

</body>
</html>
