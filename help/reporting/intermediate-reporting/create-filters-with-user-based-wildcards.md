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
last-substantial-update: '2025-06-26T00:00:00.000Z'
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2: id: ceb4d94a-32ed-4fea-9724-1339d684b0bc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:58:26.659Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 88%

---

# Crie filtros com curingas baseados no usuário

Neste vídeo, você aprenderá a:

* Entenda por que usar curingas
* Crie um filtro com um curinga baseado no usuário

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on&enablevpops=0)

>[!TIP]
>
>Use origem e nome do campo Usuários atribuídos >> ID, quando criar filtros que exibam uma informação de atribuição de tarefa ou problema.  Essa opção analisa todos os usuários atribuídos à tarefa ou problema, não apenas o &quot;proprietário&quot; ou o responsável principal.

>[!TIP]
>
>Use $$USER.ID (em vez do seu nome) mesmo ao criar filtros para você mesmo(a). Dessa forma, se alguém vir um filtro que você está executando e solicitar que você o compartilhe, ele já estará configurado para que cada pessoa que o utilizar veja suas próprias informações.

>[!TIP]
>
>Use sempre o qualificador de filtro “Igual” ao usar curingas com base no usuário.


## Atividades “Criar filtros com curingas baseados no usuário”

### Atividade 1

Você tem um tempinho extra esta semana e deseja saber se alguém na sua equipe precisa de ajuda com as tarefas. Crie um filtro de tarefas para encontrar tarefas atribuídas à sua equipe inicial que vencem esta semana e ainda não foram concluídas.

### Resposta 1

Ajudar colegas de equipe é uma bela atitude de sua parte. Com o filtro configurado como na imagem abaixo, você encontrará tarefas:

* Que não foram concluídas (o que significa que elas não têm um status [!UICONTROL Concluído] ou equivalente);
* Que estejam em projetos com status [!UICONTROL Atual] (afinal, você não deseja encontrar tarefas para projetos que ainda não foram iniciados);
* Que estejam atribuídas a alguém da sua equipe interna, conforme definido nas configurações de equipe do Workfront;
* E que tenham uma data de conclusão para esta semana (esta regra usou o filtro de data pré-construído para definir “esta semana”).

![Uma imagem da tela para criar um filtro de tarefa com um curinga baseado no usuário](assets/user-wildcard-exercise-answer.png)

Pode ser necessário adicionar alguns filtros adicionais se precisar limitar um pouco mais a lista. Por exemplo, você pode querer adicionar uma regra de filtro que analise um programa ou portfólio específico no qual sua equipe trabalha.
