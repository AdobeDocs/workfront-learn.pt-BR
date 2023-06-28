---
title: Apresentação dos armazenamentos de dados
description: Saiba como usar um armazenamento de dados para sincronizar nomes de empresas entre uma lista de empresas e a Workfront usando [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Apresentação dos armazenamentos de dados

Neste exercício, estamos usando um armazenamento de dados para sincronizar nomes de empresas entre uma lista de empresas e a Workfront.

Essa é uma parte de uma sincronização unidirecional de empresas no Workfront e em algum outro sistema. Por enquanto, ela só será sincronizada entre um arquivo CSV e o Workfront. Mas ela também manterá uma tabela em um armazenamento de dados que rastreará a Workfront ID (WFID) e a ID da empresa no arquivo CSV (CID) para cada empresa. Isso nos permitirá fazer dessa uma sincronização bidirecional em algum ponto no futuro.

![Uma imagem de um cenário do Fusion](assets/data-structures-and-data-stores-2.png)

## Apresentação dos armazenamentos de dados

A Workfront recomenda assistir ao vídeo de apresentação do exercício antes de tentar recriá-lo em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on)

>[!TIP]
>
>Para obter instruções passo a passo sobre como concluir a apresentação, acesse o [Apresentação dos armazenamentos de dados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) exercício.


## Nota final

Agora que você terminou de aprender sobre estruturas de dados e armazenamentos de dados, você pode estar se perguntando: &quot;Quando você deve usá-los?&quot;

As estruturas de dados são usadas com mais frequência para serializar ou analisar formatos de dados, como JSON, XML, CSV e outros. As estruturas de dados permitem controlar a estrutura dos dados e até mesmo validá-los. O motivo mais comum para usar uma estrutura de dados é criar dados válidos para enviar a uma API que espera JSON ou XML. Nesses casos, é desejável usar o aplicativo JSON ou XML junto com a estrutura de dados para garantir que os dados estejam no formato correto.

Os armazenamentos de dados devem ser usados apenas para armazenar dados persistentes que precisam ser acessados por mais de uma execução de cenário. Por exemplo, você pode armazenar metadados sobre o último registro processado para casos de uso avançados que exigem controle preciso sobre o processamento.

Os armazenamentos de dados não foram projetados para serem usados como data warehouse ou registro. Os armazenamentos de dados não estão acessíveis fora do Workfront Fusion e a maioria das interações com os armazenamentos de dados ocorre por meio de um cenário do Workfront Fusion. Consequentemente, não é possível conectar um armazenamento de dados a uma ferramenta de análise ou relatório que seria esperada para casos de uso de data warehouse e log. O papel do Workfront Fusion em casos de uso como esses seria preencher um sistema apropriado para organizar e armazenar dados (por exemplo, SQL, MariaDB).

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
