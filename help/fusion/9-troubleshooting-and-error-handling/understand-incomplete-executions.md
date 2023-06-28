---
title: Entender as execuções incompletas
description: Saiba o que são execuções incompletas e como lidar com um erro que resulta em uma execução incompleta no [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Entender as execuções incompletas

As execuções incompletas podem ser armazenadas no Workfront Fusion, onde podem ser revisadas e resolvidas posteriormente. Saiba como aproveitar esse recurso incrível.

Neste vídeo, você aprenderá:

* O que são execuções incompletas
* Como lidar com um erro que resulta em uma execução incompleta

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on)

## Erros que resultam em execuções incompletas

Há várias categorias de erros que resultam no armazenamento de execuções incompletas.

Tipos de erro diferentes recebidos dependerão das APIs às quais você está se conectando. O erro pode ser um erro de validação decorrente de dados incompletos ou errados, principalmente por causa de um item ausente esperado para processar com êxito todos os dados que passam por um módulo. Ou os erros podem ocorrer desde a indisponibilidade do destino final devido a uma falha temporária ou de longo prazo na conexão (por exemplo, durante a conexão com o servidor de email ou FTP remoto).

Se ocorrer um erro no primeiro módulo do cenário, a execução será interrompida imediatamente e nenhuma execução incompleta será armazenada.

Se ocorrer um erro em qualquer outro módulo e não houver nenhuma rota de manipulador de erros anexada, então:

* Se o tipo de erro for ConnectionError, RateLimitError, OutOfSpaceError ou ModuleTimeoutError, um registro de execução incompleto COM repetição automática será armazenado.
* Se o tipo de erro for DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError ou MaxResultsExceededError, um registro de execução incompleta SEM repetição automática será armazenado.
* Se o tipo de erro for qualquer coisa diferente da descrita acima, a execução falhará.

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
