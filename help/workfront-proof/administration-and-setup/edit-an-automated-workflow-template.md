---
title: Editar um modelo de fluxo de trabalho automatizado
description: Saiba como fazer alterações em um modelo de fluxo de trabalho de prova automatizada existente no [!DNL  Workfront].
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
kt: 8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Editar um modelo de fluxo de trabalho automatizado

À medida que os processos de revisão e aprovação de prova são refinados ou alterações organizacionais são feitas, os modelos de fluxo de trabalho automatizados devem ser atualizados para refletir as operações atuais das equipes que usam o Workfront.

Manter os modelos atualizados garante a consistência em seus processos de revisão e aprovação, além de economizar tempo para esses processos de upload, pois eles não precisam ajustar constantemente um fluxo de trabalho.

1. Selecionar **[!UICONTROL Tofing]** do **[!UICONTROL Menu principal]** em [!DNL Workfront].
1. Em seguida, selecione **[!UICONTROL Fluxos de trabalho]** no menu do painel esquerdo.
1. Clique no menu de 3 pontos à direita do nome do modelo e selecione **[!UICONTROL Exibir detalhes do modelo]**.

As opções para compartilhar, copiar e excluir o modelo estão na parte superior da janela de detalhes do modelo para cada modelo. A exclusão de um modelo não afeta as provas em andamento que têm esse modelo aplicado, mas significa que o modelo não está mais disponível para uso.

![Janela de detalhes do modelo](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

Clique na seta para expandir a variável [!UICONTROL Detalhes] para alterar coisas como o nome do modelo ou o fuso horário do modelo.

## Fazer alterações em palcos e recipients

As alterações podem ser necessárias na [!UICONTROL Fluxo de trabalho] área em que um processo simplificado significa um prazo anterior ou quando alguém ingressar na equipe e revisará provas.

Cada estágio de um fluxo de trabalho automatizado tem sua própria seção, que permite que prazos, privacidade, recipients de prova e outras informações sejam modificados independentemente.

Este vídeo mostra algumas das mudanças que você pode fazer na [!UICONTROL Fluxo de trabalho] área. Consulte a lista com marcadores neste vídeo, que analisa essas configurações. Não há áudio neste vídeo.

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12&learn=on)

Como revisão, aqui estão as alterações no modelo de prova que você pode fazer na [!UICONTROL Fluxo de trabalho] seção:

* Clique no botão [!UICONTROL nome do estágio] ou o [!UICONTROL prazo] para atualizar essas informações.
* Selecione a seta ao lado do [!UICONTROL prazo] para bloquear o palco, determinar quando o palco é ativado ou exigir apenas uma decisão.
* Na lista de recipients, clique em na variável [!UICONTROL Função] ou [!UICONTROL Alertas por email] campos para selecionar outra opção.
* Vá para o menu de 3 pontos à extrema direita do nome de um destinatário para excluí-los da lista, torná-los o principal decisor para esse estágio de fluxo de trabalho ou edite a função de prova e as informações de alerta por email.
* Você tem duas opções para adicionar recipients à lista. Depois de abrir o [!UICONTROL Adicionar pessoas ao palco] clique em qual estágio deseja adicioná-los. Em seguida, insira o nome ou endereço de email na lista de recipients e atribua uma função de prova e um alerta de email. Clique no botão [!UICONTROL Adicionar pessoas] quando terminar.
   1. No canto superior direito de cada seção de estágio, vá para o [!UICONTROL Mais] e selecione [!UICONTROL Adicionar pessoas ao palco].
   1. Na parte superior do [!UICONTROL Fluxo de trabalho] , selecione [!UICONTROL Adicionar pessoas ao palco].

## Compartilhamento de modelo

O [!UICONTROL Compartilhado com] exibe os usuários de prova que podem usar o modelo. Remova as pessoas que não precisam mais usar o modelo clicando no menu de três pontos à extrema direita do nome e selecionando [!UICONTROL Remover].

![[!UICONTROL Compartilhado com] lista](assets/proof-system-setups-edit-template-shared-with.png)

No entanto, não é possível adicionar pessoas à lista de compartilhamento desta seção. Para fazer isso, volte para a parte superior da janela de detalhes do modelo e clique no botão [!UICONTROL Compartilhar modelo] botão.

## Seção Atividade

[!DNL Workfront] mantém um histórico de auditoria de quando as alterações foram feitas no modelo. Você pode ver a data, quem fez a alteração e algumas informações resumidas sobre quais alterações foram feitas.

Esta seção não registra informações sobre quando o template foi usado em provas.

![Lista de atividades de prova](assets/proof-system-setups-edit-template-activity.png)
