---
title: Apresentação dos Webhooks
description: Saiba como usar um webhook para criar um aplicativo e determinar se um cliente é ou não velho o suficiente para comprar álcool, tudo em [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
source-git-commit: 96f963bf5a44eac234cbf9215f19f6dddbe23143
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Apresentação dos Webhooks

## Visão geral

Esse cenário cria um aplicativo da loja de conveniência para que possa determinar facilmente se um cliente é ou não velho o suficiente para comprar álcool. O caixa simplesmente precisa postar o nome e a data de nascimento do cliente E um token de cliente verificado para um URL que foi fornecido. Depois de inserido, o acionará o cenário para calcular a resposta apropriada e retorná-la ao solicitante.

![Uma imagem usando o módulo switch](assets/beyond-basic-modules-5.png)

## Apresentação dos Webhooks

A Workfront recomenda assistir ao vídeo de apresentação de exercícios antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>Para obter instruções passo a passo sobre como concluir a apresentação, acesse o [Apresentação dos Webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) exercício.

## Configuração do Postman

Para acompanhar o exercício de explicação passo a passo, é necessário baixar o aplicativo Postman gratuito. Siga as etapas abaixo para navegar até a área direita do Postman para o exercício.

1. Crie um espaço de trabalho e abra-o.
1. Clique na guia New e crie uma nova coleção chamada Drinking Age.
1. Clique na guia New novamente e crie uma nova solicitação de GET chamada GET data de nascimento.
1. Altere a ação de solicitação de GET para POST.
1. Vá para a área da subguia Body abaixo do campo POST URL .
1. Escolha os dados de formulário abaixo da subguia Autorização .
1. Crie três chaves para Nome, Birthdate e clientToken.

![Uma imagem usando o módulo switch](assets/beyond-basic-modules-6.png)

## Sua vez

>[!NOTE]
>
>Os exercícios práticos são opcionais e não são necessários para concluir a formação em Fusão.

Este exercício de prática baseia-se no que você aprendeu na apresentação, mas a solução não é fornecida.

Crie um webhook do Workfront que está aguardando novas atualizações criadas e, em seguida, registra a data, o nome da pessoa que fez a atualização e o que a atualização diz. Enviar essas informações por email para você mesmo.

**Dica**: Use o módulo acionador Eventos de observação do Workfront para criar seu webhook. Além disso, no Workfront, as atualizações são chamadas de notas.

**Desafio**: Você pode encontrar e adicionar o URL para onde a atualização foi feita para facilitar o acesso?


## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
