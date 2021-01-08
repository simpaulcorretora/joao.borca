# Teste para Engenheiro de Software Backend

A proposta deste teste é criar uma integração integrações com a API da marvel.

## Como fazer seu teste
   - Para realizar o teste faça um Fork da branch master com seu nome-sobrenome, por exemplo: "Paulo.Silva". Quando terminar faça um commit desta branch.

## Prazo para entrega
   Subimeter no git até 20/11 às 23:59h.

## Detalhes API Marvel
  - Acessar o site da API Marvel [Site da API](https://developer.marvel.com/documentation/getting_started)
  - Criar uma conta para obter as credencias para acessar a api Marvel
  - Uma vez gerada sua chave você usará as credencias para implementar os endpoints a seguir.
  - Detalhe no README.md as informações necessárias para que podamos avaliar seu teste.



## Especificação do projeto

  - Fazer setup de uma API restfull usando NodeJS. Pode utilizar algum framework caso desejar.
  - Implemente sua API seguindo as melhores metodologias e práticas de arquitetura e design patterns.
  - Utilize as libs que ache necessário na implementação do seu app.
  - Documentar em arquivo .md steps para execução do projeto.

## Primeiro exercício

  - Fazer setup do projeto da API rest.
  - Criar um endpoint para recuperar da api Marvel o personagem (characters) "Avengers" e todas suas publicações (comics).

## Segundo exercício

 - Inserir cada item (nó) do retorno do endpoint acima em uma fila chamada (Avengers) de forma sincrona usando RabbitMQ.

## Terceiro exercício

   - Criar um serviço para escutar a fila Avengers e processar os seus itens.
   - Persistir estas informações em collections (nosql) ou tabelas (relacional).
      * Dados importantes personagem (id, name, description, modified, thumbnail).
      * Dados importantes comics (available, items[resourceURI, name])
   - Criar o MER das entidades

## Quarto exercício

   - Criar um endpoint que recupera do banco de dados o resourceURI de uma publicações (comic) de Avengers a partir do código = 77059 localizado na resourceURI.
   - Fazer um request para a url recuperada do banco. Deve retornar os detalhes da comigc = 77059.

## Quinto exercício

  - Criar um docker-compose para a app, database, filas e outros.

  ## Sexto exercício

  - Documentar a api no swagger.

## Sétimo exercício

  - Configurar um arquivo serverless.yml para fazer o deploy dos endpoints em um cloud (aws, azure ou google cloud) usando [serverless framework](https://www.serverless.com/framework/docs/).
