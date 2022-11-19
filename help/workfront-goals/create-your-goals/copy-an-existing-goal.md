---
title: Copiar uma meta existente
description: Saiba como copiar uma meta existente no [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
kt: 10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Copiar uma meta existente

Digamos que seja o fim de um trimestre e você quer recriar uma meta existente para o próximo período. Ou talvez você não tenha completado a meta e precise se estender para o próximo período de tempo. Qual é a melhor opção para criar essa meta? Você desejará copiar e modificar uma meta existente.

Copiar uma meta existente também é útil se vários membros da equipe tiverem metas semelhantes e você precisar criar uma meta para cada um deles.

<!--
Pro-tips graphic
-->

Aqui estão algumas coisas que devem ser consideradas antes de copiar metas:

* Todas as informações da meta original serão copiadas, com exceção do período de meta (porque está no passado).
* Você pode copiar os resultados de uma meta existente e eles serão transferidos para a nova meta.
* Por padrão, os resultados copiados são atribuídos ao mesmo proprietário.
* Não é possível copiar o progresso da meta existente para uma nova meta.
* Não é possível copiar as atividades de uma meta ao copiar uma meta.

## Como copiar uma meta

1. Clique em um nome de meta para abrir a **[!UICONTROL Detalhes da meta]** painel.
1. Clique no ícone de 3 pontos e selecione **[!UICONTROL Copiar]**.
1. Atualize qualquer uma das seguintes informações para a meta copiada:
   * **Nova meta**—Este é o nome da nova meta. O padrão é o nome da meta original.
   * **Período**—O período de tempo durante o qual você deseja atingir a meta. Selecione um período de tempo no menu suspenso ou clique em Definir datas personalizadas para indicar um período de tempo personalizado. O período padrão é sempre o trimestre atual.
   * **Proprietário**—O proprietário do objetivo. Pode ser um usuário, uma equipe, um grupo ou uma empresa. O padrão é o proprietário da meta original.
   * **Descrição**—Informações adicionais sobre a meta.

1. Verifique a **[!UICONTROL Copiar resultados]** se a meta original tiver resultados adicionados a ela e você quiser copiá-los para a nova meta. Os resultados da meta copiada têm o mesmo proprietário, nomes e valores medidos que os resultados da meta original.

1. Clique em **[!UICONTROL Salvar]**. A meta copiada é salva com um status Rascunho.

   ![Uma imagem da [!UICONTROL Detalhes da meta] no painel [!DNL Workfront Goals] com o [!UICONTROL Copiar] opção](assets/03-workfront-goals-copy-a-goal.png)

1. Clique em **[!UICONTROL Ativar]**, que atualiza o status da meta para Ativo. A meta deve ter uma atividade ou resultado associado para &quot;ativar&quot;.

1. Clique no botão **X** no canto superior direito do [!UICONTROL Detalhes da meta] para fechá-lo.

Se você copiou uma meta que não foi concluída em um período anterior e deseja continuar trabalhando nela no período seguinte, faça o seguinte:

1. Vá para a meta original no **[!UICONTROL Lista de metas]**, **[!UICONTROL Check-in]** seção, ou **[!UICONTROL Pulso]** seção.
1. Comentário sobre a meta para indicar que foi copiada e que uma meta mais atual foi criada.
1. Feche a meta original para preservar o progresso feito durante seu período de tempo original. Clique no ícone de 3 pontos na **[!UICONTROL Detalhes da meta]** e selecione **[!UICONTROL Fechar]** no menu .
1. Atualize o [!UICONTROL Inicial] valor do novo resultado para corresponder ao valor **[!UICONTROL Target]** do resultado anterior, para que o novo progresso da meta comece a calcular a partir do ponto alcançado no período anterior.
