---
title: Entender como navegar e revisar projetos no [!UICONTROL Analítica aprimorada]
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
source-git-commit: 65bd26fefb280d12ec44a4923f6d96ac8d88d6fb
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Entender como navegar e revisar projetos no [!UICONTROL Analítica aprimorada]

Neste vídeo, você aprenderá:

* Como ler o gráfico Plano de voo

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12&learn=on)

## Gráfico de plano de voo

![Imagem de um gráfico de plano de voo com números correspondentes aos marcadores abaixo](assets/section-2-1.png)

No gráfico, você vê:

1. Os nomes dos projetos estão à esquerda.
1. As datas são exibidas na parte inferior.
1. A linha azul vertical mostra a data específica em que seu mouse está passando.
1. As linhas azuis horizontais mostram as datas planejadas de início e término do projeto.
1. As linhas verdes indicam que o projeto está no destino.
1. As linhas em laranja indicam que o projeto está em risco.
1. As linhas vermelhas indicam que o projeto está com problemas.

Ver essas informações sobre os projetos ajuda a determinar:

* Quais eventos estendem um projeto além da data planejada de conclusão.
* Quando um projeto começa a ter problemas.
* Quantos projetos estão abertos no mesmo período de tempo.
* Quantos projetos estão ativos.
* Quais projetos precisam de mais atenção ou suporte.

## A condição é baseada no status do progresso

A condição do projeto é uma representação visual de como o projeto está progredindo. O Workfront determina a condição com base no status do progresso das tarefas no projeto.

![Uma imagem dos status de progresso possíveis](assets/section-2-2.png)

A condição de um projeto pode ser definida:

* **Manualmente**, por usuários com acesso para gerenciar o projeto, quando o tipo de condição do projeto for definido como manual. Isso permite que você defina a condição do projeto independentemente do caminho crítico.
* **Automaticamente**, da Workfront, quando o tipo de condição do projeto é definido como Status de progresso.

A Workfront recomenda definir o tipo de condição como Status de progresso para que você tenha uma indicação clara do progresso real do projeto, com base no progresso de suas tarefas.

![Uma imagem dos status de progresso possíveis](assets/section-2-3.png)

Quando definida como Status de progresso, a condição do projeto pode ser:

* **No Destino**—Quando o status de progresso da última tarefa no caminho crítico for No Prazo, a condição do projeto será No Prazo. O projeto está no caminho certo para terminar no prazo.
* **Em Risco**— Quando o status do progresso da última tarefa no caminho crítico é Atrás ou Em Risco, a condição do projeto é Em Risco. O projeto está no bom caminho para terminar atrasado, mas ainda não está atrasado.
* **Com Problemas**—Quando o status de progresso da última tarefa no caminho crítico é Late, a condição do projeto é In Trouble. A data de conclusão está no passado e o projeto está atrasado.

>[!NOTE]
>
>As condições podem ser personalizadas para seu ambiente, portanto, você pode encontrar mais de três opções ou os nomes podem ser diferentes dos acima. Para obter informações sobre como personalizar condições, consulte o artigo [Criar ou editar uma Condição personalizada](https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-conditions/create-edit-custom-conditions.html?lang=en).
