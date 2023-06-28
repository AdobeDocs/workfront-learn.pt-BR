---
title: Entender o modo de texto básico para filtros
description: Saiba o que é modo de texto, o que é camel case e conheça modos de texto básicos de "plug and play" que podem ser usados nos filtros de relatório no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Entender o modo de texto básico para filtros

>[!IMPORTANT]
>
>Pré-requisitos:
>
>* Entender os elementos de relatórios
>* Entender os componentes de relatórios
>* Criar um filtro básico

>[!TIP]
>
>* Para obter uma compreensão mais detalhada do modo de texto, recomendamos assistir ao evento gravado do webinário [Pergunte a um especialista - Introdução aos relatórios no modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tem uma hora de duração.
>* Para saber ainda mais sobre o modo de texto, recomendamos assistir ao [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriais, que juntos têm cinco horas e meia de duração.


Neste vídeo, você aprenderá:

* O que é modo texto
* O que camel case é
* Alguns modos básicos de texto &quot;plug and play&quot; que podem ser usados nos filtros de relatório

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## Tarefa - Filtre as tarefas nas quais marquei &quot;Concluído com minha parte&quot;

O modo de texto a seguir excluirá as tarefas nas quais o usuário tiver marcado &quot;Concluído com minha parte&quot;. Basta criar um filtro de tarefa, adicionar as regras de filtro desejadas, alternar para o modo de texto e colar o código abaixo após qualquer modo de texto exibido no filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Tarefa - Mostrar todas as tarefas que estão aguardando minha aprovação

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## Tarefa - Mostrar todas as tarefas aprovadas

Crie um relatório de tarefas com os filtros que quiser, vá para a guia Filter e clique em Switch to Text Mode (Alternar para modo de texto). Adicionar este código ao que já estiver lá:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## Tarefa - Mostre todas as tarefas que tenham pelo menos uma predecessora entre projetos

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## Tarefa - Mostrar todas as tarefas atribuídas a outras pessoas

Crie um relatório de tarefas com os filtros que quiser, vá para a guia Filter e clique em Switch to Text Mode (Alternar para modo de texto). Adicionar este código ao que já estiver lá:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Isso mostrará todas as tarefas em que o usuário conectado atribuiu pelo menos um dos atribuídos atuais. Se os atribuídos foram atribuídos por várias pessoas, somente o nome da primeira pessoa que atribuiu alguém será exibido como &quot;Solicitado por&quot; na landing page da tarefa.

## Tarefa - Mostrar todas as tarefas que estão Concluídas - Aprovação Pendente

```
status=CPL:A
status_Mod=in
```


## Problema - Mostrar todos os problemas Concluídos - Aprovação Pendente

```
status=CPL:A
status_Mod=in
```


## Projeto - Mostrar todos os projetos Concluídos - Aprovação Pendente

```
status=CPL:A
status_Mod=in
```


## Observação - mostrar todos os comentários nos quais estou marcado

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Relatório de parâmetro/campo personalizado - Mostre-me os campos personalizados que não estão anexados a um formulário personalizado (muito útil em esforços de limpeza)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
