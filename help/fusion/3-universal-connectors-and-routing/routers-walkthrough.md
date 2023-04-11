---
title: Apresentação de roteadores
description: Saiba como usar um roteador para passar pacotes Pokemon vs. super-heróis pelo caminho correto em [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
doc-type: video
source-git-commit: 57b112921738c01fe4222e50403c8953c412a0f7
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Apresentação de roteadores

Use um roteador para passar Pokemon vs. super-heróis para baixo no caminho correto e crie uma tarefa para cada caractere.

![Uma imagem do cenário de Fusão](assets/universal-connectors-and-routing-2.png)

## Apresentação de roteadores

A Workfront recomenda assistir ao vídeo de apresentação de exercícios antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12&learn=on)

## URLs de exercício

* Site da API do Superhero: `https://www.superheroapi.com/`
* Primeiro URL para exercício: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* Segundo URL de exercício: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

Se tiver problemas para acessar seu próprio token de super-herói, você pode usar este token compartilhado: 10110256647253588. Considere quantas vezes você chama a API de super-herói para que esse token compartilhado continue a funcionar para todos.

>[!TIP]
>
>Para obter instruções passo a passo sobre como concluir a apresentação, acesse o [Apresentação de roteadores](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) exercício.


## Pesquisar itens no painel de mapeamento

O campo Pesquisar itens na parte superior dos painéis de mapeamento ajuda você a encontrar rapidamente os campos no painel, mesmo que eles estejam aninhados em arrays. A pesquisa não diferencia maiúsculas de minúsculas.

![Uma imagem do primeiro painel de pesquisa](assets/universal-connectors-and-routing-3.png)

![Uma imagem do segundo painel de pesquisa](assets/universal-connectors-and-routing-4.png)

## Dicas e truques para trabalhar com APIs

Até esse ponto, você trabalhou com uma API muito simples (Application Programming Interface) que não requer autenticação extra para obter as informações necessárias no cenário. Estas são algumas dicas para ajudá-lo a navegar trabalhando com APIs e conectores universais.

## Etapa 1: Determine o tipo de API

A Workfront e muitos sistemas de software são criados usando uma REST (Representational State Transfer) API, que é o tipo mais fácil e padrão de API atualmente. No entanto, há algumas outras, como:

* SOAP (Simple Object Access Protocol) (A API de Prova da Workfront é baseada em SOAP)
* FTP (Protocolo de transferência de arquivos)
* SFTP (Protocolo de transferência segura de arquivo)
* Para saber mais, faça uma pesquisa na Web por tipos de API e palavras-chave de interesse.

>[!NOTE]
>
>Ao se conectar a plataformas maiores, como o Salesforce, diferentes áreas dessas plataformas fornecerão APIs diferentes. Certifique-se de encontrar o serviço correto ao qual deseja se conectar.

## Etapa 2: Determine o tipo de autenticação exigido pela API

Autenticação de API é uma forma de identificação usada para controlar o acesso a um serviço, como quando você tenta se conectar por meio do Workfront Fusion. Ele ajuda você a provar para outro sistema que está autorizado a acessar o sistema. O OAuth 2 é o tipo de autenticação mais comum usado atualmente. Saiba mais com uma pesquisa na Internet sobre autenticação de API.

A autenticação pode ser o aspecto mais difícil de trabalhar com uma API. Um dos recursos mais valiosos dos conectores universais do Workfront Fusion é que o Workfront Fusion pode manipular a autenticação para você ao usar métodos de autenticação comuns, como autenticação básica, como OAuth 2, Chave da API e outros. Depois de criar uma conexão usando o módulo Workfront Fusion apropriado para o método de autenticação (por exemplo, OAuth 2), o Workfront Fusion gerará continuamente chaves de API e/ou tokens sempre que você quiser executar seu cenário.

Saiba mais sobre os diferentes tipos de autenticação que a Workfront fornece no artigo de visão geral sobre autenticação aprimorada no Experience League.

## Etapa 3: Leia a documentação da API e localize os endpoints necessários

Quando uma API interage com outro sistema, os pontos de contato dessa comunicação são considerados pontos finais. Um endpoint é o local onde as APIs enviam solicitações e onde o recurso está.

Ao interagir com uma API usando um conector universal, é necessário entender quais endpoints a API suporta e quais dados são necessários para cada solicitação. A documentação da API deve descrever os endpoints de uma API e como executar operações comuns, como criar, ler, atualizar ou excluir. A execução dessas chamadas requer alguma prática, especialmente se você for novo em fazer chamadas de API ou trabalhar com uma nova API.

Saiba mais sobre os Workfront Fusion Universal Connectors e como configurá-los para se conectar às APIs necessárias no Experience League.

## Nota final

Você pode verificar a lista inteira de nossos conectores de aplicativo pré-criados no Experience League. Caso deseje sugerir um novo conector de aplicativo para a equipe de produtos do Workfront Fusion, envie sua ideia para o Laboratório de Inovação. Se você não tiver apresentado antes, saiba mais sobre o Laboratório de Inovação, além de como pode votar em ideias e participar da priorização duas vezes por ano do Quadro de Liderança. Se você já tiver acesso ao Laboratório de Inovação, faça logon e envie suas ideias.

## Sua vez

>[!NOTE]
>
>Os exercícios práticos e os desafios são opcionais e não são necessários para concluir a formação em Fusão.

Este exercício de prática baseia-se no que você aprendeu na apresentação, mas a solução não é fornecida.

No módulo Definir várias variáveis para caracteres Pokemon, crie uma variável chamada &quot;Stat (Level)&quot;. Mapeie o nome das Estatísticas do Pokemon para essa variável. Use o recurso de valor de matriz para alterar a forma como a matriz é exibida, de modo que cada Estado seja uma nova linha, como mostrado abaixo.

**Dica:** Há apenas seis estatísticas Pokemon diferentes com um nível correspondente.

![Uma imagem de Estatísticas](assets/universal-connectors-and-routing-5.png)

**Desafio:** Veja se você pode usar as fórmulas de matriz para fazer com que as capacidades sejam exibidas da mesma maneira que as linhas diferentes acima, em vez de uma sequência de valores separados por vírgula. Há uma dica na captura de tela abaixo.

![Uma imagem de um nome de matriz](assets/universal-connectors-and-routing-6.png)

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
