---
title: Entender o modo de texto básico para filtros
description: Saiba qual é o modo de texto, qual é o caso de camel e algum modo de texto "plug and play" básico que você pode usar nos filtros de relatório no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Entender o modo de texto básico para filtros

>[!IMPORTANT]
>
>Pré-requisitos:
>
>* Entender os elementos de relatório
>* Entender os componentes de relatório
>* Criar um filtro básico


>[!TIP]
>
>* Para obter uma compreensão mais profunda do modo de texto, recomendamos assistir ao evento de webinar gravado [Pergunte a um especialista - Introdução aos relatórios do modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tem duração de uma hora.
>* Para saber mais ainda sobre o modo de texto, recomendamos assistir ao [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriais, que juntos têm cinco horas e meia de duração.



Neste vídeo, você aprenderá:

* O modo de texto é
* Qual é o caso do camelo?
* Algum modo de texto &quot;plug and play&quot; básico que você pode usar nos filtros de relatório

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)


## Tarefa - Filtrar tarefas em que marquei &quot;Concluído com a minha parte&quot;

O modo de texto a seguir excluirá tarefas em que um usuário marcou &quot;Concluído com a minha parte&quot;. Tudo o que você precisa fazer é criar um filtro de tarefa, adicionar as regras de filtro desejadas, alternar para o modo de texto e colar o código abaixo após qualquer modo de texto que você ver no filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Tarefa - Mostrar todas as tarefas que aguardam a minha aprovação

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## Tarefa - Mostrar todas as tarefas que aprovei

Crie um relatório de tarefa com os filtros desejados, vá para a guia Filter e clique em Switch to Text Mode. Adicione este código ao que já estiver lá:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## Tarefa - Mostre-me todas as tarefas que tenham pelo menos um antecessor entre projetos

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## Tarefa - Mostrar todas as tarefas que atribuí a outros

Crie um relatório de tarefa com os filtros desejados, vá para a guia Filter e clique em Switch to Text Mode. Adicione este código ao que já estiver lá:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Isso mostrará todas as tarefas em que o usuário conectado atribuiu pelo menos um dos destinatários atuais. Se os destinatários tiverem sido atribuídos por várias pessoas, somente o nome da primeira pessoa que atribuiu alguém será exibido como &quot;Solicitado por&quot; na página de aterrissagem da tarefa.

## Tarefa - Mostrar todas as tarefas concluídas - Aprovação pendente

```
status=CPL:A
status_Mod=in
```


## Problema - Mostre-me todos os problemas que estão completos - Aprovação pendente

```
status=CPL:A
status_Mod=in
```


## Projeto - Mostre-me todos os projetos concluídos - aprovação pendente

```
status=CPL:A
status_Mod=in
```


## Observação - Mostrar todos os comentários que estou conectado

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Relatório de parâmetro/campo personalizado - Mostre-me campos personalizados que não estão anexados a um formulário personalizado (muito útil em esforços de limpeza)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
