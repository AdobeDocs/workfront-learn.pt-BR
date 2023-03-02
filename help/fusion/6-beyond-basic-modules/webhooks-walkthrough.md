---
title: Apresentação dos Webhooks
description: Saiba como usar um webhook para criar um aplicativo para determinar se um cliente tem ou não idade suficiente para comprar álcool, tudo em [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Apresentação dos Webhooks

## Visão geral

Esse cenário cria um aplicativo da loja de conveniência para que possam determinar facilmente se um cliente tem idade suficiente para comprar álcool. O operador de caixa precisa apenas postar o nome e a data de nascimento do cliente E um token de cliente verificado para um URL que foi fornecido. Depois de inserido, isso acionará nosso cenário para calcular a resposta apropriada e retorná-la ao solicitante.

![Uma imagem usando o módulo de comutação](assets/beyond-basic-modules-5.png)

## Apresentação dos Webhooks

A Workfront recomenda assistir ao vídeo de apresentação do exercício antes de tentar recriá-lo em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>Para obter instruções passo a passo sobre como concluir a apresentação, acesse o [Apresentação dos Webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) exercício.

## Configuração do Postman

Para seguir o exercício de explicação passo a passo, é necessário baixar o aplicativo gratuito do Postman. Siga as etapas abaixo para navegar até a área direita do Postman para o exercício.

1. Crie um espaço de trabalho e abra-o.
1. Clique na guia New e crie uma nova coleção chamada Drinking Age.
1. Clique na guia Novo novamente e crie uma nova solicitação do GET GET chamada Data de nascimento.
1. Altere a ação de solicitação de GET para POST.
1. Vá para a área da subguia Corpo abaixo do campo URL do POST.
1. Escolha dados de formulário abaixo da subguia Autorização.
1. Crie três chaves para Name, Birthdate e clientToken.

![Uma imagem usando o módulo de comutação](assets/beyond-basic-modules-6.png)

## Sua vez

>[!NOTE]
>
>Exercícios práticos e desafios são opcionais e não são necessários para concluir o treinamento do Fusion.

Esse exercício de prática se baseia no que você aprendeu na apresentação, mas a solução não é fornecida.

Crie um webhook do Workfront que está aguardando novas atualizações criadas e registra a data, o nome da pessoa que fez a atualização e o que a atualização diz. Envie por email a si mesmo essas informações.

**Dica**: use o módulo acionador do Workfront Watch Events para criar seu webhook. Além disso, no Workfront, as atualizações são chamadas de notas.

**Desafio**: é possível localizar e adicionar o URL de onde a atualização foi feita para facilitar o acesso?


## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
