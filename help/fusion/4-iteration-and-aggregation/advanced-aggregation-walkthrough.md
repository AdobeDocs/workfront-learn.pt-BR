---
title: Tutorial sobre agregação avançada
description: Aprenda como chamar um serviço da web para retornar detalhes sobre vários países e identificar a população, agrupada por sub-região, sem sair do [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
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
autotag-review: '2026-05-06T16:33:27.197Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 91%

---

# Tutorial sobre agregação avançada

Chame um serviço da web para retornar detalhes sobre vários países e identificar a população total de todos os países, agrupada por sub-região.

![Uma imagem do cenário do Fusion](assets/iteration-and-aggregation-3.png)

## Tutorial sobre agregação avançada

O Workfront recomenda assistir ao tutorial em vídeo antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops=1)

## URLs de exercício

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## Reforço do princípio de agregação

Sempre que um módulo gera vários pacotes configuráveis, cada módulo posterior executará cada um dos pacotes.

Para evitar isso, adicione um agregador após um módulo que possa gerar vários pacotes configuráveis.

Você verá uma sombra ao redor dos segmentos do cenário, desde o **iterador inicial** até o **agregador final**. Isso ajuda a facilitar a localização desses segmentos no cenário do Workfront Fusion.

## Sua vez

>[!NOTE]
>
>Os exercícios práticos e desafios são opcionais e não são necessários para concluir o treinamento do Fusion.

Este exercício prático baseia-se no que você aprendeu no tutorial, mas a solução não é fornecida.

Crie um novo cenário para somar todas as horas registradas em tarefas nos projetos do portfólio de marketing. Em seguida, envie um email dizendo &quot;A equipe do projeto {Project Name} registrou {summed hours} do total de {planned hours} horas planejadas, colocando você em {percentage} do plano.&quot;

**Desafio:** tente fazer o mesmo, mas apenas para as horas registradas neste ano.

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
