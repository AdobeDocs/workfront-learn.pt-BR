---
title: Criar uma equipe Kanban
description: Saiba como criar um grupo Kanban e determinar configurações para o grupo.
feature: Agile
role: Admin, Leader, User
level: Intermediate
jira: KT-10881
thumbnail: create-kanban-team.png
exl-id: 01573905-514d-4df6-b2b6-1c92585e56fc
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Criar uma equipe Kanban

A Equipe de marketing criativo já usa o Scrum há algum tempo. Eles apreciam o ambiente flexível de uma equipe ágil, mas estão tendo dificuldade em vincular histórias a um período específico devido à frequência com que as prioridades mudam para sua equipe.

Eles têm uma alternativa para Scrum. Chama-se Kanban.

Kanban trabalha para equipes que não querem definir no que estão trabalhando dentro do período exigido por uma iteração baseada em Scrum. Em vez disso, o Kanban permite que as equipes trabalhem continuamente em seu backlog.

Vamos mudar a Equipe de marketing criativo de uma equipe Scrum para uma equipe Kanban [1]. Faça esta alteração na seção Agile das Configurações do grupo.

Depois de alterar a metodologia, é necessário especificar quantas histórias uma equipe Kanban pode ter por vez em cada coluna ajustando o &quot;Limite de WIP&quot;. [2]. WIP significa Trabalho em andamento. O número que você escolher para colocar aqui depende de quantos itens ativos a equipe pode lidar. Ele será exibido no storyboard da equipe para ajudar a lembrá-los de que estão superalocados ou não. Você (e qualquer membro da equipe com direitos de edição) também pode alterar o limite de WIP diretamente do storyboard.

![Página de configurações da equipe](assets/teamspage-01.png)

Observe que você pode arrastar e soltar as colunas de status para colocá-las na ordem que gostaria que estivessem.

![Página de configurações da equipe](assets/teamspage-02.png)

As equipes Kanban também podem optar por ter a próxima história no backlog automaticamente exibida no storyboard quando uma história é concluída [ver número 3 na imagem superior]. Isso ajudará as equipes que preferem um ciclo de trabalho contínuo.


A imagem abaixo mostra como se parece quando uma nova história aparece automaticamente no storyboard quando uma história é concluída.

![Página de configurações da equipe](assets/teamspage-03.png)

Para ajudar a gerenciar o seu trabalho concluído com mais eficiência, as histórias permanecem no quadro por 14 dias por padrão.

![Página de configurações da equipe](assets/teampage-04.png)

Se necessário, esta configuração pode ser ajustada para entre 1 e 30 dias na janela de configurações do grupo.

Lembre-se de que, embora essa seja uma metodologia diferente, ainda é importante, ao trabalhar em um ambiente ágil, limpar continuamente o backlog discutindo os requisitos da história e ajustando a prioridade da história. Sempre que quiser priorizar novamente o backlog, mova uma guia para a guia Backlog para reorganizá-lo.
