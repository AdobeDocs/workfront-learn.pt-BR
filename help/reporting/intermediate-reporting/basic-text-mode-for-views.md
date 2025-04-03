---
title: Entenda o modo de texto básico para visualizações
description: Aprenda o que é o modo de texto, o que é “Camel case” e veja alguns modos de texto “plug and play” básicos que você pode usar em suas visualizações no Workfront.
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: 2c9e57b8f85c74061bd3e52ef4eaea60bc4ec5bb
workflow-type: ht
source-wordcount: '656'
ht-degree: 100%

---

# Entenda o modo de texto básico para visualizações


>[!PREREQUISITES]
>
>* [Entenda os elementos dos relatórios](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=pt-BR)
>* [Entenda os componentes dos relatórios](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=pt-BR)
>* [Criar uma visualização básica](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-view.html?lang=pt-BR)


>[!TIP]
>
>* Para obter uma compreensão mais aprofundada do modo de texto, recomendamos assistir ao evento do webinário gravado [Pergunte ao especialista - Introdução aos relatórios em modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=pt-BR), que tem uma hora de duração.
>* Para aprender ainda mais sobre o modo de texto, recomendamos assistir aos tutoriais de [Relatórios avançados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=pt-BR), que juntos têm cinco horas e meia de duração.
>* Clique aqui para acessar o [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)

Neste vídeo, você aprenderá:

* O que é o modo de texto
* O que é camel case
* Alguns modos de texto “plug and play” básicos que você pode usar em suas visualizações

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12&learn=on)

## Atividades “Compreender o modo de texto básico para exibições”

### Tarefa - Visualização das 4 principais

Crie primeiro uma coluna para o Nome da tarefa e o Nome da principal e, depois, use o modo de texto a seguir para criar as outras três colunas.

#### Tarefa - Principal do nome da principal

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

#### Tarefa - Principal da principal do nome da principal

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

#### Tarefa - Principal da principal da principal do nome da principal

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

![Imagem de tela mostrando a visualização das 4 principais](assets/4-parents-view.png)

### Usuário - Iterações mostrando listas nas visualizações do usuário

#### Usuário - Todas as funções

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

#### Usuário - Todas as funções de trabalho mostrando opções primárias

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

#### Usuário - Todas as equipes

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
>A interface disponibiliza um campo de Equipe que mostra todas as equipes separadas por vírgulas, mas ao usar o modo de texto acima, cada equipe é exibida em uma linha separada.


#### Usuário - Todos os grupos

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

#### Usuário - Todos os grupos mostrando o grupo inicial

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


#### Usuário - Relatórios diretos

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

#### Usuário - Folga futura

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

![Imagem da tela que mostra a visualização de Listas de usuários](assets/user-lists-view-large.png)

### Tarefa - Como exibir atribuições de tarefas e status de trabalho

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

![Imagem da tela que mostra a visualização de Atribuições e Status](assets/assignments-and-status-view.png)


### Tarefa - Como mostrar a função e alocação em atribuições de várias tarefas

#### Tarefa - Função + horas

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

#### Tarefa - Atribuição + percentual de alocação

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![Imagem da tela que mostra a visualização de Atribuições e Funções](assets/assignments-roles-and-percent-view.png)

### Tarefa - Predecessoras e sucessoras entre projetos

#### Filtro de tarefa (opcional)

**Mostrar todas as tarefas que têm pelo menos uma predecessora ou sucessora entre os projetos atuais**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
project:statusEquatesWith=CUR
project:statusEquatesWith_Mod=in
OR:1:project:statusEquatesWith=CUR
OR:1:project:statusEquatesWith_Mod=in
OR:1:successorsMM:ID_Mod=notblank
OR:1:successorsMM:projectID=FIELD:projectID
OR:1:successorsMM:projectID_Mod=ne
```

#### Tarefa - Mostrar nomes das predecessoras e os projetos nos quais elas estão

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

#### Tarefa - Mostrar os nomes das sucessoras e os projetos nos quais elas estão

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

#### Tarefa - Mostrar data de conclusão projetada das predecessoras

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

#### Tarefa - Mostrar status do progresso das predecessoras

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

#### Tarefa - Mostrar percentual concluído do projeto da predecessora entre projetos

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

![Imagem da tela que mostra a visualização de predecessoras e sucessoras entre projetos](assets/cross-project-predecessors-and-successors.png)


### Tarefa - Iteração mostrando todas as pessoas atribuídas e quem as atribuiu

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![Imagem da tela que mostra todas as pessoas atribuídas e quem as atribuiu](assets/all-assignees-and-requesters.png)

### Tarefa e projeto - Iteração mostrando todos os formulários personalizados em um projeto ou tarefa

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![Imagem da tela que mostra todos os formulários personalizados em um projeto](assets/all-custom-forms-on-a-project.png)


### Projeto - Iteração mostrando todos os contatos primários para problemas resolvíveis na visualização do projeto

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

![Imagem da tela que mostra os contatos primários para problemas resolvíveis](assets/primary-contacts-for-resolvables.png)

### Projeto - Iteração mostrando todos os membros da equipe do projeto

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

![Imagem da tela que mostra todos os membros da equipe do projeto](assets/all-project-team-members.png)

### Projeto - Iteração mostrando a entryDate de todos os problemas resolvíveis de um projeto

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

![Imagem de tela mostrando a entryDate de todos os problemas resolvíveis de um projeto](assets/resolvables-entry-date.png)

### Projeto - Mostra o grupo inicial do solicitante original do projeto

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Imagem de tela mostrando o grupo inicial do solicitante do projeto](assets/requestor-home-group.png)

### Projeto - Mostra se o projeto é uma fila de solicitações

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

![Imagem de tela mostrando se o projeto é uma fila de solicitações](assets/project-is-a-request-queue.png)

### Problema - Iteração mostrando todos os membros da equipe do projeto resolutivo

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

![Imagem de tela mostrando todos os membros da equipe do projeto resolutivo](assets/all-resolve-project-team-members.png)

### Problema – Iteração mostrando todas as equipes do contato principal do problema

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

![Imagem de tela mostrando todas as equipes de contato principais](assets/all-primary-contact-teams.png)

### Documento - Iteração mostrando pasta em um relatório de documento

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![Imagem de tela mostrando a pasta no relatório de um documento](assets/folder-in-a-document-report.png)

### Documento - Iteração mostrando a pasta principal em um relatório de documento

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![Imagem de tela mostrando a pasta principal em um relatório de documento](assets/parent-folder-in-a-document-report.png)

### Documento - Datas de aprovação do documento

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

![Imagem de tela mostrando a visualização das datas de aprovação do documento](assets/document-approval-dates.png)

### Aprovações de revisões

#### Aprovação de prova - Mostrar nome do projeto

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

#### Aprovação de prova - Mostrar nome da tarefa

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Imagem de tela mostrando o projeto e a tarefa de uma aprovação de prova](assets/proof-approval-project-and-task.png)
