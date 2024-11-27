# Teste para Desenvolvedor(a) Back-End PHP

## Introdução

Bem-vindo(a) ao processo seletivo para a posição de **Desenvolvedor(a) Back-End** em nossa equipe! Este teste tem como objetivo avaliar suas habilidades técnicas em PHP 8+, Slim Framework, e outras tecnologias mencionadas na descrição da vaga.

## Instruções

- Faça um **fork** deste repositório para o seu GitHub pessoal.
- Desenvolva as soluções solicitadas abaixo, seguindo as **melhores práticas de desenvolvimento**.
- Após a conclusão, envie o link do seu repositório para avaliação.
- Sinta-se à vontade para adicionar qualquer documentação ou comentários que julgar necessário.

## Desafio

### Contexto

Você foi designado para desenvolver uma API RESTful para um sistema de gerenciamento de tarefas. O sistema deve permitir que usuários:

- Criem, visualizem, atualizem e excluam tarefas.
- Cada tarefa deve conter: título, descrição, status (pendente, em andamento, concluída) e data de criação.
- O sistema deve suportar múltiplos usuários, cada um com suas próprias tarefas.

### Requisitos

1. **Configuração do Ambiente**

   - Configure um ambiente de desenvolvimento utilizando **Docker** e **Docker-compose**, incluindo:
     - Servidor web (Nginx ou Apache).
     - PHP na versão 7.4 ou superior.
     - Banco de dados MongoDB e/ou SQL Server (você pode escolher qual utilizar).
     - Redis.
   - Certifique-se de que a aplicação possa ser iniciada com um único comando (`docker-compose up`).

2. **Autenticação e Autorização**

   - Implemente um sistema de autenticação de usuários utilizando **Laravel Sanctum** ou **JWT**.
   - Proteja as rotas da API para que somente usuários autenticados possam acessá-las.

3. **CRUD de Tarefas**

   - Implemente as operações CRUD (Create, Read, Update, Delete) para as tarefas seguindo os princípios **RESTful**.
   - Utilize **Eloquent ORM** para manipulação dos dados.
   - Assegure-se de que um usuário só possa acessar suas próprias tarefas.

4. **Cache com Redis**

   - Implemente o cache das listagens de tarefas utilizando **Redis** para melhorar a performance.
   - Garanta que o cache seja invalidado ou atualizado quando houver alterações nas tarefas (criação, atualização ou exclusão).

5. **Boas Práticas de Código**

   - Aplique os princípios de **Clean Code** em toda a sua implementação.
   - Utilize **PSR-12** como padrão de codificação.
   - Documente o código quando necessário para melhorar a legibilidade.

6. **Logs**

   - Implemente o registro de logs para operações críticas, como:
     - Falhas de autenticação.
     - Erros no servidor.
     - Acesso não autorizado a recursos.

7. **Documentação da API**

   - Forneça uma documentação da API utilizando **Swagger/OpenAPI** ou uma coleção do **Postman**.
   - A documentação deve estar acessível através de uma rota, por exemplo, `/docs`.

### Diferenciais (Desejável)

- **MongoDB**

  - Implemente uma funcionalidade onde determinadas informações das tarefas sejam armazenadas em um banco de dados **MongoDB**.

- **Microserviços**

  - Estruture a aplicação considerando uma arquitetura de **microserviços**, separando, por exemplo, a parte de autenticação em um serviço próprio.

- **Comunicação em Tempo Real**

  - Implemente notificações em tempo real quando uma nova tarefa for criada utilizando **WebSockets** (por exemplo, com **Laravel Echo** e **Pusher**).

## Entrega

- O código deve estar disponível em um repositório Git (preferencialmente GitHub) público.
- Inclua um arquivo `README.md` com:
  - Instruções claras sobre como configurar e executar a aplicação.
  - Descrição das funcionalidades implementadas.
  - Possíveis limitações ou melhorias futuras.

## Avaliação

Os seguintes aspectos serão considerados na avaliação:

- **Funcionalidade**: se a aplicação atende aos requisitos propostos.
- **Qualidade do Código**: organização, legibilidade e aderência às boas práticas.
- **Uso das Tecnologias**: implementação correta e eficaz das ferramentas solicitadas.
- **Boas Práticas**: aplicação de princípios de Clean Code e padrões de projeto.
- **Documentação**: clareza das instruções e documentação fornecidas.
- **Testes**: qualidade e abrangência dos testes implementados.
- **Histórico de Commits**: uso adequado do Git com commits bem descritos.

## Observações

- Caso não seja possível implementar todos os requisitos, explique as razões e descreva como você abordaria a solução.
- Sinta-se à vontade para adicionar funcionalidades extras que julgar relevantes.
- Demonstre criatividade e inovação em sua solução.

---

Boa sorte! Estamos ansiosos para conhecer o seu trabalho e potencial.
