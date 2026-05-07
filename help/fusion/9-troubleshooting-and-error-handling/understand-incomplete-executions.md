---
title: Entenda sobre execuções incompletas
description: Saiba o que são execuções incompletas e como lidar com um erro que resulta em uma execução incompleta no  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
recommendations: noDisplay,catalog
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:07:51.152Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 100%

---

# Entenda sobre execuções incompletas

Execuções incompletas podem ser armazenadas no Workfront Fusion, onde podem ser revisadas e resolvidas posteriormente. Saiba como utilizar esse recurso incrível.

Neste vídeo, você aprenderá:

* O que são execuções incompletas
* Como lidar com um erro que resulta em uma execução incompleta

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on&enablevpops=1)

## Erros que resultam em execuções incompletas

Há várias categorias de erros que resultam no armazenamento de execuções incompletas.

Os diferentes tipos de erros recebidos dependerão das APIs às quais você está se conectando. Ele pode ser um erro de validação resultante de dados incompletos ou incorretos, principalmente devido à ausência de um item esperado para processar com êxito todos os dados que passam por um módulo. Ou os erros podem ocorrer devido à indisponibilidade do destino final devido a uma falha temporária ou de longo prazo na conexão (por exemplo, durante a conexão com o servidor de email ou FTP remoto).

Se ocorrer um erro no primeiro módulo do cenário, a execução será interrompida imediatamente e nenhuma execução incompleta será armazenada.

Se o erro ocorrer em qualquer outro módulo e não houver nenhuma rota do manipulador de erros anexada, então:

* Se o erro for do tipo ConnectionError, RateLimitError, OutOfSpaceError ou ModuleTimeoutError, um registro de execução incompleto COM repetição automática será armazenado.
* Se o erro for do tipo DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError ou MaxResultsExceededError, um registro de execução incompleta SEM repetição automática será armazenado.
* Se o tipo de erro for diferente dos mencionados acima, a execução falhará.

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
