---
title: Tutorial sobre webhooks
description: Aprenda a usar um webhook para criar um aplicativo para determinar se um(a) cliente tem ou não idade suficiente para comprar bebidas alcóolicas, sem sair do  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:29:34.923Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 100%

---

# Tutorial sobre webhooks

Este cenário cria um aplicativo de loja de conveniência para determinar com facilidade se um(a) cliente tem ou não idade suficiente para comprar bebidas alcoólicas. O(a) operador(a) do caixa precisa apenas informar o nome e a data de nascimento do(a) cliente ALÉM DE um token de cliente verificado para uma URL fornecida. Depois de inserido, isso acionará o cenário para calcular a resposta apropriada e retorná-la ao solicitante.

![Uma imagem mostrando a utilização do módulo de comutação](assets/beyond-basic-modules-5.png)

## Tutorial sobre webhooks

O Workfront recomenda assistir ao tutorial em vídeo antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on&enablevpops=1)


## Configuração do Postman

Para acompanhar o exercício do tutorial, você precisa baixar o aplicativo gratuito Postman. Siga as etapas abaixo para navegar até a área correta do Postman para o exercício.

1. Crie um espaço de trabalho e abra-o.
1. Clique na guia Novo e crie uma nova coleção chamada Idade para beber.
1. Clique na guia Novo novamente e crie uma nova solicitação GET chamada GET data de nascimento.
1. Altere a ação de solicitação de GET para POST.
1. Acesse a área da subguia Corpo abaixo do campo URL da solicitação POST.
1. Escolha dados de formulário abaixo da subguia Autorização.
1. Crie três chaves para Nome, Data de nascimento e Token de cliente.

![Uma imagem mostrando a utilização do módulo de comutação](assets/beyond-basic-modules-6.png)

## Sua vez

>[!NOTE]
>
>Os exercícios práticos e desafios são opcionais e não são necessários para concluir o treinamento do Fusion.

Este exercício prático baseia-se no que você aprendeu no tutorial, mas a solução não é fornecida.

Crie um webhook do Workfront que aguarde a criação de novas atualizações e, em seguida, registre a data, o nome da pessoa que fez a atualização e o conteúdo da atualização. Envie essas informações para o seu email.

**Dica**: use o módulo acionador Monitoramento de eventos do Workfront para criar seu webhook. Além disso, no Workfront, as atualizações são chamadas de notas.

**Desafio**: você consegue localizar e adicionar a URL do local em que a atualização foi feita para facilitar o acesso?


## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
