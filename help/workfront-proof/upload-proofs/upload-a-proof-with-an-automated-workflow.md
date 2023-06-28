---
title: Fazer upload de uma prova com um fluxo de trabalho automatizado
description: Saiba quando usar um fluxo de trabalho de prova automatizado, como aplicar um fluxo de trabalho usando um modelo de prova e como configurar um fluxo de trabalho automatizado do zero.
activity: use
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335133.png
jira: KT-8833
exl-id: 8301ef00-1f47-4779-aa35-c735b66fdcac
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# Fazer upload de uma prova com um fluxo de trabalho automatizado

Neste vídeo, você aprenderá:

* Quando um fluxo de trabalho de prova automatizado pode ser usado
* Como aplicar um fluxo de trabalho usando um template de prova
* Como configurar um fluxo de trabalho automatizado do zero

>[!VIDEO](https://video.tv.adobe.com/v/335133/?quality=12&learn=on)



## Configurações adicionais de fluxo de trabalho de prova

As configurações na parte inferior da janela de upload de prova são opcionais, portanto, verifique com sua organização se e como você as está usando.

![Uma imagem do [!UICONTROL Nova prova]janela com o [!UICONTROL Configurações de preparo] destacado.](assets/additional-proof-workflow-settings.png)

* **[!UICONTROL Bloquear estágio] —** Isso impede que as pessoas neste estágio do fluxo de trabalho façam comentários ou alterem decisões depois que seu estágio do fluxo de trabalho for concluído.
* **[!UICONTROL Transferir direitos de decisão primários para] —** Acelere o processo de prova designando um tomador de decisão principal. Quando definido, [!DNL Workfront] O reconhece a decisão de prova por essa pessoa como A decisão. Quando essa pessoa toma sua decisão, o palco termina e nenhuma outra decisão é necessária.
* **[!UICONTROL Requer apenas uma decisão para este estágio] —** Outra maneira de simplificar o processo de prova é exigir apenas uma decisão sobre a prova. Com isso ativado, não importa quantos aprovadores você tenha nesse estágio, uma vez que qualquer um deles tome uma decisão, esse estágio é concluído.
* **[!UICONTROL Tornar privado este estágio] —** Por padrão, os comentários na prova ficam visíveis para todos em todos os estágios. Impeça que os recipients de prova em outros estágios vejam os comentários feitos durante esse estágio clicando na caixa.

Na parte inferior da janela de upload de prova há várias configurações de prova que afetam a segurança da prova, como a exigência de um logon para visualizar a prova.

<!--
Learn more about these in the Proof settings section of the Configure a proof article.
-->

![Uma imagem do [!UICONTROL Configurações de prova] seção da janela de upload de prova.](assets/additional-proof-workflow-settings-2.png)

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

Você perceberá que está na lista de recipients de prova porque é você que está fazendo upload da prova. Isso também torna você o proprietário da prova, o que lhe dá direitos de edição sobre a prova, permitindo alterar as configurações do fluxo de trabalho ou fazer upload de uma nova versão, entre outras coisas.

![Uma imagem da janela de upload de prova com o proprietário da prova destacado na lista de recipients.](assets/proof-owner.png)

Se você estiver apenas carregando a prova, mas outra pessoa estiver gerenciando o fluxo de trabalho, é possível alterar o proprietário da prova clicando no link [!UICONTROL Proprietário] e digitando seu nome. Isso é recomendado se alguém que não seja o carregador original estiver carregando uma versão.

## Sua vez

>[!IMPORTANT]
>
>Não se esqueça de lembrar aos colegas de trabalho que você está enviando a eles uma prova como parte do treinamento do Workfront.


Carregue uma prova com um fluxo de trabalho avançado. Se sua organização já tiver modelos de prova configurados, selecione aquele usado pela equipe e faça alguns ajustes.

* Ajuste os alertas de email para que ninguém seja notificado quando a atividade ocorrer na prova.
* O primeiro estágio deve ter 2 revisores/aprovadores.
* O segundo estágio deve ter apenas 1 revisor/aprovador.

Se sua organização ainda não tiver modelos de prova criados, configure um fluxo de trabalho de 2 etapas do zero.

* Atribua a si mesmo e a seu colega de trabalho favorito o primeiro estágio.
* Estabeleça o prazo para o primeiro estágio em 1 dia a partir de quando a prova é criada.
* Atribua outro colega de trabalho favorito ao segundo estágio.
* Faça com que a etapa comece quando o prazo da primeira etapa expirar.
* Dê à pessoa neste estágio dois dias para concluir a revisão, mas isso deve ser feito até o meio-dia.


