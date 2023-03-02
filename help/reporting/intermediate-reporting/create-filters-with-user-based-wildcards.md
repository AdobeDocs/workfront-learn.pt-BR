---
title: Criar filtros com curingas baseados no usuário
description: Saiba como usar curingas com base no usuário e como criar um filtro com base no usuário conectado.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Criar filtros com curingas baseados no usuário

Neste vídeo, você aprenderá a:

* Entender por que usar curingas
* Criar um filtro com um curinga baseado no usuário

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12)

>[!TIP]
>
>Use a origem e o nome do campo Usuários de atribuição >> ID ao criar filtros que observam informações de atribuição de tarefas ou problemas.  Essa opção analisa todos os usuários atribuídos à tarefa ou problema, não apenas o &quot;proprietário&quot; ou o responsável principal.

>[!TIP]
>
>Use o $$USER.ID (em vez do seu nome) mesmo ao criar filtros para si mesmo. Dessa forma, se alguém vir um filtro que você está executando e disser &quot;compartilhe isso comigo&quot;, o filtro já está configurado para que cada pessoa que o usa veja suas próprias informações.

>[!TIP]
>
>Você sempre deve usar o qualificador de filtro Igual ao usar curingas com base no usuário.

## Atividade

Você tem um pouco de tempo extra esta semana, então você quer ver se há alguém na sua equipe que poderia usar alguma assistência em suas tarefas. Crie um filtro de tarefa para encontrar tarefas com vencimento nesta semana que ainda não foram concluídas.

## Resposta

Você é incrível por ajudar seus colegas de equipe! Com o filtro configurado como a imagem abaixo, você encontrará tarefas:

* Que não foram concluídas (o que significa que não têm uma [!UICONTROL Concluído] status ou status que equivale a [!UICONTROL Concluído]);
* Que estejam em projetos com uma [!UICONTROL Atual] status (afinal, você não quer encontrar tarefas para projetos que ainda não foram iniciados);
* Que são atribuídos a alguém da sua equipe inicial, conforme definido pelas configurações da equipe do Workfront;
* E que tenham uma data de conclusão em algum momento desta semana (essa regra usou o filtro de datas pré-criado para definir &quot;esta semana&quot;).

![Uma imagem da tela para criar um filtro de tarefa com um curinga baseado no usuário](assets/user-wildcard-exercise-answer.png)

Talvez seja necessário adicionar alguns filtros adicionais para limitar a lista um pouco mais. Por exemplo, você pode adicionar uma regra de filtro que procura um programa ou portfólio específico do qual sua equipe trabalha.
