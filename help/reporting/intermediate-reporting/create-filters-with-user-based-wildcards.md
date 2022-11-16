---
title: Criar filtros com curingas baseadas em usuário
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
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Criar filtros com curingas baseadas em usuário

Neste vídeo, você aprenderá a:

* Entenda por que usar curingas
* Criar um filtro com um curinga baseado no usuário

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12)

>[!TIP]
>
>Use a fonte e o nome do campo Atribuir usuários > ID ao criar filtros que analisam as informações de atribuição de tarefa ou emissão.  Essa opção considera todos os usuários atribuídos à tarefa ou ocorrência, não apenas o &quot;proprietário&quot; ou o destinatário principal.

>[!TIP]
>
>Use o $$USER.ID (em vez do seu nome) mesmo ao criar filtros para você mesmo. Dessa forma, se alguém vir um filtro que você está executando e disser &quot;compartilhe isso comigo&quot;, o filtro já estará configurado para que cada pessoa usando ele veja suas próprias informações.

>[!TIP]
>
>Você sempre deve usar o qualificador de filtro Equal ao usar curingas com base em usuário.

## Atividade

Você tem um pouco de tempo extra esta semana, então você quer ver se há alguém em sua equipe que possa usar alguma assistência com suas atribuições. Crie um filtro de tarefas para localizar tarefas que vencem esta semana e que não foram concluídas.

## Resposta

Você é incrível por ajudar seus colegas de equipe! Com o filtro configurado como a imagem abaixo, você encontrará tarefas:

* Isso não foi concluído (o que significa que eles não têm um [!UICONTROL Concluído] status ou status que seja igual a [!UICONTROL Concluído]);
* Que estão em projetos com uma [!UICONTROL Atual] status (afinal, você não deseja encontrar tarefas para projetos que ainda não foram iniciados);
* Que são atribuídos a alguém em sua equipe inicial, conforme definido pelas configurações da equipe do Workfront;
* E que têm uma data de conclusão em algum momento desta semana (esta regra usou o filtro de datas pré-criado para definir &quot;esta semana&quot;).

![Uma imagem da tela para criar um filtro de tarefa com um curinga baseado no usuário](assets/user-wildcard-exercise-answer.png)

Talvez seja necessário adicionar alguns filtros adicionais se for necessário limitar um pouco mais a lista. Por exemplo, talvez você queira adicionar uma regra de filtro que analise um programa ou portfólio específico do qual a equipe trabalha.
