# 1 Meu Ecommerce

`/1 Meu Ecommerce`

* [Overview](/docs/README.md)
  * [**1 Meu Ecommerce**](/docs/1%20Meu%20Ecommerce/README.md)
  * [Omnichannel](/docs/Omnichannel/README.md)

---

[Overview (up)](/docs/README.md)

---

![diagram](https://www.plantuml.com/plantuml/svg/0/hLNBRjj65DqRy3zCjP81IKJZP9DL58bstCYY4iaDiZAko14rDJd3paEAK_HZWYu25EYoNw0Vwxr3YgJaHxkejR0qSyyvzyN3DyQ2jYxFs3LtB8nLddCTyzEJ7uICCvTmjhQsCA-3GCDsa0gxTajdC4H9owKT8220H0kGcymLBXYzxCyoaFRcUX9aOBcnU7GxmcWGakj1WL98dl0L_cJZyEUhKJIT_mSHwmhKEGyAOaUIli3R_WeZ-gRG0fM278pbEaZuXkvC8tCHJHV3J-4ykWx_LoL_1bjkLCxxhrezszSLW4nT1dNP3-v_WGqSNxQo3IWtKmMSdao6dwERnUsdgyMxsqbu6Kx7tJCwds6Gabrd76YXUgnpOzpk6txjqFUSkUfdZua4gnGh4KEYc79CxlvGx5V76SJS662AyVqA30ZizJjUP7wFDUUtuHVR1MVNU3bqr3Fasdqdcef4iUvxVXzd2kxEY68k20TUXTgiLGOCFuVWH9awJODKATTSne8ogbZXEBUz2gNNIgw052ylSVUsSC-mdpD88KSjrSu6pulwl2RegbmAZ8hmNxm6ANb685pV3TVfxa-V4K9Za20CbfDZVlkq6V_occtNO0qKFOOY8kinasCrDXuS9RdIu9B3T78bXLMw5F3ttBHGRvMJ2UZxhbWQ11uyhPqpzjlf2SE_-a7hcW8ylqmptmBEXaMHOR-jK9AAejKpiHQ5xR5gJUbuw8FAeQmqBJYNYU_tFkZiM0eAuO62edv2sXxxW9juvuo75G9RhO66RrnEesw8zuay93MM5dbkLNp7vbpZ8yqVfMzr47Uc796VAfsW_IZSkwTLLWvdrBbmsKfaX7fUYkvstpqphfTCH2qquud05NvIQBpi9aky78E59HZFFrF6fffxq53dy9LBO4Ak57x7_l_DJRk4HnbV755UAvcgyTld6OigrqSPpuyOFsBmSndwoRO7Ygo_arryv5bZIEKo_jWVxbscMLqyVxTOpEQboH3A1vSxzOBrAJ_ZCeiJ1ZA9Il2YBTYWIcEQpoCsYIwlfjucmi-ZIJHylm_qpENSpzlqoFbm3IgC3oytykK196ocqs8lsrY7_Nl7Qerof4yWczcXGSRa559jg2NDG7qdA4-_RK_pL5j5dcqTPEAhj_wc6EBnHbCPOYWtNgvyTvGy1ucNhZjQ0pwAQUEzHTjxwpaJoWFsDbWdsdgQBoeBzC1P0wmmfGrEgunOeOpP_RNXwCejxwJuieBctLYMWaaPD4LPpyErNfcrYUCxmB8jNteVxo7862xHPYfxF-XKjNjrAHjiAwuifrgikaCfeeuABg_6vRwymUbNR_RJaty0)

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


