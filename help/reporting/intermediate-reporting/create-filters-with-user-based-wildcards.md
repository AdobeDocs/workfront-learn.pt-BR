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
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 48%

---

# Crie filtros com curingas baseados no usuário

Neste vídeo, você aprenderá a:

* Entenda por que usar curingas
* Crie um filtro com um curinga baseado no usuário

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>Use origem e nome do campo Usuários atribuídos >> ID, quando criar filtros que exibam uma informação de atribuição de tarefa ou problema.  Essa opção considera todas as   usuários atribuídos à tarefa ou problema, não apenas o &quot;proprietário&quot; ou o responsável principal.

>[!TIP]
>
>Use $$USER.ID (em vez do seu nome) mesmo ao criar filtros para você mesmo. Dessa forma, se alguém vir um filtro que você está executando e disser &quot;compartilhe isso comigo&quot;, o filtro já está configurado para que cada pessoa que o usa veja suas próprias informações.

>[!TIP]
>
>Você sempre deve usar o qualificador de filtro “Igual” ao usar curingas com base no usuário.


## Criar filtros com atividades de curingas baseadas no usuário

[Clique aqui](/help/assets/create-filters-with-user-based-wildcards-activities.pdf) para baixar um PDF desta página.

### Atividade 1

Você tem um pouco de tempo extra esta semana, então você quer ver se há alguém na sua equipe que poderia usar alguma assistência com suas tarefas. Crie um filtro de tarefa para encontrar tarefas com vencimento nesta semana que ainda não foram concluídas.

### Resposta 1

Você é incrível por ajudar seus colegas de equipe! Com o filtro configurado como a imagem abaixo, você encontrará tarefas:

* Que não foram concluídas (o que significa que elas não têm um status de [!UICONTROL Concluído] ou status que equivale a [!UICONTROL Concluído]);
* Que estão em projetos com status [!UICONTROL Atual] (afinal, você não quer encontrar tarefas para projetos que ainda não foram iniciados);
* Que estejam atribuídas a alguém da sua equipe interna, conforme definido nas configurações de equipe do Workfront;
* E que tenham uma data de conclusão em algum momento desta semana (essa regra usou o filtro de datas pré-criado para definir &quot;esta semana&quot;).

![Uma imagem da tela para criar um filtro de tarefa com um curinga baseado no usuário](assets/user-wildcard-exercise-answer.png)

Pode ser necessário adicionar alguns filtros adicionais se precisar limitar um pouco mais a lista. Por exemplo, você pode querer adicionar uma regra de filtro que analise um programa ou portfólio específico no qual sua equipe trabalha.
