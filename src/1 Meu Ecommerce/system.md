**Level 2: Container diagram**

O sistema Meu Ecommerce é composto por 3 microserviços todos desenvolvidos com Java usando o framework [quarkus](https://quarkus.io/)

- Single Page Application

Aplicação de front-end desenvolvida com [angular](https://angular.io/).
Esta aplicação consome dados do serviço de Api.

- Api

Serviço responsável por prover os dados para o front-end.
Este Serviço busca os dados de um cache [redis](https://redis.io/).

- Fulfilment Service

Serviço responsavel pelo ciclo de compras dentro do ecommerce.
Este serviço tem um banco não relacional [mongodb](https://www.mongodb.com/)
Este serviço também chama um gateway de pagamento externo para finalizar os pedidos.

- Stock Service

Serviço responável pelo controle de estoque.
Este consome um banco relacional PostgreSql.


