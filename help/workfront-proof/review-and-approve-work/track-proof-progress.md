---
title: Acompanhar progresso da prova
description: Aprenda a usar os indicadores [!UICONTROL EACD], o progresso da prova e os relatórios para acompanhar o andamento de uma prova no  [!DNL &#x200B; Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 8ad86921177da189503211635116146e886dbd17
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 64%

---

# Acompanhar progresso da prova

Como gerente de projeto, gerente de prova ou outra parte interessada no processo de revisão e aprovação, convém acompanhar o progresso de suas provas. Isso é possível por meio dos **indicadores de progresso de prova** integrados do [!DNL Workfront's], disponíveis na página [!UICONTROL Documentos], ou por meio de relatórios personalizados.

Para visualizar o progresso da prova no [!DNL Workfront], você deve ter uma licença de Plano, Trabalho ou Revisão e ser um usuário de revisão. Se você não tem certeza de que o perfil do [!DNL Workfront] atende a esses requisitos, verifique com o administrador do sistema de comprovação em sua organização.

## Acompanhe o progresso da prova com indicadores [!UICONTROL EACD] e o status da prova

Obtenha uma visão de alto nível de como a prova está progredindo no processo de revisão e aprovação usando os ícones [!UICONTROL EACD] da lista de [!UICONTROL Documentos]. Esses ícones indicam ações específicas realizadas na prova.

![Imagem da lista de [!UICONTROL Documentos] em um projeto do [!DNL &#x200B; Workfront] com os ícones [!UICONTROL EACD] destacados.](assets/manage-proofs-socd.png)

Os ícones indicam o trabalho feito em uma prova desde o momento em que você a envia para os destinatários até o momento em que eles tomam uma decisão sobre a prova.

* **E -** A prova foi enviada aos destinatários.
* **A -** A prova foi aberta.
* **C -** Foram feitos comentários na prova.
* **D -** Uma decisão foi tomada na prova (aprovada, rejeitada etc.).

As cores indicam se a ação foi concluída ou não.

* **Branco —** A etapa ainda não aconteceu.
* **Verde -** A etapa foi concluída.
* **Laranja —** O prazo de prova é de 24 horas e a etapa não ocorreu.
* **Vermelho —** O prazo de prova já passou e a etapa não ocorreu.

O [!UICONTROL SOCD] na lista [!UICONTROL Documentos], no painel de resumo ou nos [!UICONTROL Detalhes do Documento], é um resumo de alto nível do progresso da prova. O [!DNL Workfront] configura isso com base no destinatário que está &quot;mais atrasado&quot; no processo de prova.

Por exemplo, se houver três revisores ou aprovadores e apenas dois analisaram a prova e fizeram comentários, então os ícones [!UICONTROL EACD] mostrarão que a prova foi enviada ([!UICONTROL E]) e aberta ([!UICONTROL A]), mas não que foram feitos comentários ([!UICONTROL C]).

**Depois que uma decisão final** (por exemplo, Aprovada ou Rejeitada) é tomada em uma prova, todos os indicadores SOCD podem aparecer em verde para os usuários nesse estágio, mesmo se ações individuais (como abrir a prova ou fazer comentários) não tiverem sido executadas. Esse é um comportamento em todo o sistema projetado para refletir a conclusão geral do estágio, não o engajamento individual.

**Antes de uma decisão ser registrada**, cada indicador SOCD reflete a atividade real do usuário (por exemplo, branco se nenhuma ação foi tomada, verde se a ação foi concluída). Após a decisão, o sistema assume a conclusão do workflow e atualiza todos os indicadores adequadamente.

Se quiser saber o que cada destinatário individual da prova está fazendo, abra o fluxo de trabalho da prova. O progresso geral da prova fica localizado na parte superior da janela. Cada estágio possui seu próprio indicador de progresso na barra cinza.  E ao lado de cada usuário está o progresso de cada indivíduo.

![Imagem da seção [!UICONTROL Fluxo de trabalho de prova] de um documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Status da prova

O status da prova é baseado no status dos recipients da prova do estágio. O status geral da prova é visível na página [!UICONTROL Documentos], à direita dos indicadores [!UICONTROL EACD], para que você possa saber facilmente se foi tomada uma decisão sobre a prova.

![Uma imagem da lista de [!UICONTROL Documentos] em um projeto do [!DNL &#x200B; Workfront] com o status geral da prova destacado.](assets/manage-proofs-overall-status.png)

Este “status da prova” indica o status geral da prova. Por exemplo, se dois destinatários aprovaram a prova, seus status individuais serão exibidos como [!UICONTROL Aprovada]. No entanto, o terceiro destinatário ainda não tomou uma decisão, portanto, o status dessa pessoa é [!UICONTROL Pendente]. Portanto, o status geral é exibido como [!UICONTROL Pendente].

Se foram configurados status personalizados para sua organização, eles serão usados. Caso contrário, você verá as opções de status padrão de:

* [!UICONTROL Pendente]
* [!UICONTROL Aprovado]
* [!UICONTROL Aprovado com alterações]
* [!UICONTROL Alterações exigidas]
* [!UICONTROL Não é relevante]

Abra a janela do fluxo de trabalho de revisão para ver o status da prova dos destinatários atribuídos às funções de [!UICONTROL Revisor e aprovador] ou [!UICONTROL Aprovador]da prova.

## Relatórios no [!DNL Workfront]

Você também pode aproveitar os recursos de relatórios do [!DNL Workfront's] para acompanhar as provas à medida que elas avançam no processo de revisão e aprovação.

Um relatório de aprovação de prova ajuda a acompanhar as aprovações pendentes para garantir que os prazos sejam cumpridos.

![Imagem de um relatório de aprovação de prova no [!DNL &#x200B; Workfront].](assets/proof-approval-report.png)

Um relatório de versão do documento permite gerenciar e acompanhar versões da prova.

![Imagem de um relatório de versão do documento no [!DNL &#x200B; Workfront].](assets/document-version-report.png)

Recomendamos conversar com o(a) consultor(a) do [!DNL Workfront] para criar relatórios que atendam aos requisitos da sua organização. Alguns dos relatórios exigem conhecimento sobre os relatórios do modo de texto do [!DNL Workfront's].

## Sua vez

Converse com sua equipe ou administrador do sistema de prova para descobrir que tipo de relatório você usará no Workfront para manter os fluxos de trabalho de prova em perfeita execução.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
