---
title: Criar uma atividade básica de filtro
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
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Criar uma atividade básica de filtro

Neste vídeo, você criará um filtro de projeto chamado &quot;Projetos que possuo fechando este mês&quot;. Se você estiver de olho em muitos projetos, esse filtro pode ajudá-lo a ampliar aqueles que estão planejados para fechar em breve.

As instruções passo a passo estão incluídas abaixo.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

## Resposta

![Uma imagem da tela para criar um novo filtro](assets/basic-filter-activity-updated-6-15-21.png)

1. Navegue até a [!UICONTROL Projetos] área a partir da [!UICONTROL Menu principal]. Você verá uma lista de projetos.
1. Clique em **[!UICONTROL Filtro]** e selecione **[!UICONTROL Novo Filtro]**.
1. Nomeie seu filtro &quot;Projetos que possuo fechando este mês&quot;.
1. Clique em **[!UICONTROL Adicionar Regra de Filtro]**.
1. No [!UICONTROL Comece a digitar o nome do campo] digite &quot;proprietário&quot;. Em seguida, selecione [!UICONTROL ID do proprietário] no [!UICONTROL Projeto] origem do campo.
1. Deixe a [!UICONTROL Igual] operador como está.
1. Digite &quot;$$&quot; no campo Comece a digitar o nome.
1. Selecionar [!UICONTROL $$USER.ID]. Este é o curinga do usuário conectado.
1. Clique em [!UICONTROL Adicionar Regra de Filtro] novamente.
1. No [!UICONTROL Comece a digitar o nome do campo] digite &quot;Está concluído&quot;. Em seguida, selecione [!UICONTROL Está Concluído] na origem do campo Projeto.
1. Deixe a [!UICONTROL Igual] operador como está.
1. Selecione &quot;Falso&quot;.
1. Clique em [!UICONTROL Adicionar Regra de Filtro] novamente.
1. No [!UICONTROL Comece a digitar o nome do campo] tipo de campo &quot;planejado&quot;, selecione [!UICONTROL Data de Término Planejada] no [!UICONTROL Projeto] origem do campo.
1. Altere o [!UICONTROL Igual] operador para [!UICONTROL Este mês].
1. Clique em **[!UICONTROL Salvar Filtro]**
