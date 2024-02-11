---
title: Criar atividades básicas de filtro
description: Nesta atividade, você criará um filtro de projeto chamado "Projetos que possuo fechando este mês".
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 32%

---

# Criar atividades básicas de filtro

## Atividade 1 - Todos os projetos no portfólio de marketing

Nesta atividade, você criará um filtro de projeto chamado &quot;Todos os projetos no portfólio de marketing&quot; na [!UICONTROL Filtro herdado] experiência. Isso mostrará todos os projetos no portfólio chamados &quot;Portfolio de marketing&quot;, independentemente do status.

O passo a passo é apresentado abaixo.

### Resposta à Atividade 1

![Uma imagem da tela para criar um novo filtro](assets/basic-filter-activity-1.png)

1. Navegue até a área [!UICONTROL Projetos] do [!UICONTROL Menu principal]. Você verá uma lista de projetos.
1. Clique em **[!UICONTROL Filtro]** e selecione [!UICONTROL Filtros legados].
1. Selecionar **[!UICONTROL Novo Filtro]**.
1. Nomeie seu filtro como &quot;Todos os projetos no portfólio de marketing&quot;.
1. Clique em **[!UICONTROL Adicionar regra de filtro]**.
1. No [!UICONTROL Comece a digitar o nome do campo] campo, tipo &quot;[!UICONTROL nome do portfólio]&quot;. Em seguida, selecione [!UICONTROL Nome] no [!UICONTROL Portfolio] origem do campo.
1. Deixe o operador [!UICONTROL Igual] como está.
1. Tipo &quot;[!UICONTROL marketing]&quot; no [!UICONTROL Comece a digitar o nome] campo.
1. Selecionar [!UICONTROL Portfolio de marketing] supondo que você tenha um portfólio com esse nome no qual deseja filtrar. Se não estiver apenas usando o recurso de digitação antecipada para encontrar o portfólio desejado.
1. Clique em **[!UICONTROL Salvar Filtro]**.

## Atividade 2 - Projetos que possuo fechando este mês

Neste vídeo, você criará um filtro de projeto chamado &quot;Projetos que possuo fechando este mês&quot; na [!UICONTROL Filtro herdado] experiência. Se você estiver de olho em muitos projetos, este filtro pode ajudá-lo a ampliar aqueles que estão planejados para fechar em breve.

O passo a passo é apresentado abaixo.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

### Resposta à Atividade 2

![Uma imagem da tela para criar um novo filtro](assets/basic-filter-activity-updated-6-15-21.png)

1. Navegue até a área [!UICONTROL Projetos] do [!UICONTROL Menu principal]. Você verá uma lista de projetos.
1. Clique em **[!UICONTROL Filtro]** e selecione [!UICONTROL Filtros legados].
1. Selecionar **[!UICONTROL Novo Filtro]**.
1. Nomeie seu filtro como &quot;Projetos que possuo fechando este mês&quot;.
1. Clique em **[!UICONTROL Adicionar regra de filtro]**.
1. No [!UICONTROL Comece a digitar o nome do campo] digite &quot;proprietário&quot;. Em seguida, selecione [!UICONTROL ID do proprietário] na fonte do campo [!UICONTROL Projeto].
1. Deixe o operador [!UICONTROL Igual] como está.
1. Digite &quot;$$&quot; no [!UICONTROL Comece a digitar o nome] campo.
1. Selecione [!UICONTROL $$USER.ID].  Esse é o curinga do usuário conectado.
1. Clique em [!UICONTROL Adicionar regra de filtro] novamente.
1. No [!UICONTROL Comece a digitar o nome do campo] digite &quot;Está concluído&quot;. Em seguida, selecione [!UICONTROL Está concluído] na origem do campo “Projeto”.
1. Deixe o operador [!UICONTROL Igual] como está.
1. Selecione &quot;Falso&quot;.
1. Clique em [!UICONTROL Adicionar regra de filtro] novamente.
1. No [!UICONTROL Comece a digitar o nome do campo] tipo de campo &quot;planejado&quot;, selecione [!UICONTROL Data de Término Planejada] no [!UICONTROL Projeto] origem do campo.
1. Altere o operador [!UICONTROL Igual] para [!UICONTROL Este mês].
1. Clique em **[!UICONTROL Salvar Filtro]**.
