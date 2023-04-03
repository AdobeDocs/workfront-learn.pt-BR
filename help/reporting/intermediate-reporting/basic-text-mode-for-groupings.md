---
title: Entender o modo de texto básico para agrupamentos
description: Saiba qual é o modo de texto, qual é o caso de camel e algum modo de texto "plug and play" básico que você pode usar em seus agrupamentos no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Entender o modo de texto básico para agrupamentos

>[!IMPORTANT]
>
>Pré-requisitos:
>
>* Entender os elementos de relatório
>* Entender os componentes de relatório
>* Criar um agrupamento básico


>[!TIP]
>
>* Para obter uma compreensão mais profunda do modo de texto, recomendamos assistir ao evento de webinar gravado [Pergunte a um especialista - Introdução aos relatórios do modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tem duração de uma hora.
>* Para saber mais ainda sobre o modo de texto, recomendamos assistir ao [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriais, que juntos têm cinco horas e meia de duração.


Neste vídeo, você aprenderá:

* O modo de texto é
* Qual é o caso do camelo?
* Algum modo de texto &quot;plug and play&quot; básico que você pode usar em seus agrupamentos

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12&learn=on)

## Tarefa - Agrupamento de 4 pais

O modo de texto a seguir agrupará tarefas com base em até quatro níveis de pais e deixará os pais que não existirem em branco.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![Uma imagem de tela mostrando tarefas de projeto agrupadas por 4 pais](assets/4-parents-grouping.png)


## Tarefa - Percentual de agrupamento concluído

O modo de texto a seguir agrupará tarefas com base em sua porcentagem de conclusão. As tarefas serão incluídas em uma das seguintes categorias quando agrupadas:

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

![Uma imagem de tela mostrando tarefas de projeto agrupadas por porcentagem concluída](assets/percent-complete-grouping.png)

## Tarefa - statusEquatesWith, em seguida status

O modo de texto a seguir agrupará tarefas por statusEquatesWith e, em seguida, por status.

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


## Aprovação de prova - Agrupar por nome de projeto

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![Uma imagem de tela mostrando aprovações de Prova agrupadas pelo nome do projeto](assets/proof-approvals-grouped-by-project-name.png)

