---
title: Prática recomendada - Status
description: Explore as recomendações de práticas recomendadas dos especialistas da Adobe Workfront sobre a configuração, gerenciamento e uso dos status do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Prática recomendada - Status

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para status

* Ao renomear os status padrão do Workfront, mantenha a finalidade original do status igual.

* Se você criar um status de projeto personalizado para Cancelado, equipare o status a Inativo.

* Reduza ao mínimo os status personalizados globais.

* Não use status de projeto no lugar de tarefas para indicar a progressão de um projeto.


</br>
</br>



## Por que essas práticas recomendadas?

**Prática recomendada**

Ao renomear os status padrão do Workfront, mantenha a finalidade original do status igual.



**Veja o porquê**

Algumas ações no Workfront são acionadas pelos status padrão do sistema. Alterar a intenção de um status pode afetar como o Workfront se comporta em determinadas situações, afetar os relatórios etc.



Por exemplo, o status padrão de Concluído da tarefa informa ao Workfront para alterar o percentual concluído de uma tarefa para 100%. O status Concluído também permite que a Workfront saiba que o trabalho em tarefas dependentes pode começar. Se você alterou o nome do status para Aguardando, para indicar que um trabalho em uma tarefa está pausado, o Workfront pensará que a tarefa foi concluída e iniciará as próximas etapas no projeto.

</br>
</br>



**Prática recomendada**

Se você criar um status de projeto personalizado para Cancelado, equipare o status a Inativo.



**Veja o porquê**

Se você equiparar Cancelado a Concluído, não poderá usar o status para cancelar um projeto a menos que todas as tarefas estejam marcadas como concluídas e todos os problemas estejam fechados. Porém, se você igualar Cancelado a Desativado, poderá cancelar o projeto sem alterar nada no registro histórico.


</br>
</br>

**Prática recomendada**

Reduza ao mínimo os status personalizados globais.



**Veja o porquê**

Menos é mais. Além de criar manutenção desnecessária, muitos status personalizados geram confusão, especialmente ao trabalhar em projetos multifuncionais. Em vez disso, torne específico o grupo de status personalizados. Isso mantém seu ambiente do Workfront mais limpo e melhor posicionado para expansão para outros grupos no futuro. Trabalhe com seu comitê de governança/supervisão e as partes interessadas para identificar os status que os grupos de sua organização precisam usar.


</br>
</br>

**Prática recomendada**

Não use status de projeto no lugar de tarefas para indicar a progressão de um projeto.



**Veja o porquê**

Mantenha os status do projeto simples para indicar fases de alto nível da progressão, como Planejamento, Atual, Concluído etc. Permita que as tarefas, os status das tarefas e o percentual de conclusão da tarefa informem como o trabalho está progredindo no geral no projeto. Esses indicadores de nível de tarefa se acumulam na porcentagem concluída do projeto, na condição do projeto e no status do progresso do projeto. Todos esses indicadores são melhores e mais precisos para a progressão do projeto do que o status do projeto. Além disso, essas informações no nível de tarefa fornecem relatórios melhores para o projeto.
