---
title: Como fazer upload usando fluxos de trabalho automatizados
description: Saiba quando usar um workflow de prova automatizada, como aplicar um workflow usando um template de prova e como configurar um workflow automatizado do zero.
activity: use
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335133.png
kt: 8833
exl-id: 8301ef00-1f47-4779-aa35-c735b66fdcac
source-git-commit: c06dcc985c3b63781911e3c8cb1ac0f1a888ac7d
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---

# Fazer upload de uma prova com um fluxo de trabalho automatizado

Neste vídeo, você aprenderá:

* Quando um workflow de prova automatizada pode ser usado
* Como aplicar um workflow usando um template de prova
* Como configurar um fluxo de trabalho automatizado do zero

>[!VIDEO](https://video.tv.adobe.com/v/335133/?quality=12)



## Configurações adicionais do fluxo de trabalho de prova

As configurações na parte inferior da janela de upload de prova são opcionais, portanto, verifique com sua organização se e como você as está usando.

![Uma imagem da [!UICONTROL Nova prova ]com a [!UICONTROL Configurações de preparo] destacado.](assets/additional-proof-workflow-settings.png)

* **[!UICONTROL Bloquear palco] —** Isso impede que as pessoas neste estágio de fluxo de trabalho façam comentários ou alterem decisões após a conclusão de seu estágio.
* **[!UICONTROL Transferir direitos de decisão primária para] —** Acelere o processo de verificação de provas designando um tomador de decisão principal. Quando definido, [!DNL Workfront] reconhece a decisão de prova dessa pessoa como A decisão. Assim que essa pessoa tomar a sua decisão, o palco acabou e não são necessárias outras decisões.
* **[!UICONTROL Exigir apenas uma decisão para esta fase] —** Outra maneira de simplificar o processo de comprovação é exigir apenas uma decisão sobre a prova. Com isso ativado, não importa quantos aprovadores você tem naquela fase, uma vez que qualquer um deles tome uma decisão, essa etapa está completa.
* **[!UICONTROL Tornar este estágio privado] —** Por padrão, os comentários na prova ficam visíveis para todos em todos os estágios. Impeça que os recipients de prova em outros estágios vejam os comentários feitos nesta fase clicando na caixa .

Na parte inferior da janela de upload de prova estão várias configurações de prova que afetam a segurança de sua prova, como exigir um logon para exibir a prova.

<!--
Learn more about these in the Proof settings section of the Configure a proof article.
-->

![Uma imagem da [!UICONTROL Configurações de prova] da janela de upload de prova.](assets/additional-proof-workflow-settings-2.png)

<!--
### Learn more
* Automated workflow overview
* Automated workflow stages overview
-->

<!--
### Guides
* Plan an advanced workflow worksheet
-->

## Por que você está no fluxo de trabalho de prova?

Você perceberá que está na lista de destinatários de prova porque foi você quem fez o upload da prova. Isso também torna você o proprietário da prova, que oferece direitos de edição sobre a prova, permitindo alterar as configurações do fluxo de trabalho ou fazer upload de uma nova versão, entre outras coisas.

![Uma imagem da janela de upload de prova com o proprietário da prova destacado na lista de recipients.](assets/proof-owner.png)

Se você estiver apenas fazendo upload da prova, mas outra pessoa estiver gerenciando o workflow, você poderá alterar o proprietário da prova clicando no link [!UICONTROL Proprietário] e inserir seu nome. Isso é recomendado se alguém que não seja o carregador original estiver carregando uma versão.

## Sua vez

>[!IMPORTANT]
>
>Não se esqueça de lembrar seus colegas de trabalho de que você está enviando uma prova como parte de seu treinamento do Workfront.


Faça upload de uma prova com um workflow avançado. Se a organização já tiver modelos de prova configurados, selecione aquele que foi usado pela equipe e faça alguns ajustes.

* Ajuste os alertas de email para que ninguém seja notificado quando a atividade ocorrer na prova.
* A primeira etapa deve ter dois revisores/aprovadores.
* O segundo estágio deve ter apenas 1 revisor/aprovador.

Se sua organização ainda não tiver modelos de prova criados, configure um fluxo de trabalho de duas etapas do zero.

* Atribua a si mesmo e ao seu colega de trabalho favorito ao primeiro estágio.
* Faça o prazo para a primeira etapa 1 dia a partir do momento em que a prova for criada.
* Atribua outro colega favorito ao segundo estágio.
* Faça o estágio começar quando o prazo do primeiro estágio tiver expirado.
* Dê à pessoa nesta fase 2 dias para concluir a revisão, mas ela tem de ser feita até ao meio-dia.


