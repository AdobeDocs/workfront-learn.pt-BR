---
title: Passo a passo sobre armazenamentos de dados
description: Saiba como usar um armazenamento de dados para sincronizar nomes de empresas entre uma lista de empresas e o Workfront usando o [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:18:10.872Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 411
ht-degree: 100%

---

# Passo a passo sobre armazenamentos de dados

Neste exercício, estamos usando um armazenamento de dados para sincronizar nomes de empresas entre uma lista de empresas e o Workfront.

Isso faz parte de uma sincronização unidirecional de empresas no Workfront e algum outro sistema. Por enquanto, ele fará a sincronização apenas entre um arquivo CSV e o Workfront. Mas também manterá uma tabela num armazenamento de dados que acompanhará a ID do Workfront (WFID) e a ID da empresa no arquivo CSV (CID) de cada empresa. Isso nos permitirá tornar essa sincronização bidirecional em algum momento no futuro.

![Imagem de um cenário do Fusion](assets/data-structures-and-data-stores-2.png)

## Passo a passo sobre armazenamentos de dados

O Workfront recomenda assistir ao tutorial em vídeo antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on&enablevpops=1)



## Observação final

Agora que você terminou de aprender sobre estruturas de dados e armazenamentos de dados, você pode estar se perguntando: “Quando devo usá-los?”

As estruturas de dados são mais comumente usadas para serializar ou analisar formatos de dados como JSON, XML, CSV e outros. As estruturas de dados oferecem a capacidade de controlar a estrutura dos seus dados e até mesmo validá-los. O motivo mais comum para se usar uma estrutura de dados é criar dados válidos para enviar a uma API que espera JSON ou XML. Nesses casos, é desejável usar o aplicativo JSON ou XML com a estrutura de dados para garantir que os dados estejam no formato correto.

Os armazenamentos de dados só devem ser usados para armazenar dados persistentes que precisam ser acessados por mais de uma execução de cenário. Por exemplo, você pode armazenar metadados sobre o último registro processado para casos de uso avançados que exigem controle preciso sobre o processamento.

Os armazenamentos de dados não foram projetados para serem usados como data warehouse ou registro. Os armazenamentos de dados não são acessíveis fora do Workfront Fusion e a maioria das interações com armazenamentos de dados ocorre por meio de um cenário do Workfront Fusion. Consequentemente, não é possível conectar um armazenamento de dados a uma ferramenta de análise ou de relatórios que seria esperada para casos de uso de data warehouse e registro. A função do Workfront Fusion em casos de uso como esses seria preencher um sistema apropriado para organizar e armazenar dados (por exemplo, SQL, MariaDB).

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
