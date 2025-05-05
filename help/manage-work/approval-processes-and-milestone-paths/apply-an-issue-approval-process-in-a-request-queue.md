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
last-substantial-update: 2025-03-26T00:00:00Z
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: 3fc3a58c829769ca06ffb93971ac75516dfbd5f2
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 5%

---

# Aplicar um processo de aprovação de problema em uma fila de solicitações

>[!PREREQUISITES]
>
>* [Criar um fluxo de solicitações](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Criar um processo de aprovação global e de uso único](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


O vídeo explica o processo de aplicar um processo de aprovação padrão ao criar uma fila de solicitações. &#x200B; Quando uma solicitação é criada, ela começa com o status &quot;Novo - Aprovação pendente&quot; e uma notificação de aprovação é enviada ao aprovador designado. &#x200B; Se aprovado, o status muda para &quot;Novo&quot;, permitindo que os indivíduos designados comecem a trabalhar. &#x200B; Se rejeitado, o status pode reverter incorretamente para &quot;Novo&quot; devido a um erro comum na configuração do processo de aprovação. &#x200B;
O vídeo destaca que o processo de aprovação é acionado quando o status é definido como &quot;Novo&quot;, que é o padrão para novas solicitações. &#x200B; Se for rejeitada, o sistema assumirá como padrão a alteração do status para o anterior, o que não é ideal para novas solicitações. &#x200B; Em vez disso, um status diferente, como &quot;Não resolverá&quot;, deve ser escolhido. &#x200B; O vídeo também observa que não há status &quot;Rejeitado&quot; fornecido por padrão, mas um administrador do sistema pode criar um, se necessário. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455029/?quality=12&learn=on&enablevpops&captions=por_br)

## Principais pontos

* **Processo de aprovação padrão:** Ao criar uma fila de solicitações, você pode aplicar um processo de aprovação padrão que atribui automaticamente um fluxo de trabalho de aprovação a cada solicitação.
* **Alterações de Status Após a Aprovação:** as solicitações aprovadas alteram seu status de &quot;Novo - Aprovação pendente&quot; para &quot;Novo&quot;, permitindo que os indivíduos atribuídos comecem a trabalhar nelas.
* **Erro Comum no Tratamento de Rejeição:** Se uma solicitação for rejeitada, o status será revertido para &quot;Novo&quot; devido a uma configuração de sistema padrão no processo de aprovação.
* **Status recomendado para Solicitações Rejeitadas:** Em vez de reverter para o status anterior (&quot;Novo&quot;), é melhor escolher um status diferente; por exemplo, &quot;Não Resolverá&quot;, para evitar confusão.
* **Opções de Status Personalizado:** Não há status &quot;Rejeitado&quot; fornecido por padrão, mas um administrador do sistema pode criar um, se necessário, para maior clareza no processo de aprovação.


## Tutoriais recomendados sobre este tópico

* [Delegar tarefas, problemas e aprovações](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Entenda os processos de aprovação específicos do grupo](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Criar um fluxo de solicitação](/help/manage-work/request-queues/create-a-request-flow.md)
* [Criar um processo de aprovação global e de uso único](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
