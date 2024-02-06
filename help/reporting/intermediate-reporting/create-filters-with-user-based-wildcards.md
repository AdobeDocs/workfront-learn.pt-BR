---
title: Crie filtros com curingas baseados no usuário
description: Saiba como usar curingas com base no usuário e como criar um filtro com base no usuário conectado.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '340'
ht-degree: 100%

---

# Crie filtros com curingas baseados no usuário

Neste vídeo, você aprenderá a:

* Entenda por que usar curingas
* Crie um filtro com um curinga baseado no usuário

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>Use origem e nome do campo Usuários atribuídos >> ID, quando criar filtros que exibam uma informação de atribuição de tarefa ou problema.  Essa opção analisa todos os usuários atribuídos à tarefa ou problema, não apenas o “proprietário” ou responsável principal.

>[!TIP]
>
>Use $$USER.ID (em vez do seu nome) mesmo ao criar filtros para você mesmo. Dessa forma, se alguém vir um filtro que você está executando e disser “compartilhe isso comigo”, o filtro já está configurado para que cada pessoa que o utilizar veja as próprias informações.

>[!TIP]
>
>Você sempre deve usar o qualificador de filtro “Igual” ao usar curingas com base no usuário.

## Atividade

Você tem um pouco de tempo extra esta semana, então quer ver se há alguém em sua equipe que poderia precisar de ajuda nas tarefas. Crie um filtro de tarefas para encontrar tarefas para esta semana que ainda não foram concluídas.

## Responder

Você é incrível por ajudar seus colegas de equipe! Com o filtro configurado como a imagem abaixo, você encontrará tarefas:

* Que não foram concluídas (o que significa que elas não têm um status [!UICONTROL Concluído] ou que equivalha a [!UICONTROL Concluído]);
* Que estejam em projetos com status [!UICONTROL Atual] (afinal, você não quer encontrar tarefas para projetos que ainda não foram lançados);
* Que estejam atribuídas a alguém da sua equipe interna, conforme definido nas configurações de equipe do Workfront;
* E que tenham uma data de conclusão para esta semana (esta regra usou o filtro de data pré-construído para definir “esta semana”).

![Uma imagem da tela para criar um filtro de tarefa com um curinga baseado no usuário](assets/user-wildcard-exercise-answer.png)

Pode ser necessário adicionar alguns filtros adicionais se precisar limitar um pouco mais a lista. Por exemplo, você pode querer adicionar uma regra de filtro que analise um programa ou portfólio específico no qual sua equipe trabalha.
