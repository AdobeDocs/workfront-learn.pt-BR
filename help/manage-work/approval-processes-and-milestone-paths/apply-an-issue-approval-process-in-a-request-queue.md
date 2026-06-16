---
title: Aplicar um processo de aprovação de problema em uma fila de solicitações
description: Implemente um processo de aprovação padrão para simplificar os workflows de solicitação, garantindo que as solicitações aprovadas alterem seu status adequadamente para "Novo". Corrija a confusão de solicitações rejeitadas ao selecionar uma alteração de status para "Não resolverá".
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: '2025-03-26T00:00:00.000Z'
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T15:58:59.618Z'
source-git-commit: f0f541bf3fd6db69e6d813cf81456a5df6848d49
workflow-type: tm+mt
source-wordcount: 291
ht-degree: 24%

---

# Aplicar um processo de aprovação de problema em uma fila de solicitações

>[!PREREQUISITES]
>
>* [Criar um fluxo de solicitação no Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Criar e gerenciar processos de aprovação](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


O vídeo explica o processo de aplicar um processo de aprovação padrão ao criar uma fila de solicitações. &#x200B; Quando uma solicitação é criada, ela começa com o status &quot;Novo - Aprovação pendente&quot; e uma notificação de aprovação é enviada ao aprovador designado. &#x200B; Se aprovada, o status muda para &quot;Novo&quot;, permitindo que os indivíduos atribuídos comecem a trabalhar. &#x200B; Se rejeitado, o status pode reverter incorretamente para &quot;Novo&quot; devido a um erro comum na configuração do processo de aprovação. &#x200B;
O vídeo destaca que o processo de aprovação é acionado quando o status é definido como &quot;Novo&quot;, que é o padrão para novas solicitações. &#x200B; Se for rejeitada, o sistema assumirá como padrão a alteração do status para o status anterior, o que não é ideal para novas solicitações. &#x200B; Em vez disso, um status diferente, como &quot;Não resolverá&quot;, deve ser escolhido. &#x200B; O vídeo também observa que não há status &quot;Rejeitado&quot; fornecido por padrão, mas um administrador do sistema pode criar um, se necessário. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops=1)

## Principais lições

* **Processo de aprovação padrão:** Ao criar uma fila de solicitações, você pode aplicar um processo de aprovação padrão que atribui automaticamente um fluxo de trabalho de aprovação a cada solicitação.
* **Alterações de Status Após a Aprovação:** as solicitações aprovadas alteram seu status de &quot;Novo - Aprovação pendente&quot; para &quot;Novo&quot;, permitindo que os indivíduos atribuídos comecem a trabalhar nelas.
* **Erro Comum no Tratamento de Rejeição:** Se uma solicitação for rejeitada, o status será revertido para &quot;Novo&quot; devido a uma configuração de sistema padrão no processo de aprovação.
* **Status recomendado para Solicitações Rejeitadas:** Em vez de reverter para o status anterior (&quot;Novo&quot;), é melhor escolher um status diferente; por exemplo, &quot;Não Resolverá&quot;, para evitar confusão.
* **Opções de Status Personalizado:** Não há status &quot;Rejeitado&quot; fornecido por padrão, mas um administrador do sistema pode criar um, se necessário, para maior clareza no processo de aprovação.


## Tutoriais recomendados sobre este tópico

* [Delegar tarefas, problemas e aprovações efetivamente](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Entenda os processos de aprovação específicos do grupo](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Criar um fluxo de solicitação no Workfront](/help/manage-work/request-queues/create-a-request-flow.md)
* [Criar e gerenciar processos de aprovação](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
