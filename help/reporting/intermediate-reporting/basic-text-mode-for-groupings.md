---
title: Entender o modo de texto básico para agrupamentos
description: Saiba o que é modo de texto, o que é camel case e conheça modos de texto básicos de "plug and play" que podem ser usados em seus agrupamentos no Workfront.
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
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Entender o modo de texto básico para agrupamentos

>[!IMPORTANT]
>
>Pré-requisitos:
>
>* Entender os elementos de relatórios
>* Entender os componentes de relatórios
>* Criar um agrupamento básico


>[!TIP]
>
>* Para obter uma compreensão mais detalhada do modo de texto, recomendamos assistir ao evento gravado do webinário [Pergunte a um especialista - Introdução aos relatórios no modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tem uma hora de duração.
>* Para saber ainda mais sobre o modo de texto, recomendamos assistir ao [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriais, que juntos têm cinco horas e meia de duração.


Neste vídeo, você aprenderá:

* O que é modo texto
* O que camel case é
* Alguns modos básicos de texto &quot;plug and play&quot; que você pode usar em seus agrupamentos

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12)

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


## Tarefa - Agrupamento de percentual de conclusão

O modo de texto a seguir irá agrupar as tarefas com base na sua porcentagem concluída. As tarefas se encaixarão em uma das seguintes categorias quando agrupadas:

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

![Uma imagem de tela mostrando as tarefas do projeto agrupadas por porcentagem concluída](assets/percent-complete-grouping.png)

## Tarefa - statusEquatesWith, depois status

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

![Uma imagem de tela mostrando tarefas de projeto agrupadas por statusEquatesWith](assets/status-equates-with.png)


## Aprovação da prova - Agrupar por nome de projeto

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![Uma imagem de tela mostrando aprovações de provas agrupadas por nome de projeto](assets/proof-approvals-grouped-by-project-name.png)

