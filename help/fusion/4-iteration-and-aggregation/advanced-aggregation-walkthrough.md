---
title: Apresentação de agregação avançada
description: Saiba como chamar um serviço da Web para retornar detalhes sobre vários países e identificar a população, agrupada por sub-região, tudo em [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
source-git-commit: 0618bf27478744e0e9976015a24c5ec8519efbb7
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Apresentação de agregação avançada

## Visão geral

Chame um serviço da Web para retornar detalhes sobre vários países e identificar a população total de todos os países, agrupados por sub-região.

![Uma imagem do cenário de Fusão](assets/iteration-and-aggregation-3.png)

## Apresentação de agregação avançada

A Workfront recomenda assistir ao vídeo de apresentação de exercícios antes de tentar recriar o exercício em seu próprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## URLs de exercício

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>Para obter instruções passo a passo sobre como concluir a apresentação, acesse o [Apresentação de agregação avançada](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) exercício.

## Reforço do princípio da agregação

Sempre que um módulo gerar vários pacotes, cada módulo depois disso executará cada pacote.

Para evitar isso, adicione um agregador depois de um módulo que potencialmente produz vários pacotes.

Você verá uma sombra ao redor de qualquer segmento em seu cenário a partir de um **iterador inicial** para **agregador final**. Isso ajuda a facilitar a detecção desses segmentos no seu cenário do Workfront Fusion.

## Sua vez

>[!NOTE]
>
>Os exercícios práticos e os desafios são opcionais e não são necessários para concluir a formação em Fusão.

Este exercício de prática baseia-se no que você aprendeu na apresentação, mas a solução não é fornecida.

Crie um novo cenário para somar todas as horas logadas nas tarefas em projetos no portfólio de marketing. Em seguida, envie um e-mail que diga &quot;A equipe do projeto {Nome do Projeto} registrou {horas somadas} do total de {horas planejadas} horas planejadas, colocando-o em {percentagem} do plano.&quot;

**Desafio:** Veja se você pode fazer a mesma coisa, mas apenas por horas registradas este ano.

## Quer saber mais? Recomendamos o seguinte:

[Documentação do Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
