---
title: Acompanhar progresso da prova
description: Aprenda a usar os indicadores [!UICONTROL EACD], o progresso da prova e os relatórios para acompanhar o andamento de uma prova no  [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '674'
ht-degree: 100%

---

# Acompanhar progresso da prova

Como gerente de projeto, gerente de provas ou outra parte interessada no processo de revisão e aprovação, você deseja acompanhar o progresso das provas. Isso é possível por meio dos **indicadores de progresso de prova** integrados do [!DNL Workfront’s], disponíveis na página [!UICONTROL Documentos], ou por meio de relatórios personalizados.

Para visualizar o progresso da prova no [!DNL Workfront], você deve ter uma licença de Plano, Trabalho ou Revisão e ser um usuário de revisão. Se você não tem certeza de que seu perfil no [!DNL Workfront] atende a esses requisitos, consulte o(a) admin do sistema de revisão da sua organização.

## Acompanhe o progresso da prova com indicadores [!UICONTROL EACD] e o status da prova

Obtenha uma visão de alto nível de como a prova está progredindo no processo de revisão e aprovação usando os ícones [!UICONTROL EACD] da lista de [!UICONTROL Documentos]. Esses ícones indicam ações específicas realizadas na prova.

![Imagem da lista de [!UICONTROL Documentos] em um projeto do [!DNL  Workfront] com os ícones [!UICONTROL EACD] destacados.](assets/manage-proofs-socd.png)

Os ícones indicam o trabalho feito em uma prova desde o momento em que você a envia para os destinatários até o momento em que eles tomam uma decisão sobre a prova.

* **E -** A prova foi enviada aos destinatários.
* **A -** A prova foi aberta.
* **C -** Foram feitos comentários na prova.
* **D -** Uma decisão foi tomada na prova (aprovada, rejeitada etc.).

As cores indicam se a ação foi concluída ou não.

* **Branco -** A etapa ainda não aconteceu.
* **Verde -** A etapa foi concluída.
* **Laranja -** O prazo da prova termina em 24 horas e a etapa ainda não aconteceu.
* **Vermelho -** O prazo da prova já passou e a etapa não aconteceu.

O [!UICONTROL EACD] na lista de [!UICONTROL Documentos], no painel de resumo ou em [!UICONTROL Detalhes do documento], é um resumo geral do progresso da prova. O [!DNL Workfront] configura isso com base no destinatário que está “mais atrasado” no processo de revisão.

Por exemplo, se houver três revisores ou aprovadores e apenas dois analisaram a prova e fizeram comentários, então os ícones [!UICONTROL EACD] mostrarão que a prova foi enviada ([!UICONTROL E]) e aberta ([!UICONTROL A]), mas não que foram feitos comentários ([!UICONTROL C]).

Se quiser saber o que cada destinatário individual da prova está fazendo, abra o fluxo de trabalho da prova. O progresso geral da prova fica localizado na parte superior da janela. Cada estágio possui seu próprio indicador de progresso na barra cinza.  E ao lado de cada usuário está o seu indicador de progresso.

![Imagem da seção [!UICONTROL Fluxo de trabalho de prova] de um documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Status da prova

O status da prova é baseado no status dos destinatários da prova do estágio. O status geral da prova é visível na página [!UICONTROL Documentos], à direita dos indicadores [!UICONTROL EACD], para que você possa saber facilmente se foi tomada uma decisão sobre a prova.

![Uma imagem da lista de [!UICONTROL Documentos] em um projeto do [!DNL  Workfront] com o status geral da prova destacado.](assets/manage-proofs-overall-status.png)

Este “status da prova” indica o status geral da prova. Por exemplo, se dois destinatários aprovaram a prova, seus status individuais serão exibidos como [!UICONTROL Aprovada]. No entanto, o terceiro destinatário ainda não tomou uma decisão, então o status dessa pessoa é exibido como [!UICONTROL Pendente]. Portanto, o status geral é exibido como [!UICONTROL Pendente].

Se foram configurados status personalizados para sua organização, eles serão usados. Caso contrário, você verá as opções de status padrão:

* [!UICONTROL Pendente]
* [!UICONTROL Aprovado]
* [!UICONTROL Aprovado com alterações]
* [!UICONTROL Alterações exigidas]
* [!UICONTROL Não é relevante]

Abra a janela do fluxo de trabalho de revisão para ver o status da prova dos destinatários atribuídos às funções de [!UICONTROL Revisor e aprovador] ou [!UICONTROL Aprovador]da prova.

## Relatórios no [!DNL Workfront]

Você também pode aproveitar os recursos de relatórios do [!DNL Workfront’s] para acompanhar as provas à medida que elas avançam no processo de revisão e aprovação.

Um relatório de aprovação de prova ajuda a acompanhar as aprovações pendentes para garantir que os prazos sejam cumpridos.

![Imagem de um relatório de aprovação de prova no [!DNL  Workfront].](assets/proof-approval-report.png)

Um relatório de versão do documento permite gerenciar e acompanhar versões da prova.

![Imagem de um relatório de versão do documento no [!DNL  Workfront].](assets/document-version-report.png)

Recomendamos conversar com o(a) consultor(a) do [!DNL Workfront] para criar relatórios que atendam aos requisitos da sua organização. Alguns dos relatórios exigem conhecimento sobre os relatórios do modo de texto do [!DNL Workfront’s].

## Sua vez

Converse com sua equipe ou com o(a) admin do sistema de revisão para descobrir que tipo de relatório você usará no Workfront para manter os fluxos de trabalho de provas funcionando perfeitamente.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
