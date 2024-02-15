---
title: Criar atividades básicas de filtro
description: Nesta atividade, você criará um filtro de projeto chamado “Meus projetos que se encerram neste mês”.
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
workflow-type: ht
source-wordcount: '420'
ht-degree: 100%

---

# Criar atividades básicas de filtro

## Atividade 1: todos os projetos no portfólio de marketing

Nesta atividade, você criará um filtro de projeto chamado “Todos os projetos no portfólio de marketing” utilizando a experiência de [!UICONTROL filtro herdada]. Isso mostrará todos os projetos no “Portfólio de marketing”, independentemente do status deles.

O passo a passo é apresentado abaixo.

### Resposta à atividade 1

![Uma imagem da tela para criar um novo filtro](assets/basic-filter-activity-1.png)

1. Navegue até a área [!UICONTROL Projetos] do [!UICONTROL Menu principal]. Você verá uma lista de projetos.
1. Clique no menu **[!UICONTROL Filtro]** e selecione [!UICONTROL Filtros herdados].
1. Selecione **[!UICONTROL Novo filtro]**.
1. Nomeie seu filtro como “Todos os projetos no portfólio de marketing”.
1. Clique em **[!UICONTROL Adicionar regra de filtro]**.
1. No campo [!UICONTROL Comece a digitar o nome do campo], digite “[!UICONTROL nome do portfólio]”. Em seguida, selecione [!UICONTROL Nome] no campo de origem [!UICONTROL Portfólio].
1. Deixe o operador [!UICONTROL Igual] como está.
1. Digite “[!UICONTROL marketing]” no campo [!UICONTROL Comece a digitar o nome].
1. Selecione [!UICONTROL Portfólio de marketing] se possuir um portfólio com esse nome que deseja filtrar. Caso contrário, utilize o recurso de previsão de texto para encontrar o portfólio desejado.
1. Clique em **[!UICONTROL Salvar filtro]**.

## Atividade 2: meus projetos que se encerram este mês

Neste vídeo, você criará um filtro de projeto chamado “Meus projetos que se encerram este mês” na experiência de [!UICONTROL filtro herdada]. Se estiver monitorando muitos projetos, esse filtro pode ajudar a focar nos que estão planejados para se encerrar em breve.

O passo a passo é apresentado abaixo.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

### Resposta à atividade 2

![Uma imagem da tela para criar um novo filtro](assets/basic-filter-activity-updated-6-15-21.png)

1. Navegue até a área [!UICONTROL Projetos] do [!UICONTROL Menu principal]. Você verá uma lista de projetos.
1. Clique no menu **[!UICONTROL Filtro]** e selecione [!UICONTROL Filtros herdados].
1. Selecione **[!UICONTROL Novo filtro]**.
1. Nomeie o filtro como “Meus projetos que se encerram este mês”.
1. Clique em **[!UICONTROL Adicionar regra de filtro]**.
1. No campo [!UICONTROL Comece a digitar o nome do campo], digite “proprietário”. Em seguida, selecione [!UICONTROL ID do proprietário] na fonte do campo [!UICONTROL Projeto].
1. Deixe o operador [!UICONTROL Igual] como está.
1. Digite “$$” no campo [!UICONTROL Comece a digitar o nome].
1. Selecione [!UICONTROL $$USER.ID].  Esse é o curinga do usuário conectado.
1. Clique em [!UICONTROL Adicionar regra de filtro] novamente.
1. No campo [!UICONTROL Comece a digitar o nome do campo], digite “Está concluído”. Em seguida, selecione [!UICONTROL Está concluído] na origem do campo “Projeto”.
1. Deixe o operador [!UICONTROL Igual] como está.
1. Selecione “Falso”.
1. Clique em [!UICONTROL Adicionar regra de filtro] novamente.
1. No campo [!UICONTROL Comece a digitar o nome do campo], digite “planejada” e selecione [!UICONTROL Data de conclusão planejada] na origem do campo [!UICONTROL Projeto].
1. Altere o operador [!UICONTROL Igual] para [!UICONTROL Este mês].
1. Clique em **[!UICONTROL Salvar filtro]**.
