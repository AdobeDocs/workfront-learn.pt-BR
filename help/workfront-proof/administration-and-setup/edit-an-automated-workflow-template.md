---
title: Editar um template de workflow automatizado
description: Saiba como fazer alterações em um modelo de fluxo de trabalho de comprovação automatizada existente no [!DNL  Workfront].
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
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Editar um template de workflow automatizado

À medida que os processos de revisão e aprovação de prova são refinados ou que alterações organizacionais são feitas, os modelos automatizados de fluxo de trabalho devem ser atualizados para refletir as operações atuais das equipes que usam o Workfront.

Manter os modelos atualizados garante a consistência em seus processos de revisão e aprovação, além de economizar tempo para essas provas de upload, pois elas não precisam ajustar constantemente um fluxo de trabalho.

1. Selecionar **[!UICONTROL Prova]** do **[!UICONTROL Menu principal]** in [!DNL Workfront].
1. Nesse ponto, selecione **[!UICONTROL Fluxos de trabalho]** no menu do painel esquerdo.
1. Clique no menu de 3 pontos na extremidade direita do nome do modelo e selecione **[!UICONTROL Exibir detalhes do modelo]**.

As opções para compartilhar, copiar e excluir o modelo estão na parte superior da janela de detalhes de cada modelo. A exclusão de um modelo não afeta as provas em andamento que têm esse modelo aplicado, mas significa que o modelo não está mais disponível para uso.

![Janela Detalhes do modelo](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

Clique na seta para expandir a [!UICONTROL Detalhes] para alterar coisas como o nome do template ou o fuso horário do template.

## Fazer alterações em estágios e destinatários

As alterações podem ser necessárias no [!UICONTROL Fluxo de trabalho] área em que um processo simplificado significa um prazo mais curto ou quando alguém entra na equipe do e revisará as provas.

Cada estágio de um fluxo de trabalho automatizado tem sua própria seção, que permite que os prazos, a privacidade, os recipients de prova e outras informações sejam modificados independentemente.

Este vídeo demonstra brevemente algumas das alterações que você pode fazer no [!UICONTROL Fluxo de trabalho] área. Consulte a lista com marcadores neste vídeo, que analisa essas configurações. Não há áudio neste vídeo.

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12)

Como revisão, estas são as alterações de modelo de prova que você pode fazer no [!UICONTROL Fluxo de trabalho] seção:

* Clique em na [!UICONTROL nome do estágio] ou a variável [!UICONTROL prazo] para atualizar essas informações.
* Selecione a seta ao lado da [!UICONTROL prazo] para bloquear o estágio, determine quando o estágio é ativado ou exija apenas uma decisão.
* Na lista de destinatários, clique na guia [!UICONTROL Função] ou [!UICONTROL Alertas de email] para selecionar outra opção.
* Acesse o menu de 3 pontos na extremidade direita do nome de um destinatário para excluí-lo da lista, torná-lo o principal responsável pela tomada de decisões nesse estágio do fluxo de trabalho ou edite as informações de função de prova e alerta de email.
* Você tem duas opções para adicionar recipients à lista. Depois de abrir o [!UICONTROL Adicionar pessoas ao estágio] clique no estágio ao qual deseja adicioná-los. Em seguida, insira seu nome ou endereço de email na lista de recipients e atribua uma função de prova e um alerta por email. Clique em [!UICONTROL Adicionar pessoas] quando terminar.
   1. No canto superior direito de cada seção de estágio, vá para a [!UICONTROL Mais] e selecione [!UICONTROL Adicionar pessoas ao estágio].
   1. Na parte superior do [!UICONTROL Fluxo de trabalho] , selecione [!UICONTROL Adicionar pessoas ao estágio].

## Compartilhamento de modelo

A variável [!UICONTROL Compartilhado com] exibe os usuários de prova que podem usar o modelo. Remova as pessoas que não precisam mais usar o modelo clicando no menu de 3 pontos à direita do nome e selecionando [!UICONTROL Remover].

![[!UICONTROL Compartilhado com] lista](assets/proof-system-setups-edit-template-shared-with.png)

No entanto, não é possível adicionar pessoas à lista de compartilhamento nesta seção. Para fazer isso, volte para a parte superior da janela de detalhes do modelo e clique na guia [!UICONTROL Compartilhar modelo] botão.

## seção Atividade

[!DNL Workfront] mantém um histórico de auditoria de quando as alterações foram feitas no modelo. Você pode ver a data, quem fez a alteração e algumas informações resumidas sobre quais alterações foram feitas.

Esta seção não registra informações sobre quando o modelo foi usado em provas.

![Lista de atividades de prova](assets/proof-system-setups-edit-template-activity.png)
