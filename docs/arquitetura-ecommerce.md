# arquitetura-ecommerce

* [Overview](#Overview)
  * [1 Meu Ecommerce](#1-Meu-Ecommerce)
  * [Omnichannel](#Omnichannel)

---

## Overview

![diagram](https://www.plantuml.com/plantuml/svg/0/RLFBRjj03BmRy3-mFZc0QbrwoYb6AYH1xSIeRGGz6Qp4M8jAItKVVdnEqKE10Zts2_nZvKhoGqQXWxHBSZWpfEwiG-DyMS2KF2GfboMPbFgzTqgdXSy8SkSgUnl71hUZjNAv_-gjfB1sfDr82cBCZ4AzANpbu_iFxsS5QhUSJk827LadLwlxaBrpeqeQzNlztcJyvMMvMBq-BHvNa-GXUVuul0dtCpAMzT1RZqPn18EbzOSVyZa8toNuzXY1ogIxUbCfPWpiGHz-Cdpt19YIjGWCTDGo6WZsV6yTbSDmAL0ThG5xha8OGVIUwiB1iA_GNY9mgPKKlCWhpL5hAaAz2DoGMHz-wrJLA2bgL1O4IwWSQGFjRc6RexDOHI3zL161BIsGIozwh9AT6w9tkG2FVR1PP1v-1OMjFeRX9zgd1UEtcqlwmO0m6SC5WZpTuepjYOhqX3KPgldo4HN_RrjDgCArT7gGcMvn7oJES8sbuFELWTNflWlmPj1dtTIIjN9i6ilgEDb1lGcVgJYlGJkrfSKG3A5c2kSzQVoNkNSD3ynU7yUB-NWMpQVpA9cEdoP7Z0QrdMUYDy92SxDJujVVXiavyNeWPokxUOrF3Tx9YbDE7JqwCMtaIvxXPW3NzeMIDhiruRcb21LRU_Yp8Tco2-VkI6VjJzRl_GC0)

**Contexto do sistema**

Visão geral do sistema Meu Ecommerce

O Sistema terá 2 sistemas que serão desenvolvidos 
- Meu Ecommerce
- OmniChanel

Os sistemas em cinza são aplicações que já existem.
- Autenticação e Acesso 

Para controle de autenticação e acesso será usado o [keycloak](https://www.keycloak.org/)



## 1 Meu Ecommerce

`/1 Meu Ecommerce`

[Overview](#arquitetura-ecommerce)

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




## Omnichannel

`/Omnichannel`

[Overview](#arquitetura-ecommerce)

![diagram](https://www.plantuml.com/plantuml/svg/0/hLDBZjf04Dtx53siG0AyIBB9QWZZ6KOQFXf3hAnGOHVGYRlRqn-ZKPJ3H5dC2N82BfPgcryW2nPXGtVNUw_gLPLlZGLjdSZPM4ZUNuEKc0StNAQvov2jhItCnp3KiEckk5sxXJEeKoKjIjjDbGWXqnnacRl2XVttdKaEqiw6Js4E5esbftcVqC0bwcv1UOAR39TqOtVHvyV-U1HVaSEwWjAy2milJXeTJj7EaX0TKsXEYK81ng8EConzp1oot8z7qruInUDXz5yJLM-mGQC4TZuS6xPt5O9SkHpsdY_2Nw64izX9gQ4lpDJnuAdtPJoRpfF7wM3-53r4exjcAmWc152owOm3pLMRDMR6RN_IiU7FWhdTjSruHlRuagUGAQOSazjVYhquP92YCS0KG_8kg1FOzUGgTwCLnA_aL3Hza5w7w5YqntbOp7qO65L-VAV2Qjhyat8o0_tQLBHN1D-l5-QDrlU0qM-dlrc3b-UfLfIuvDitnP8rM0E5JxC_jZpbb6U4kU35mbIb3MEFFqKBl4GFoJxA5MhF6KPn78qUekTpvWON5qpod59ThC1SCGabhgYtbKo22qOsRQNo8mYUCJ_EQDTA-Y3ysdZuO3gTnBvh7bU7T_sAPCc1ZLGzkUtRzZTMtZGi5joA5o9vJeq-Ra5V2IU9m4YB9kjEbiANnHBlXlhJPicWDurxapOxSLv9LWCvLPGbBSIvOkrzyuz1LIBLTAuGKPgPUcZ-h-PMixgoW7jQueLIt_uUfZXSTfQywoiL3nCaO5fDCWXkKMRqBVu1)

**OmniChanel**

    Sistema responsável pela comunicação com o cliente em diversas plataformas externas.


O sistema é composto por 4 microserviços que recebem notificações do ecommerce por messageria [rabbitMq](https://www.rabbitmq.com/) e enviam ao cliente por uma das plataforma selecionadas pelo cliente.


