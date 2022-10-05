---
title: Apresentação dos Data Stores
description: Saiba como usar o em um armazenamento de dados para sincronizar nomes de empresas entre uma lista de empresas e a Workfront usando [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Apresentação dos armazenamentos de dados

## Visão geral

Neste exercício, estamos usando um armazenamento de dados para sincronizar nomes de empresas entre uma lista de empresas e a Workfront.

Essa é uma parte de uma sincronização unidirecional de empresas no Workfront e em algum outro sistema. Por enquanto, ele só sincronizará entre um arquivo CSV e o Workfront. Mas também manterá uma tabela em um armazenamento de dados que acompanhará a Workfront ID (WFID) e a ID da empresa no arquivo CSV (CID) de cada empresa. Isto permitir-nos-á tornar esta situação numa sincronização bidirecional num futuro próximo.

![Uma imagem de um cenário de Fusão](assets/data-structures-and-data-stores-2.png)

## Apresentação dos armazenamentos de dados

A Workfront recomenda assistir ao vídeo de apresentação de exercícios antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>Para obter instruções passo a passo sobre como concluir a apresentação, acesse o [Apresentação dos armazenamentos de dados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) exercício.


## Nota final

Agora que você terminou de aprender sobre estruturas de dados e armazenamentos de dados, você pode estar se perguntando, &quot;Quando você deve usá-los?&quot;

As estruturas de dados são usadas mais frequentemente para serializar ou analisar formatos de dados, como JSON, XML, CSV e outros. As estruturas de dados oferecem a capacidade de controlar a estrutura de seus dados e até mesmo validar os dados. O motivo mais comum para usar uma estrutura de dados é criar dados válidos para enviar a uma API que espera JSON ou XML. Nesses casos, você deverá usar o aplicativo JSON ou XML juntamente com sua estrutura de dados para garantir que os dados estejam no formato correto.

Os armazenamentos de dados devem ser usados apenas para armazenar dados persistentes que precisam ser acessados por mais de uma execução de cenário. Por exemplo, você pode armazenar metadados sobre o último registro processado para casos de uso avançados que exigem controle preciso sobre o processamento.

Os armazenamentos de dados não são projetados para serem usados como data warehouse ou registro. Os armazenamentos de dados não são acessíveis fora do Workfront Fusion e a maioria das interações com armazenamentos de dados é por meio de um cenário do Workfront Fusion. Consequentemente, não é possível conectar um armazenamento de dados a uma ferramenta de análise ou relatório que seria esperada para casos de uso de data warehouse e log. A função do Workfront Fusion em casos de uso como esses seria preencher um sistema apropriado para organizar e armazenar dados (por exemplo, SQL, MariaDB).

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
