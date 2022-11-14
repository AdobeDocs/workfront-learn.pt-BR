---
title: Entender o modo de texto básico para exibições
description: Saiba qual é o modo de texto, qual é o caso de camel e algum modo de texto "plug and play" básico que você pode usar em suas visualizações no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
source-git-commit: 818ee105af32589cb0e297e6f419a4a449a60052
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Entender o modo de texto básico para exibições


>[!IMPORTANT]
>
>Pré-requisitos:
>
>* Entender os elementos de relatório
>* Entender os componentes de relatório
>* Criar uma exibição básica


>[!TIP]
>
>* Para obter uma compreensão mais profunda do modo de texto, recomendamos assistir ao evento de webinar gravado [Pergunte a um especialista - Introdução aos relatórios do modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tem duração de uma hora.
>* Para saber mais ainda sobre o modo de texto, recomendamos assistir ao [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriais, que juntos têm cinco horas e meia de duração.


Neste vídeo, você aprenderá:

* O modo de texto é
* Qual é o caso do camelo?
* Algum modo de texto &quot;plug and play&quot; básico que você pode usar em suas visualizações

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12)

## Tarefa - exibição 4 pais

Crie uma coluna para o Nome da tarefa e o Nome pai primeiro e use o seguinte modo de texto para criar as outras três colunas.

### Tarefa - Pai do Nome Pai

```
displayname=Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:name
textmode=true
valuefield=parent:parent:name
valueformat=HTML
```

### Tarefa - Pai do Nome Pai

```
displayname=Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:name
valueformat=HTML
```

### Tarefa - Pai do Pai do Nome do Pai

```
displayname=Parent of Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:parent:name
valueformat=HTML
```

![Uma imagem de tela mostrando a exibição 4 pais](assets/4-parents-view.png)

## Usuário - Iterações que mostram listas nas visualizações do usuário

### Usuário - Todas as funções

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### Usuário - Todas as funções de trabalho que mostram as principais

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### Usuário - Todas as equipes

```
displayname=All teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

>[!NOTE]
>
>Existe um campo Equipe acessível por meio da interface do usuário que mostra todas as equipes, separadas por vírgulas, mas o uso do modo de texto acima mostrará cada equipe em uma linha separada.


### Usuário - Todos os grupos

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### Usuário - Todos os grupos que mostram o grupo inicial

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### Usuário - Relatórios diretos

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### Usuário - PTO Futuro

```
displayname=Future PTO
listdelimiter=<br>
listmethod=nested(reservedTimes).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),"")
valueformat=HTML
width=150
```

![Uma imagem de tela mostrando a exibição de listas de usuários](assets/user-lists-view-large.png)

## Tarefa - Como exibir atribuições de tarefas e trabalhar no status

```
displayname=Assignments and Status
listdelimiter=<br>
listmethod=nested(assignments).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT({assignedTo}.{name},IF(ISBLANK({assignedTo}.{name}),"",IF({status}="AA"," - Requested",IF({status}="AD"," - Working"," - Done"))))
valueformat=HTML
width=150
```

![Uma imagem da tela mostrando a exibição Atribuições e Status](assets/assignments-and-status-view.png)


## Tarefa - Como mostrar a função e alocação em várias atribuições de tarefa

### Tarefa - Função + horas

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### Tarefa - Atribuição + alocação de porcentagem

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![Uma imagem da tela mostrando a exibição Atribuições e Funções](assets/assignments-roles-and-percent-view.png)

## Tarefa - Antecessores e sucessores de projetos cruzados

### Filtro de tarefas (opcional)

**Mostrar todas as tarefas que tenham pelo menos um antecessor de projeto cruzado**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Tarefa - Mostrar nomes de antecessores e o antecessor do projeto está em

```
displayname=Predecessor names
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{predecessor}.{name}," >> PROJECT = ",{predecessor}.{project}.{name})
valueformat=HTML
width=150
```

### Tarefa - Mostrar nomes de sucessores e sucessor do projeto está em

```
displayname=Successor names
listdelimiter=<br>
listmethod=nested(successors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{successor}.{name}," >> PROJECT = ",{successor}.{project}.{name})
valueformat=HTML
width=150
```

### Tarefa - Mostrar a data de conclusão projetada dos antecessores

```
displayname=Predecessor projected completion dates
valueformat=atDate
listdelimiter=
textmode=true
width=90
stretch=0
valuefield=predecessor:projectedCompletionDate
type=iterate
listmethod=nested(predecessors).lists
shortview=false
```

### Tarefa - Mostrar status de progresso dos predecessores

```
displayname=Predecessor progress status
listdelimiter=<br>
listmethod=nested(predecessors).lists
shortview=false
stretch=0
textmode=true
type=iterate
valueexpression=IF({predecessor}.{progressStatus}="OT","On Time",IF({predecessor}.{progressStatus}="LT","Late",IF({predecessor}.{progressStatus}="BH","Behind","At Risk")))
valueformat=HTML
width=90
```

### Tarefa - Mostrar a porcentagem completa do projeto entre projetos do antecessor

```
displayname=Predecessor project percent complete
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({isCP}=true,CONCAT({predecessor}.{project}.{percentComplete},"%"),"")
valueformat=HTML
width=150
```

![Uma imagem de tela mostrando a exibição entre predecessores e sucessores do projeto](assets/cross-project-predecessors-and-successors.png)


## Tarefa - Iteração mostrando todas as pessoas atribuídas e que atribuíram cada uma

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![Uma imagem de tela mostrando todas as pessoas atribuídas e que atribuíram cada uma](assets/all-assignees-and-requesters.png)

## Tarefa/Projeto - Iteração mostrando todos os formulários personalizados em um projeto ou tarefa

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![Uma imagem de tela mostrando todos os formulários personalizados em um projeto](assets/all-custom-forms-on-a-project.png)


## Projeto - Iteração mostrando todos os contatos primários para resolvíveis na exibição do projeto

```
displayname=Requestor
listdelimiter=<br>
listmethod=nested(resolvables).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=owner:name
valueformat=HTML
width=150
```

![Uma imagem de tela mostrando contatos primários para resolvíveis](assets/primary-contacts-for-resolvables.png)

## Projeto - Iteração mostrando todos os membros da equipe do projeto

```
displayname=Project Team Members
listdelimiter=<br>
listmethod=nested(projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

![Uma imagem de tela mostrando todos os membros da equipe do projeto](assets/all-project-team-members.png)

## Projeto - Iteração mostrando a entradaData de todos os problemas resolvíveis de um projeto

```
displayname=Resolvables entry date
linkedname=direct
listdelimiter=<br>
listmethod=nested(project.resolvables).lists
listsort=string(description)
querysort=description
section=0
textmode=true
type=iterate
valuefield=entryDate
valueformat=HTML
```

![Uma imagem de tela mostrando a entradaData de todos os problemas resolvíveis de um projeto](assets/resolvables-entry-date.png)

## Projeto - Mostrar o grupo inicial do solicitante do projeto original

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Uma imagem da tela mostrando o grupo inicial do solicitante do projeto](assets/requestor-home-group.png)

## Projeto - Mostrar se o projeto é uma fila de solicitações

```
querysort=queueDef:isPublic
valueformat=val
description=0 (None), 1 (Public), 2 (Private), 3 (Company), 4 (Group)
linkedname=direct
textmode=true
enumtype=PROJ
valuefield=queueDef:isPublic
namekey=status
type=enum
enumclass=com.attask.common.constants.ProjectStatusEnum
displayname=Public Selection
```

![Uma imagem de tela mostrando se o projeto é uma fila de solicitações](assets/project-is-a-request-queue.png)

## Problema - Iteração mostrando todos os membros da equipe de projeto resolvidos

```
displayname=Resolve Project: Team Members
listdelimiter=<br>
listmethod=nested(resolveProject.projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
width=150
```

![Uma imagem de tela mostrando todos os membros da equipe de projeto resolvidos](assets/all-resolve-project-team-members.png)

## Problema - Iteração mostrando todas as equipes do contato principal do problema

```
displayname=Requestor Teams
listdelimiter=<br>
listmethod=nested(owner.teams).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=name
valueformat=HTML
width=150
```

![Uma imagem de tela mostrando todas as equipes de contato primárias](assets/all-primary-contact-teams.png)

## Documento - Iteração mostrando a pasta em um relatório de documento

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![Uma imagem de tela mostrando a pasta em um relatório de documento](assets/folder-in-a-document-report.png)

## Documento - Iteração mostrando a pasta principal em um relatório de documento

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![Uma imagem de tela mostrando a pasta principal em um relatório de documento](assets/parent-folder-in-a-document-report.png)

## Documento - Datas de aprovação do documento

```
displayname=Document Approval Dates
valueformat=HTML
listdelimiter=<br>
linkedname=direct
textmode=true
listsort=string(description)
valuefield=approvalDate
type=iterate
listmethod=nested(approvals).lists
shortview=false
section=0
```

![Uma imagem de tela mostrando a exibição Datas de aprovação do documento](assets/document-approval-dates.png)

## Aprovações de revisões

### Aprovação de prova - Mostrar nome do projeto

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### Aprovação de prova - Mostrar nome da tarefa

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Uma imagem de tela mostrando o projeto e a tarefa de uma aprovação de prova](assets/proof-approval-project-and-task.png)
