---
title: Prática recomendada - Planejamento e gerenciamento do cronograma
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre como configurar, gerenciar e usar linhas do tempo do projeto no Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
kt: 10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Prática recomendada - Planejamento e gerenciamento do cronograma

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de gerenciamento e planejamento de linha do tempo

* Todos os projetos concluídos devem ter um status que reflita que estão concluídos.

* Ao copiar um projeto, defina o status do novo projeto como Planejamento.

* Faça com que os usuários registrem o tempo real gasto em tarefas para que você possa comparar as horas reais às horas planejadas.

* Use as durações da tarefa e os antecessores quando possível para criar e atualizar uma linha do tempo do projeto, em vez de selecionar datas específicas de início e conclusão.

* Solicite aos usuários que atualizem seus status de tarefa, o percentual de conclusão e as horas reais a cada dia (ou em uma programação definida a cada semana).

* Defina o status do projeto como Planejamento ao atualizar o plano do projeto para impedir que as notificações sejam enviadas automaticamente quando alterações forem feitas.

* Remova usuários da equipe do projeto que não recebem trabalho no projeto.

* Coloque Métricas de projeto na parte superior do menu do painel esquerdo para usuários que usam o Workfront principalmente para exibir dados.


</br>
</br>


## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Todos os projetos concluídos devem ter um status que reflita que estão concluídos.


**Veja o porquê**

Garantir que todos os projetos concluídos tenham um status Concluído (ou equivalente) manterá a instância do Workfront limpa e atualizada. Ao manter os status do projeto atualizados e fechá-los, os usuários podem facilmente saber qual trabalho já foi realizado, para que possam se concentrar em prioridades ativas. Também garante a precisão dos dados dos relatórios sobre projetos, tarefas, recursos, etc.


</br>
</br>

**Prática recomendada**

Ao copiar um projeto, defina o status do novo projeto como Planejamento.

**Veja o porquê**

O status de Planejamento (ou equivalente) impede que as notificações do Workfront sobre atribuições, alterações na linha do tempo etc. sejam enviadas antes que o projeto esteja pronto. Ao copiar um projeto, uma caixa de diálogo com opções de projeto será exibida; altere o status aqui, enquanto ajuste outras opções para que os dados não copiem do projeto original para a versão copiada.

</br>
</br>

**Prática recomendada**

Faça com que os usuários registrem o tempo real gasto em tarefas para que você possa comparar as horas reais às horas planejadas.


**Veja o porquê**

Saber quanto tempo leva o trabalho da tarefa significa que você pode atualizar os modelos de projeto para ter mais precisão no planejamento de projetos futuros. Também significa que as estimativas de recursos, usando as ferramentas de gerenciamento de recursos da Workfront, são mais precisas.

</br>
</br>

**Prática recomendada**

Use as durações da tarefa e os antecessores quando possível para criar e atualizar uma linha do tempo do projeto, em vez de selecionar datas específicas de início e conclusão.

**Veja o porquê**

O uso de durações e antecessores juntamente com restrições flexíveis de tarefa (o mais rápido possível e o mais tarde possível) permite alterações automáticas da data da linha do tempo que &quot;em cascata&quot; por meio do plano de projeto. Por exemplo, quando a duração de uma tarefa aumenta em um dia, isso altera a data de conclusão planejada da tarefa, que por sua vez altera as datas de conclusão das tarefas a seguir.

Selecionar datas específicas de início e conclusão de tarefas altera a restrição da tarefa para uma que &quot;bloqueia&quot; a data (Deve iniciar em, Deve terminar em, Datas fixas), o que significa que você precisa fazer algumas atualizações de data da linha do tempo manualmente.

</br>
</br>


**Prática recomendada**

Solicite aos usuários que atualizem seus status de tarefa, o percentual de conclusão e as horas reais a cada dia (ou em uma programação definida a cada semana).

**Veja o porquê**

Os relatórios no Workfront são tão precisos quanto os dados inseridos no Workfront. Quando as informações que indicam o progresso do trabalho, como status e porcentagem concluída, não são atualizadas regularmente, os relatórios que mostram o progresso do trabalho não serão precisos. A atualização diária proporciona a maior precisão possível nos dados de relatório em tempo real.


O status da tarefa também é usado para informar aos usuários quando o trabalho anterior foi concluído e suas novas tarefas podem começar. Quando o status da tarefa não é alterado para refletir o progresso real no item de trabalho, o Workfront não pode enviar as notificações apropriadas.

</br>
</br>

**Prática recomendada**

Defina o status do projeto como Planejamento ao atualizar o plano do projeto para impedir que as notificações sejam enviadas automaticamente quando alterações forem feitas.

**Veja o porquê**

As alterações no plano de projeto podem gerar várias notificações como atribuições de tarefa, datas de início e conclusão planejadas e outras configurações são alteradas. Isso pode causar interrupções para os usuários e confusão sobre atribuições adequadas, prazos etc.

O status de Planejamento informa ao Workfront para não enviar notificações sobre o projeto aos membros da equipe do projeto (os usuários atribuíram tarefas/problemas ou outros com acesso ao projeto) porque o plano do projeto ainda está sendo desenvolvido ou o projeto ainda não está pronto para ser ativado. Quando as alterações forem concluídas, altere o status do projeto de volta para Current (Atual) e as notificações serão enviadas. Seguir este processo ajuda a minimizar a quantidade de notificações que os usuários recebem.

</br>
</br>

**Prática recomendada**

Remova usuários da equipe do projeto que não recebem trabalho no projeto.


**Veja o porquê**

Quando você atribui uma tarefa ou um problema a alguém em um projeto, o que adiciona o usuário à lista da equipe do projeto nas seções Agendamento e Pessoas do projeto. No entanto, eles permanecem na lista da equipe do projeto mesmo que você os tenha removido da atribuição. Isso pode causar confusão para o usuário, pois como parte da equipe do projeto, ele recebe notificações sobre a atividade no projeto e vê o projeto na lista Projetos em que estou.


Além disso, os membros da equipe do projeto recebem permissões para o projeto e suas tarefas, problemas e documentos. Isso pode fazer com que os usuários tenham acesso aos itens no Workfront que não precisam ou que não deveriam ter.

</br>
</br>

**Prática recomendada**

Coloque Métricas de projeto na parte superior do menu do painel esquerdo para usuários que usam o Workfront principalmente para exibir dados.

**Veja o porquê**

A maioria dos líderes, executivos e outros usuários que não gerenciam projetos ou não realizam atribuições de tarefas apreciariam ver esse nível de métricas do projeto quando abrem um projeto pela primeira vez. Use um modelo de layout para mover Métricas de projeto para a parte superior do menu do painel esquerdo em uma página de projeto para tornar mais visível e fácil o acesso dos usuários.
