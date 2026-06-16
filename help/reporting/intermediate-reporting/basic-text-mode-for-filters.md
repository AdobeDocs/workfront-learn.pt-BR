---
title: Explorar o modo de texto básico para filtros no Workfront
description: Saiba mais sobre o modo de texto, camel case e alguns modos de texto básicos que você pode usar nos filtros de relatório no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-07-30T00:00:00.000Z'
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: cec4c78b-dd2b-46ec-b824-6ca30f0eb7b2
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:59:16.164Z'
source-git-commit: f0f541bf3fd6db69e6d813cf81456a5df6848d49
workflow-type: tm+mt
source-wordcount: 504
ht-degree: 85%

---

# Explorar o modo de texto básico para filtros no Workfront

>[!PREREQUISITES]
>
>* [Explorar elementos de relatórios do Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=pt-BR)
>* [Explorar componentes de relatórios no Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=pt-BR)
>* [Criar um filtro básico](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=pt-BR)


>[!TIP]
>
>* Para obter uma compreensão mais aprofundada do modo de texto, recomendamos assistir ao evento do webinário gravado [Pergunte ao especialista - Introdução aos relatórios em modo de texto](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), que tem uma hora de duração.
>* Para aprender ainda mais sobre o modo de texto, recomendamos assistir aos tutoriais de [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=pt-BR), que juntos têm cinco horas e meia de duração.
>* Clique aqui para acessar o [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)


Neste vídeo, você aprenderá sobre:

* Modo texto
* Camel case
* Alguns _blocos de código do modo texto_ que você pode usar nos filtros de relatório

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on&enablevpops=0)

## Atividades “Compreender o modo de texto básico para filtros”


### Tarefa: Filtrar as tarefas em que marquei “Minha parte foi concluída”

O modo de texto a seguir excluirá tarefas em que um usuário marcou “Minha parte foi concluída”. Basta criar um filtro de tarefa, adicionar as regras de filtro desejadas, alternar para o modo de texto e colar o código abaixo após qualquer modo de texto exibido no filtro.


>[!WARNING]
>
> Não foi feito para uso nos filtros do calendário.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

### Tarefa: Mostrar todas as tarefas aguardando minha aprovação

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Tarefa: Mostrar todas as tarefas que aprovei

Crie um relatório de tarefas com os filtros desejados, vá para a guia Filtro e clique em Alternar para modo de texto. Adicione este código ao que já estiver lá:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Tarefa: Mostrar todas as tarefas que tenham pelo menos um predecessor entre projetos

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Tarefa: Mostrar todas as tarefas que atribuí a outras pessoas

Crie um relatório de tarefas com os filtros desejados, vá para a guia Filtro e clique em Alternar para modo de texto. Adicione este código ao que já estiver lá:

>[!WARNING]
> 
> Não foi feito para uso nos filtros do calendário.

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Isso mostrará todas as tarefas para as quais o usuário conectado atribuiu pelo menos um dos cessionários atuais. Se os cessionários foram atribuídos por várias pessoas, apenas o nome da primeira pessoa que atribuiu alguém aparecerá como “Solicitado por” na página de destino da tarefa.

### Tarefa: Mostrar todas as tarefas concluídas - Aprovação pendente

```
status=CPL:A
status_Mod=in
```


### Problema: Mostrar todos os problemas concluídos - Aprovação pendente

```
status=CPL:A
status_Mod=in
```


### Projeto: Mostrar todos os projetos concluídos - Aprovação pendente

```
status=CPL:A
status_Mod=in
```


### Observação: Mostrar todos os comentários em que fui marcado

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### Relatório de parâmetro/campo personalizado: Mostrar campos personalizados que não estão anexados a um formulário personalizado (muito útil em iniciativas de limpeza)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
