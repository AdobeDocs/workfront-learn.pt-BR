---
title: Entenda como navegar e revisar projetos no [!UICONTROL Análise aprimorada]
description: Saiba como ler o gráfico Plano de voo no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 335047.png
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8729
exl-id: 1409a1af-3bdb-40f7-af01-f9de2357b602
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Entenda como navegar e revisar projetos no [!UICONTROL Análise aprimorada]

Neste vídeo, você aprenderá:

* Como ler o plano de voo

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12&learn=on)

## Plano de voo

![Uma imagem de um gráfico de plano de voo com números correspondentes a marcadores abaixo](assets/section-2-1.png)

No gráfico, você vê:

1. Os nomes dos projetos estão à esquerda.
1. As datas são mostradas na parte inferior.
1. A linha azul vertical mostra a data específica em que o mouse está passando o mouse.
1. As linhas azuis horizontais mostram as datas de início e término planejadas do projeto.
1. As linhas verdes indicam que o projeto está no Target.
1. Linhas laranja indicam que o projeto está em risco.
1. As linhas vermelhas indicam que o projeto está em problemas.

Ver essas informações sobre seus projetos ajuda a determinar:

* Quais eventos estendem um projeto após a data de conclusão planejada.
* Quando um projeto começa a enfrentar problemas.
* Quantos projetos estão abertos no mesmo período de tempo.
* Quantos projetos estão ativos.
* Quais projetos necessitam de mais atenção ou apoio.

## A condição é baseada no status do progresso

A condição do projeto é uma representação visual de como o projeto está progredindo. O Workfront determina a condição com base no status do progresso das tarefas no projeto.

![Uma imagem dos status de progresso possíveis](assets/section-2-2.png)

A condição de um projeto pode ser definida:

* **Manualmente**, por usuários com acesso para gerenciar o projeto, quando o tipo de condição do projeto é definido como manual. Isso permite que você defina a condição do projeto independentemente do caminho crítico.
* **Automaticamente**, por Workfront, quando o tipo de condição do projeto é definido como Status de progresso.

A Workfront recomenda que você defina o tipo de condição como Status de progresso para ter uma indicação clara do progresso real do projeto, com base no progresso de suas tarefas.

![Uma imagem dos status de progresso possíveis](assets/section-2-3.png)

Nesse caso, a condição do projeto pode ser:

* **No Target**—Quando o status do progresso da última tarefa no caminho crítico for Em Tempo, a condição do projeto será No Target. O projeto está no caminho para terminar de acordo com a programação.
* **Em Risco**—Quando o status do progresso da última tarefa no caminho crítico estiver Atrás ou Em Risco, a condição do projeto será Em Risco. O projeto está no caminho para terminar tarde, mas ainda não está atrasado.
* **Em problemas**—Quando o status do progresso da última tarefa no caminho crítico for Late, a condição do projeto será Em Problemas. A data de vencimento está no passado e o projeto está agora atrasado.

>[!NOTE]
>
>As condições podem ser personalizadas para seu ambiente, portanto, você pode encontrar mais de três opções ou os nomes podem ser diferentes dos acima. Para obter informações sobre como personalizar condições, consulte o artigo Criar ou editar uma condição personalizada.
