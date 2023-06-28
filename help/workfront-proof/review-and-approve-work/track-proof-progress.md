---
title: Rastrear o progresso da prova
description: Saiba como usar o [!UICONTROL SOCD] indicadores, progresso da prova e relatórios para acompanhar o progresso de uma prova no [!DNL  Workfront].
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
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 1%

---

# Rastrear o progresso da prova

Como gerente de projeto, gerente de prova ou outra parte interessada no processo de revisão e aprovação, você desejará acompanhar o progresso de suas provas. Você pode fazer isso com [!DNL Workfront’s] incorporado **indicadores de progresso da prova** no [!UICONTROL Documentos] ou escrevendo relatórios personalizados.

Para visualizar o progresso da prova no [!DNL Workfront], você deve ter uma licença de Plano, Trabalho ou Revisão e ser um usuário de prova. Se você não tiver certeza do seu [!DNL Workfront] o perfil atende a esses requisitos, consulte o administrador do sistema de comprovação em sua organização.

## Rastrear o progresso da prova com [!UICONTROL SOCD] indicadores e status da prova

Obtenha uma exibição de alto nível de como a prova está avançando no processo de revisão e aprovação usando o [!UICONTROL SOCD] ícones na [!UICONTROL Documentos] lista. Esses ícones indicam ações específicas tomadas na prova.

![Uma imagem do [!UICONTROL Documentos] listar em um [!DNL  Workfront] projeto com o [!UICONTROL SOCD] ícones realçados.](assets/manage-proofs-socd.png)

Os ícones indicam o trabalho feito em uma prova desde o momento em que você envia a prova para os recipients até o momento em que eles tomam uma decisão sobre a prova.

* **S —** A prova foi enviada aos recipients.
* **O —** A prova foi aberta.
* **C —** Foram feitos comentários sobre a prova.
* **D —** Foi tomada uma decisão sobre a prova (aprovada, rejeitada, etc.).

As cores indicam se a ação foi concluída ou não.

* **Branco —** A etapa ainda não aconteceu.
* **Verde —** A etapa foi concluída.
* **Laranja —** O prazo de prova é de 24 horas e a etapa não aconteceu.
* **Vermelho —** O prazo de prova terminou e a etapa não aconteceu.

A variável [!UICONTROL SOCD] no [!UICONTROL Documentos] no painel de resumo ou na lista [!UICONTROL Detalhes do documento], é um resumo de alto nível do progresso da prova. [!DNL Workfront] configura isso com base no recipient que está &quot;mais atrasado&quot; no processo de prova.

Por exemplo, se houver três revisores/aprovadores e apenas dois deles tiverem observado a prova e feito comentários, a variável [!UICONTROL SOCD] Os ícones mostrarão que a prova foi enviada ([!UICONTROL S]) e aberta ([!UICONTROL O]), mas não que tenham sido feitas observações ([!UICONTROL C]).

Se quiser saber o desempenho de cada recipient de prova individual, abra o fluxo de trabalho de prova. O progresso geral da prova está na parte superior da janela. Cada estágio tem seu próprio indicador de progresso na barra cinza.  E ao lado de cada usuário está o progresso desse indivíduo.

![Uma imagem do [!UICONTROL Fluxo de trabalho de provas] seção de um documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Status da prova

O status da prova é baseado no status dos recipients da prova do estágio. O status geral da prova é visível no [!UICONTROL Documentos] à direita da página [!UICONTROL SOCD] indicadores, para que você possa saber facilmente se tem uma decisão sobre a prova.

![Uma imagem do [!UICONTROL Documentos] listar em um [!DNL  Workfront] projeto com o status geral de prova destacado.](assets/manage-proofs-overall-status.png)

Esse status da prova indica o status geral da prova. Por exemplo, se dois recipients aprovaram a prova, seus status individuais mostrarão [!UICONTROL Aprovado]. No entanto, o terceiro recipient ainda não tomou uma decisão, de modo que o status dessa pessoa é [!UICONTROL Pending]. Por conseguinte, o estatuto geral [!UICONTROL Pending].

Se status personalizados foram configurados para sua organização, eles serão usados. Caso contrário, você verá as opções de status padrão de:

* [!UICONTROL Pendente]
* [!UICONTROL Aprovado]
* [!UICONTROL Aprovado com alterações]
* [!UICONTROL Alterações exigidas]
* [!UICONTROL Não é relevante]

Abra a janela de fluxo de trabalho de prova para ver um status de prova para os destinatários atribuídos a [!UICONTROL Revisor e Aprovador] ou [!UICONTROL Aprovador]funções de prova.

## Relatórios em [!DNL Workfront]

Você também pode aproveitar [!DNL Workfront’s] recursos de relatórios para rastrear provas à medida que elas avançam pelo processo de revisão e aprovação.

Um relatório de aprovação de prova ajuda a rastrear aprovações pendentes para garantir que os prazos sejam cumpridos.

![Uma imagem de um relatório de aprovação de prova no [!DNL  Workfront].](assets/proof-approval-report.png)

Um relatório de versão de documento permite gerenciar e rastrear versões de prova.

![Uma imagem de um relatório de versão do documento no [!DNL  Workfront].](assets/document-version-report.png)

Recomendamos trabalhar com o [!DNL Workfront] para criar relatórios que atendam aos requisitos de sua organização. Alguns relatórios exigem familiaridade com [!DNL Workfront’s] relatório em modo de texto.

## Sua vez

Converse com sua equipe ou administrador do sistema de prova para descobrir que tipo de relatório você usará no Workfront para manter os fluxos de trabalho de prova em perfeita execução.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
