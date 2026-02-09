---
title: Explorar modo de texto básico para agrupamentos no Workfront
description: Saiba mais sobre modo de texto, camel case e alguns modos de texto básicos que você pode usar nos agrupamentos de relatório no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-12T00:00:00Z
jira: KT-11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
doc-type: video
source-git-commit: 66bab1a0b2316a31cb99916220500303e49797ad
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 82%

---

# Explorar modo de texto básico para agrupamentos no Workfront

>[!PREREQUISITES]
>
>* [Entenda os elementos dos relatórios](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=pt-BR)
>* [Entenda os componentes dos relatórios](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=pt-BR)
>* [Criar um agrupamento básico](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-grouping.html?lang=pt-BR)


>[!TIP]
>
>* Para obter uma compreensão mais aprofundada do modo de texto, recomendamos assistir ao evento do webinário gravado [Pergunte ao especialista - Introdução aos relatórios em modo de texto](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), que tem uma hora de duração.
>* Para aprender ainda mais sobre o modo de texto, recomendamos assistir aos tutoriais de [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=pt-BR), que juntos têm cinco horas e meia de duração.
>* Clique aqui para acessar o [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)

Neste vídeo, você aprenderá:

* O que é o modo de texto
* O que é camel case
* Alguns _blocos de código do modo texto_ que você pode usar nos agrupamentos de relatório

>[!VIDEO](https://video.tv.adobe.com/v/3470785/?captions=por_br&quality=12&learn=on&enablevpops=0)

## Atividades “Compreender o modo de texto básico para agrupamentos”

### Tarefa: agrupamento de quatro páginas principais

O modo de texto a seguir agrupará tarefas com base em até quatro níveis de página principal e deixará as páginas principais inexistentes em branco.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![Uma imagem de tela mostrando tarefas do projeto agrupadas em quatro páginas principais](assets/4-parents-grouping.png)


### Tarefa: agrupamento de percentual concluído

O modo de texto a seguir agrupará tarefas com base no percentual concluído. As tarefas serão encaixadas em uma das seguintes categorias quando agrupadas:

* 0%
* 1% a 25%
* 26% a 50%
* 51% a 75%
* 76% a 99%
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![Uma imagem de tela mostrando as tarefas do projeto agrupadas por percentual concluído](assets/percent-complete-grouping.png)

### Tarefa: statusEquatesWith e, em seguida, status

O modo de texto a seguir agrupará as tarefas por statusEquatesWith e, em seguida, por status.

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![Uma imagem de tela mostrando as tarefas do projeto agrupadas por statusEquatesWith](assets/status-equates-with.png)


### Aprovação da revisão: agrupar por nome do projeto

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![Uma imagem de tela mostrando aprovações de revisões agrupadas por nome do projeto](assets/proof-approvals-grouped-by-project-name.png)


### Aprovação da revisão: agrupar por nome do documento

```
group.0.displayname=Document Name
group.0.valuefield=documentVersion:document:name
group.0.valueformat=HTML
```

![Uma imagem de tela mostrando aprovações de revisões agrupadas por nome do projeto](assets/proof-approvals-grouped-by-doc-name.png)

