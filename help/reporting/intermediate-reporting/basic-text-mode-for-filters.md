---
title: Compreensão do modo de texto básico para filtros
description: Aprenda o que é modo de texto, o que é camel case e alguns modos de texto “plug and play” básicos que você pode usar em seus filtros de relatório no Workfront.
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 61b6971457198d2c39cc4dab67aebc6e8c6988f6
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 100%

---

# Compreensão do modo de texto básico para filtros

>[!PREREQUISITES]
>
>* [Entenda os elementos dos relatórios](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=pt-BR)
>* [Entenda os componentes dos relatórios](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=pt-BR)
>* [Criar um filtro básico](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=pt-BR)


>[!TIP]
>
>* Para obter uma compreensão mais aprofundada do modo de texto, recomendamos assistir ao evento do webinário gravado [Pergunte ao especialista - Introdução aos relatórios em modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=br), que tem uma hora de duração.
>* Para aprender ainda mais sobre o modo de texto, recomendamos assistir aos tutoriais de [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=pt-BR), que juntos têm cinco horas e meia de duração.
>* Clique aqui para acessar o [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)


Neste vídeo, você aprenderá:

* O que é o modo de texto
* O que é camel case
* Um modo de texto básico “plug and play” que você pode usar em seus filtros de relatório

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## Tarefa: Filtrar as tarefas em que marquei “Minha parte foi concluída”

O modo de texto a seguir excluirá tarefas em que um usuário marcou “Minha parte foi concluída”. Basta criar um filtro de tarefa, adicionar as regras de filtro desejadas, alternar para o modo de texto e colar o código abaixo após qualquer modo de texto exibido no filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Tarefa: Mostrar todas as tarefas aguardando minha aprovação

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## Tarefa: Mostrar todas as tarefas que aprovei

Crie um relatório de tarefas com os filtros desejados, vá para a guia Filtro e clique em Alternar para modo de texto. Adicione este código ao que já estiver lá:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## Tarefa: Mostrar todas as tarefas que tenham pelo menos um predecessor entre projetos

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## Tarefa: Mostrar todas as tarefas que atribuí a outras pessoas

Crie um relatório de tarefas com os filtros desejados, vá para a guia Filtro e clique em Alternar para modo de texto. Adicione este código ao que já estiver lá:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Isso mostrará todas as tarefas para as quais o usuário conectado atribuiu pelo menos um dos cessionários atuais. Se os cessionários foram atribuídos por várias pessoas, apenas o nome da primeira pessoa que atribuiu alguém aparecerá como “Solicitado por” na página de destino da tarefa.

## Tarefa: Mostrar todas as tarefas concluídas - Aprovação pendente

```
status=CPL:A
status_Mod=in
```


## Problema: Mostrar todos os problemas concluídos - Aprovação pendente

```
status=CPL:A
status_Mod=in
```


## Projeto: Mostrar todos os projetos concluídos - Aprovação pendente

```
status=CPL:A
status_Mod=in
```


## Observação: Mostrar todos os comentários em que fui marcado

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Relatório de parâmetro/campo personalizado: Mostrar campos personalizados que não estão anexados a um formulário personalizado (muito útil em iniciativas de limpeza)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
