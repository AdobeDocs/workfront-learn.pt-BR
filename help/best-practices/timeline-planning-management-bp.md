---
title: 'Prática recomendada: planejamento e gerenciamento de linha do tempo'
description: Explore práticas recomendadas de especialistas do Adobe Workfront sobre como configurar, gerenciar e usar cronogramas de projetos no Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
jira: KT-10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '1110'
ht-degree: 100%

---

# Prática recomendada: planejamento e gerenciamento de linha do tempo

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, você encontrará primeiro uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite revisar as recomendações sem se aprofundar nos detalhes e motivos por trás delas.

A seção “Por que essas práticas são recomendadas?” , encontrada após a lista resumida, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta ou recurso que você deve considerar implementar na sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de planejamento e gerenciamento de linha do tempo

* Todos os projetos concluídos devem ter um status que reflita que estão concluídos.

* Ao copiar um projeto, defina o status do novo projeto como Planejamento.

* Faça com que os usuários registrem o tempo real gasto em tarefas para que você possa comparar as horas efetivas com as horas planejadas.

* Use durações de tarefas e predecessores quando possível para construir e atualizar um cronograma de projeto, em vez de selecionar datas específicas de início e conclusão.

* Peça aos usuários para atualizarem seus próprios status de tarefas, percentual concluído e horas efetivas todos os dias (ou em uma programação definida a cada semana).

* Defina o status do projeto como Planejamento ao atualizar o plano do projeto para evitar que notificações sejam enviadas automaticamente à medida que alterações são feitas.

* Remova usuários da equipe do projeto que não tenham trabalho atribuído no projeto.

* Coloque Métricas do projeto na parte superior do menu do painel esquerdo para usuários que usam o Workfront principalmente para visualizar dados.


</br>
</br>


## Por que essas práticas são recomendadas?

**Prática recomendada**

Todos os projetos concluídos devem ter um status que reflita que estão concluídos.


**Entenda o porquê**

Garantir que todos os projetos concluídos tenham o status Concluído (ou equivalente) mantém sua instância do Workfront limpa e atualizada. Ao manter os status dos projetos atualizados e encerrá-los, os usuários podem facilmente saber qual trabalho já foi concluído para que possam se concentrar nas prioridades ativas. Também garante que os dados do relatório sobre projetos, tarefas, recursos etc., sejam precisos.


</br>
</br>

**Prática recomendada**

Ao copiar um projeto, defina o status do novo projeto como Planejamento.

**Entenda o porquê**

O status Planejamento (ou equivalente) evita que notificações do Workfront sobre atribuições, alterações no cronograma etc., sejam enviadas antes que o projeto esteja pronto. Ao copiar um projeto, aparecerá uma caixa de diálogo com opções de projeto; altere o status aqui, enquanto ajusta outras opções para que os dados não sejam copiados do projeto original para a versão copiada.

</br>
</br>

**Prática recomendada**

Faça com que os usuários registrem o tempo real gasto em tarefas para que você possa comparar as horas efetivas com as horas planejadas.


**Entenda o porquê**

Saber quanto tempo leva o trabalho da tarefa significa que você pode atualizar os modelos de projeto para obter melhor precisão no planejamento de projetos futuros. Isso também significa que as estimativas de recursos, usando as ferramentas de gerenciamento de recursos do Workfront, são mais precisas.

</br>
</br>

**Prática recomendada**

Use durações de tarefas e predecessores quando possível para construir e atualizar um cronograma de projeto, em vez de selecionar datas específicas de início e conclusão.

**Entenda o porquê**

O uso de durações e predecessores em conjunto com restrições de tarefas flexíveis (O mais breve possível e O mais tarde possível) permite alterações automáticas de datas no cronograma que “se espalham” pelo plano do projeto. Por exemplo, quando a duração de uma tarefa aumenta um dia, isso altera a data de conclusão planejada da tarefa, que por sua vez altera as datas de conclusão das tarefas seguintes.

A seleção de datas específicas de início e conclusão para tarefas altera a restrição da tarefa para uma que “bloqueie” a data (Deve começar em, Deve terminar em, Datas fixas), o que significa que você terá que fazer algumas atualizações de datas na linha do tempo manualmente.

</br>
</br>


**Prática recomendada**

Peça aos usuários para atualizarem seus próprios status de tarefas, percentual concluído e horas efetivas todos os dias (ou em uma programação definida a cada semana).

**Entenda o porquê**

Os relatórios no Workfront são tão precisos quanto os dados inseridos no Workfront. Quando as informações que indicam o progresso do trabalho, como o status e o percentual concluído, não são atualizadas regularmente, os relatórios que mostram o progresso do trabalho não serão precisos. A atualização diária proporciona maior precisão nos dados de relatórios em tempo real.


O status da tarefa também é usado para informar aos usuários quando o trabalho anterior foi concluído e suas novas tarefas podem começar. Quando o status da tarefa não é alterado para refletir o progresso real no item de trabalho, o Workfront não pode enviar as notificações apropriadas.

</br>
</br>

**Prática recomendada**

Defina o status do projeto como Planejamento ao atualizar o plano do projeto para evitar que notificações sejam enviadas automaticamente à medida que alterações são feitas.

**Entenda o porquê**

As alterações no plano do projeto podem gerar diversas notificações à medida que atribuições de tarefas, datas planejadas de início e conclusão e outras configurações são alteradas. Isso pode atrapalhar os usuários e causar confusão sobre atribuições corretas, prazos etc.

O status de planejamento informa ao Workfront para não enviar notificações sobre o projeto aos membros da equipe do projeto (usuários atribuídos a tarefas/problemas ou outros com acesso ao projeto) porque o plano do projeto ainda está sendo desenvolvido ou o projeto simplesmente não está pronto para ser executado ainda. Assim que as alterações forem concluídas, altere o status do projeto de volta para Atual e as notificações serão enviadas. Seguir esse processo ajuda a minimizar a quantidade de notificações que os usuários recebem.

</br>
</br>

**Prática recomendada**

Remova usuários da equipe do projeto que não tenham trabalho atribuído no projeto.


**Veja o porquê**

Quando você atribui a alguém uma tarefa ou um problema em um projeto, isso adiciona o usuário à lista da equipe do projeto nas seções Agendamento e Pessoas do projeto. No entanto, eles permanecem na lista da equipe do projeto mesmo que você os tenha removido da atribuição. Isso pode causar confusão para os usuários, pois, como parte da equipe do projeto, eles recebem notificações sobre a atividade no projeto e o veem na lista Projetos em que estou.


Além disso, os membros da equipe recebem permissões para o projeto, com as respectivas tarefas, problemas e documentos. Isso pode fazer com que os usuários tenham acesso a itens no Workfront que não precisam ou não deveriam ter.

</br>
</br>

**Prática recomendada**

Coloque Métricas do projeto na parte superior do menu do painel esquerdo para usuários que usam o Workfront principalmente para visualizar dados.

**Veja o porquê**

A maioria dos líderes, executivos e outros usuários que não gerenciam projetos ou cumprem atribuições de tarefas gostariam de ver esse nível de métricas de projeto quando abrem um projeto pela primeira vez. Use um modelo de layout para mover as Métricas do projeto para a parte superior do menu do painel esquerdo numa página do projeto para torná-las mais visíveis e fáceis de acessar para os usuários.
