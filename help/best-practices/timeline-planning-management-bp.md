---
title: Prática recomendada - Planejamento e gerenciamento de linha do tempo
description: Explore as recomendações de práticas recomendadas dos especialistas da Adobe Workfront sobre a configuração, gerenciamento e uso das linhas do tempo do projeto no Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
jira: KT-10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Prática recomendada - Planejamento e gerenciamento de linha do tempo

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de planejamento e gerenciamento de linha do tempo

* Todos os projetos concluídos devem ter um status que reflita que estão concluídos.

* Ao copiar um projeto, defina o status do novo projeto como Planning.

* Faça com que os usuários registrem o tempo real gasto nas tarefas para que você possa comparar as horas reais com as planejadas.

* Use durações de tarefas e predecessores quando possível para criar e atualizar uma linha do tempo do projeto, em vez de selecionar datas específicas de início e conclusão.

* Solicite aos usuários que atualizem seus status de tarefa, percentual concluído e horas reais a cada dia (ou em uma programação definida a cada semana).

* Defina o status do projeto como Planejamento ao atualizar o plano de projeto para impedir que as notificações sejam enviadas automaticamente à medida que as alterações forem feitas.

* Remova os usuários da equipe de projeto que não recebem trabalho no projeto.

* Coloque Métricas do projeto na parte superior do menu do painel esquerdo para usuários que usam o Workfront principalmente para visualizar dados.


</br>
</br>


## Por que essas práticas recomendadas?

**Prática recomendada**

Todos os projetos concluídos devem ter um status que reflita que estão concluídos.


**Veja o porquê**

Garantir que todos os projetos concluídos tenham um status Concluído (ou equivalente) mantém a instância do Workfront limpa e atualizada. Ao manter os status dos projetos atualizados e fechá-los, os usuários podem saber facilmente qual trabalho já foi realizado para que possam se concentrar em prioridades ativas. Também garante a precisão dos dados de relatório sobre projetos, tarefas, recursos, etc.


</br>
</br>

**Prática recomendada**

Ao copiar um projeto, defina o status do novo projeto como Planning.

**Veja o porquê**

O status do Planejamento (ou equivalente) impede que as notificações do Workfront sobre atribuições, alterações na linha do tempo etc. saiam antes que o projeto esteja pronto. Ao copiar um projeto, uma caixa de diálogo com opções de projeto será exibida; altere o status aqui, enquanto ajusta outras opções para que os dados não sejam copiados do projeto original para a versão copiada.

</br>
</br>

**Prática recomendada**

Faça com que os usuários registrem o tempo real gasto nas tarefas para que você possa comparar as horas reais com as planejadas.


**Veja o porquê**

Saber quanto tempo leva o trabalho da tarefa significa que você pode atualizar modelos de projeto para obter maior precisão no planejamento de projetos futuros. Também significa que as estimativas de recursos, usando as ferramentas de gerenciamento de recursos da Workfront, são mais precisas.

</br>
</br>

**Prática recomendada**

Use durações de tarefas e predecessores quando possível para criar e atualizar uma linha do tempo do projeto, em vez de selecionar datas específicas de início e conclusão.

**Veja o porquê**

Usar durações e predecessores juntamente com restrições flexíveis de tarefa (o mais rápido possível e o mais tarde possível) permite alterações automáticas de data da linha do tempo que &quot;avançam&quot; no plano do projeto. Por exemplo, quando a duração de uma tarefa aumenta em um dia, isso altera a data de conclusão planejada da tarefa, o que, por sua vez, altera as datas de conclusão das tarefas a seguir.

Selecionar datas de início e conclusão específicas para tarefas altera a restrição da tarefa para uma que &quot;bloqueia&quot; a data (Precisa Iniciar em, Precisa Terminar em, Datas Fixas), o que significa que você precisa fazer algumas atualizações de data na linha do tempo manualmente.

</br>
</br>


**Prática recomendada**

Solicite aos usuários que atualizem seus status de tarefa, percentual concluído e horas reais a cada dia (ou em uma programação definida a cada semana).

**Veja o porquê**

Os relatórios no Workfront são tão precisos quanto os dados inseridos no Workfront. Quando as informações que indicam o progresso do trabalho — como status e porcentagem concluída — não são atualizadas regularmente, os relatórios que mostram o progresso do trabalho não serão precisos. A atualização diária fornece a maior precisão nos dados de relatórios em tempo real.


O status da tarefa também é usado para informar aos usuários quando um trabalho anterior foi concluído e suas novas tarefas podem começar. Quando o status da tarefa não é alterado para refletir o progresso real no item de trabalho, o Workfront não pode enviar as notificações apropriadas.

</br>
</br>

**Prática recomendada**

Defina o status do projeto como Planejamento ao atualizar o plano de projeto para impedir que as notificações sejam enviadas automaticamente à medida que as alterações forem feitas.

**Veja o porquê**

As alterações no plano de projeto podem gerar várias notificações à medida que atribuições de tarefas, datas planejadas de início e conclusão e outras configurações são alteradas. Isso pode interromper os usuários e causar confusão sobre atribuições adequadas, prazos etc.

O status do Planejamento informa ao Workfront para não enviar notificações sobre o projeto para membros da equipe do projeto (usuários com tarefas/problemas atribuídos ou outros com acesso ao projeto) porque o plano do projeto ainda está sendo desenvolvido ou o projeto ainda não está pronto para entrar em funcionamento. Quando as alterações forem concluídas, altere o status do projeto novamente para Current (Atual) e as notificações serão enviadas. Seguir esse processo ajuda a minimizar a quantidade de notificações que os usuários recebem.

</br>
</br>

**Prática recomendada**

Remova os usuários da equipe de projeto que não recebem trabalho no projeto.


**Veja o porquê**

Quando você atribui uma tarefa ou um problema a alguém em um projeto, isso adiciona o usuário à lista da equipe do projeto nas seções Agendamento e Pessoas do projeto. No entanto, elas permanecem na lista de equipes do projeto mesmo que você as tenha removido da atribuição. Isso pode causar confusão para o usuário, pois, como parte da equipe do projeto, ele recebe notificações sobre a atividade no projeto e vê o projeto na lista Projetos em que estou.


Além disso, os membros da equipe do projeto obtêm permissões para o projeto e suas tarefas, problemas e documentos. Isso pode fazer com que os usuários tenham acesso a itens na Workfront de que não precisam ou não deveriam ter.

</br>
</br>

**Prática recomendada**

Coloque Métricas do projeto na parte superior do menu do painel esquerdo para usuários que usam o Workfront principalmente para visualizar dados.

**Veja o porquê**

A maioria dos líderes, executivos e outros usuários que não gerenciam projetos ou cumprem atribuições de tarefas apreciariam ver esse nível de métricas do projeto quando abrem um projeto pela primeira vez. Use um modelo de layout para mover Métricas do projeto para a parte superior do menu do painel esquerdo em uma página de projeto, tornando-a mais visível e fácil de ser acessada pelos usuários.
