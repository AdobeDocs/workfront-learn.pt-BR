---
title: Tutorial sobre roteadores
description: Aprenda a usar um roteador para encaminhar pacotes de “Pokémon vs. super-heróis” pelo caminho correto no  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Tutorial sobre roteadores

Use um roteador para transferir pacotes de “Pokémon vs. super-heróis” pelo caminho correto e, em seguida, crie uma tarefa para cada personagem.

![Uma imagem do cenário do Fusion](assets/universal-connectors-and-routing-2.png)

## Tutorial sobre roteadores

O Workfront recomenda assistir ao tutorial em vídeo antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12&learn=on)

## URLs de exercício

* Site da API Superhero: `https://www.superheroapi.com/`
* Primeiro URL do exercício: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* Segundo URL do exercício: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

Se tiver problemas para acessar o seu próprio token de super-herói, você pode usar este token compartilhado: 10110256647253588. Leve em consideração quantas vezes você chama o “Superhero API”, para que esse token compartilhado continue funcionando para todos.



## Pesquisar itens no painel de mapeamento

O campo Pesquisar itens na parte superior dos painéis de mapeamento ajuda a localizar rapidamente os campos no painel, mesmo que estejam aninhados em matrizes. A pesquisa não diferencia maiúsculas de minúsculas.

![Uma imagem do primeiro painel de pesquisa](assets/universal-connectors-and-routing-3.png)

![Uma imagem do segundo painel de pesquisa](assets/universal-connectors-and-routing-4.png)

## Dicas e truques para trabalhar com APIs

Até este ponto, você trabalhou com uma API (Application Programming Interface) muito simples que não requer autenticação adicional para obter as informações necessárias no cenário. Veja algumas dicas para ajudar você a trabalhar com APIs e conectores universais.

## Etapa 1: determine o tipo de API

O Workfront e muitos sistemas de software são criados usando uma API REST (Representational State Transfer), que atualmente é o tipo de API mais fácil e tradicional disponível. No entanto, existem algumas outras, como:

* SOAP (Simple Object Access Protocol) (a API de prova do Workfront é baseada em SOAP)
* FTP (File Transfer Protocol)
* SFTP (Secure File Transfer Protocol)
* Para saber mais, faça uma pesquisa na web por tipos de API e palavras-chave do seu interesse.

>[!NOTE]
>
>Ao conectar-se a plataformas maiores, como o Salesforce, diferentes áreas dessas plataformas fornecerão APIs diferentes. Certifique-se de encontrar a certa para o serviço ao qual deseja se conectar.

## Etapa 2: determine o tipo de autenticação exigido pela API

A autenticação de API é uma forma de identificação usada para controlar o acesso a um serviço, como quando você tenta se conectar através do Workfront Fusion. Ela ajuda a provar para outro sistema que você está autorizado a acessá-lo. O OAuth 2 é o tipo de autenticação mais comum usado atualmente. Pesquise na Internet para saber mais sobre autenticação de API.

A autenticação pode ser o aspecto mais difícil do trabalho com uma API. Um dos recursos mais valiosos dos conectores universais do Workfront Fusion é que ele pode lidar com a autenticação se você utilizar métodos de autenticação comuns, como autenticação básica, OAuth 2, chave de API e outros. Depois de criar uma conexão usando o módulo apropriado para o método de autenticação (por exemplo, OAuth 2), o Workfront Fusion gerará chaves de API e/ou tokens sempre que você quiser executar o cenário.

Saiba mais sobre os diferentes tipos de autenticação que o Workfront fornece no artigo Visão geral da autenticação aprimorada na Experience League.

## Etapa 3: leia a documentação da API e encontre os pontos de acesso necessários

Quando uma API interage com outro sistema, os pontos de contato dessa comunicação são considerados pontos de acesso. Um ponto de acesso é o local onde as APIs enviam solicitações e onde o recurso reside.

Ao interagir com uma API usando um conector universal, você precisa entender quais pontos de acesso são compatíveis com a API e quais dados são necessários para cada solicitação. A documentação da API deve descrever os pontos de acesso de uma API e como realizar operações comuns como criar, ler, atualizar ou excluir. A execução dessas chamadas exige um pouco de prática, principalmente se você estiver iniciando agora com as chamadas de API ou o trabalho com uma nova API.

Saiba mais sobre os conectores universais do Workfront Fusion e como configurá-los para se conectar às APIs necessárias na Experience League.

## Observação final

Você pode conferir a lista completa dos conectores de aplicativos pré-construídos na Experience League. Se quiser sugerir um novo conector de aplicativo para a equipe de produto do Workfront Fusion, envie sua ideia para o Laboratório de inovação. Se você não enviou nada ainda, saiba mais sobre o Laboratório de inovação e descubra como votar em ideias e participar da priorização do Placar de líderes, que é realizada duas vezes por ano. Se você já tiver acesso ao Laboratório de inovação, faça logon e envie suas ideias.

## Sua vez

>[!NOTE]
>
>Os exercícios práticos e desafios são opcionais e não são necessários para concluir o treinamento do Fusion.

Este exercício prático baseia-se no que você aprendeu no tutorial, mas a solução não é fornecida.

No módulo Definir múltiplas variáveis para personagens Pokémon, crie uma variável chamada “Atributo (Nível)”. Mapeie o nome dos atributos do Pokémon nesta variável. Use o recurso de valor da matriz para alterar a forma como a matriz é exibida, de modo que cada Atributo seja uma nova linha, conforme mostrado abaixo.

**Dica:** existem apenas seis atributos diferentes de Pokémon com um nível correspondente.

![Uma imagem dos Atributos](assets/universal-connectors-and-routing-5.png)

**Desafio:** tente usar as fórmulas de matriz para fazer com que as Habilidades sejam exibidas de maneira semalhante ao exemplo acima, como linhas diferentes em vez de uma sequência de valores separados por vírgula. Há uma dica na captura de tela abaixo.

![Uma imagem de um nome de matriz](assets/universal-connectors-and-routing-6.png)

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=br)
