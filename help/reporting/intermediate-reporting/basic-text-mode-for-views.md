---
title: Entender o modo de texto básico para exibições
description: Saiba o que é modo de texto, o que é camel case e conheça modos de texto básicos de "plug and play" que podem ser usados em suas visualizações no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: 18aa5b742c4ad6210893af6141aa0b2777ab3c2a
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Entender o modo de texto básico para exibições


>[!IMPORTANT]
>
>Pré-requisitos:
>
>* Entender os elementos de relatórios
>* Entender os componentes de relatórios
>* Criar uma exibição básica


>[!TIP]
>
>* Para obter uma compreensão mais detalhada do modo de texto, recomendamos assistir ao evento gravado do webinário [Pergunte a um especialista - Introdução aos relatórios no modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tem uma hora de duração.
>* Para saber ainda mais sobre o modo de texto, recomendamos assistir ao [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriais, que juntos têm cinco horas e meia de duração.


Neste vídeo, você aprenderá:

* O que é modo texto
* O que camel case é
* Alguns modos básicos de texto &quot;plug and play&quot; que podem ser usados em suas visualizações

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12&learn=on)

## Tarefa - exibição com 4 pais

Primeiro, crie uma coluna para o Nome da Tarefa e o Nome do Pai e, em seguida, use o seguinte modo de texto para criar as outras três colunas.

### Tarefa - Pai do Nome do Pai

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

### Tarefa - Pai do Nome do Pai

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

![Uma imagem de tela mostrando a exibição com 4 pais](assets/4-parents-view.png)

## Usuário - Iterações mostrando listas em visualizações do usuário

### Usuário - Todas as funções de trabalho

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### Usuário - Todas as funções de trabalho mostrando o principal

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
>Há um campo Equipe acessível por meio da interface do usuário que mostra todos os grupos, separados por vírgulas, mas usando o modo de texto acima, cada grupo será exibido em uma linha separada.


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

### Usuário - PTO futuro

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

![Uma imagem de tela mostrando a visualização Listas de usuários](assets/user-lists-view-large.png)

## Tarefa - Como exibir as atribuições de tarefas e o status de trabalho

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

![Uma imagem de tela mostrando a exibição de Atribuições e Status](assets/assignments-and-status-view.png)


## Tarefa - Como mostrar a função e a alocação em atribuições de várias tarefas

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

### Tarefa - Atribuição + porcentagem de alocação

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![Uma imagem de tela mostrando a exibição de Atribuições e Funções](assets/assignments-roles-and-percent-view.png)

## Tarefa - predecessores e sucessores entre projetos

### Filtro de tarefa (opcional)

**Mostre-me todas as tarefas que tenham pelo menos uma predecessora entre projetos**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Tarefa - Mostrar nomes de predecessores e a predecessora do projeto está em

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

### Tarefa - Mostrar nomes de sucessores e o sucessor do projeto está em

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

### Tarefa - Mostra a data de conclusão projetada dos predecessores

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

### Tarefa - Mostrar status do progresso dos predecessores

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

### Tarefa - Mostra o percentual concluído do projeto da predecessora entre projetos

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

![Uma imagem de tela mostrando os predecessores e sucessores entre projetos](assets/cross-project-predecessors-and-successors.png)


## Tarefa - Iteração que mostra todas as pessoas atribuídas e que atribuíram cada uma

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

## Tarefa/Projeto - Iteração que mostra todos os formulários personalizados em um projeto ou tarefa

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


## Projeto - Iteração mostrando todos os contatos principais para contas a resolver na exibição de projeto

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

![Uma imagem de tela mostrando os contatos principais para contas a resolver](assets/primary-contacts-for-resolvables.png)

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

## Projeto - Iteração mostrando a entryDate de todos os problemas resolvíveis de um projeto

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

![Uma imagem de tela mostrando a entryDate de todos os problemas resolvíveis de um projeto](assets/resolvables-entry-date.png)

## Projeto - Mostra o grupo inicial do solicitante do projeto original

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Uma imagem de tela mostrando o grupo inicial do solicitante do projeto](assets/requestor-home-group.png)

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

## Problema - Iteração mostrando todos os membros da equipe de resolução de projetos

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

![Uma imagem de tela mostrando todos os membros da equipe do projeto resolvidos](assets/all-resolve-project-team-members.png)

## Problema - Iteração que mostra todas as equipes do contato principal do problema

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

![Uma imagem de tela mostrando todas as equipes de contato principais](assets/all-primary-contact-teams.png)

## Documento - Iteração que mostra a pasta em um relatório de documento

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![Uma imagem de tela mostrando a pasta no relatório de um documento](assets/folder-in-a-document-report.png)

## Documento - Iteração que mostra a pasta principal em um relatório de documento

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

## Documento - Datas de aprovação de documentos

```
displayname=Document approval dates
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

![Uma imagem de tela mostrando a exibição das datas de aprovação do documento](assets/document-approval-dates.png)

## Aprovações de revisões

### Aprovação da prova - Mostrar nome do projeto

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### Aprovação da prova - Mostrar nome da tarefa

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Uma imagem de tela mostrando o projeto e a tarefa de uma aprovação de prova](assets/proof-approval-project-and-task.png)
