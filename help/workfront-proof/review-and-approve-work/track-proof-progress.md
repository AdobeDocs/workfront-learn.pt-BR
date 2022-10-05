---
title: Como rastrear o progresso da prova
description: Saiba como usar [!UICONTROL SOCD] indicadores, progresso de prova e relatórios para rastrear o progresso de uma prova em [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
kt: 10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

# Rastrear progresso de prova

Como gerente de projeto, gerente de prova ou outra parte interessada no processo de revisão e aprovação, você deverá acompanhar o progresso das provas. Você pode fazer isso com [!DNL Workfront’s] integrado **indicadores de progresso da prova** no [!UICONTROL Documentos] ou escrevendo relatórios personalizados.

Para exibir o progresso da prova em [!DNL Workfront], você deve ter uma licença de Plano, Trabalho ou Revisão e ser um usuário de prova. Se você não tiver certeza da sua [!DNL Workfront] O perfil atende a esses requisitos, verifique com o administrador do sistema de prova da sua organização.

## Rastrear o progresso da prova com [!UICONTROL SOCD] indicadores e status de prova

Obtenha uma exibição de alto nível de como a prova está progredindo no processo de revisão e aprovação usando o [!UICONTROL SOCD] ícones na [!UICONTROL Documentos] lista. Esses ícones indicam ações específicas executadas na prova.

![Uma imagem da [!UICONTROL Documentos] em uma [!DNL  Workfront] com o [!UICONTROL SOCD] ícones realçados.](assets/manage-proofs-socd.png)

Os ícones indicam o trabalho feito em uma prova a partir do momento em que você envia a prova aos recipients até o momento em que eles tomam uma decisão sobre a prova.

* **S —** A prova foi enviada aos recipients.
* **O —** A prova foi aberta.
* **C —** Foram apresentadas observações sobre a prova.
* **D —** Foi tomada uma decisão sobre a prova (aprovada, rejeitada, etc.).

As cores indicam se a ação foi concluída ou não.

* **Branco —** A etapa ainda não aconteceu.
* **Verde —** A etapa foi concluída.
* **Laranja —** O prazo de prova está em 24 horas e a etapa não aconteceu.
* **Vermelho —** O prazo de prova foi ultrapassado e a etapa não aconteceu.

O [!UICONTROL SOCD] no [!UICONTROL Documentos] , no painel de resumo ou na [!UICONTROL Detalhes do documento], é um resumo de alto nível do progresso da prova. [!DNL Workfront] O configura com base no recipient que está &quot;mais atrás&quot; no processo de prova.

Por exemplo, se houver três revisores/aprovadores e apenas dois deles tiverem observado a prova e feito comentários, então a função [!UICONTROL SOCD] os ícones mostrarão que a prova foi enviada ([!UICONTROL S]) e aberto ([!UICONTROL O], mas não que tenham sido feitas observações ([!UICONTROL C]).

Para saber como cada recipient de prova está indo, abra o workflow de prova. O progresso da prova geral está na parte superior da janela. Cada estágio tem seu próprio indicador de progresso na barra cinza.  E ao lado de cada usuário está o progresso desse indivíduo.

![Uma imagem da [!UICONTROL Fluxo de trabalho de prova] de um documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Status da prova

O status da prova é baseado no status dos recipients de prova do estágio. O status geral da prova é visível no [!UICONTROL Documentos] à direita do [!UICONTROL SOCD] para que você possa identificar se tem uma decisão sobre a prova.

![Uma imagem da [!UICONTROL Documentos] em uma [!DNL  Workfront] projeto com o status de prova geral destacado.](assets/manage-proofs-overall-status.png)

Esse status de prova indica o status geral da prova. Por exemplo, se dois recipients aprovaram a prova, seus status individuais mostrarão [!UICONTROL Aprovado]. No entanto, o terceiro recipient ainda não tomou uma decisão, portanto o status dessa pessoa é [!UICONTROL Pending]. Portanto, o status geral é mostrado como [!UICONTROL Pending].

Se os status personalizados forem configurados para sua organização, esses status serão usados. Caso contrário, você verá as opções de status padrão de:

* [!UICONTROL Pendente]
* [!UICONTROL Aprovado]
* [!UICONTROL Aprovado com alterações]
* [!UICONTROL Alterações exigidas]
* [!UICONTROL Não é relevante]

Abra a janela do workflow de prova para ver um status de prova para os recipients que receberam a variável [!UICONTROL Revisor e Aprovador] ou [!UICONTROL Aprovador ]funções de prova.

## Relatórios em [!DNL Workfront]

Você também pode aproveitar [!DNL Workfront’s] recursos de relatório para rastrear provas conforme elas avançam pelo processo de revisão e aprovação.

Um relatório de aprovação de prova ajuda você a rastrear aprovações pendentes para garantir que os prazos sejam cumpridos.

![Uma imagem de um relatório de aprovação de prova em [!DNL  Workfront].](assets/proof-approval-report.png)

Um relatório de versão do documento permite gerenciar e rastrear versões de prova.

![Uma imagem de um relatório de versão de documento em [!DNL  Workfront].](assets/document-version-report.png)

Recomendamos trabalhar com a [!DNL Workfront] consultor da para criar relatórios que atendam às necessidades de sua organização. Alguns relatórios exigem familiaridade com [!DNL Workfront’s] relatório do modo de texto.

## Sua vez

Fale com a sua equipe ou o administrador do sistema de prova para descobrir que tipo de relatório você usará no Workfront para manter os fluxos de trabalho de prova em execução sem problemas.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
