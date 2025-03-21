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
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '339'
ht-degree: 100%

---

# Tutorial sobre webhooks

Este cenário cria um aplicativo de loja de conveniência para determinar com facilidade se um(a) cliente tem ou não idade suficiente para comprar bebidas alcoólicas. O(a) operador(a) do caixa precisa apenas informar o nome e a data de nascimento do(a) cliente ALÉM DE um token de cliente verificado para uma URL fornecida. Depois de inserido, isso acionará o cenário para calcular a resposta apropriada e retorná-la ao solicitante.

![Uma imagem mostrando a utilização do módulo de comutação](assets/beyond-basic-modules-5.png)

## Tutorial sobre webhooks

O Workfront recomenda assistir ao tutorial em vídeo antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on&enablevpops)


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

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=br)
