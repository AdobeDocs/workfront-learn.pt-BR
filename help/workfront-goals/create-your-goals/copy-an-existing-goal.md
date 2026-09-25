---
title: Copiar uma meta existente
description: Saiba como copiar uma meta existente no [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
    internal-label: Workfront Goals
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 98%
---
# Copiar uma meta existente

Digamos que seja o final de um trimestre e você queira recriar uma meta existente para o próximo período. Ou talvez você não tenha cumprido a meta e precise estendê-la para o próximo período. Qual é a melhor opção para criar essa meta? Você desejará copiar e modificar uma meta existente.

Copiar uma meta existente também é útil se vários membros da equipe tiverem metas semelhantes e você precisar criar uma meta para cada um deles.

<!--
Pro-tips graphic
-->

Aqui estão algumas coisas a considerar antes de copiar metas:

* Todas as informações da meta original serão copiadas, com exceção do período da meta (porque está no passado).
* Você pode copiar os resultados de uma meta existente e eles serão transferidos para a nova meta.
* Os resultados copiados são atribuídos ao mesmo proprietário, por padrão.
* Não é possível copiar o progresso da meta existente para uma nova meta.
* Você não pode copiar as atividades de uma meta ao copiar uma meta.

## Como copiar uma meta

1. Clique no nome de uma meta para abrir o painel **[!UICONTROL Detalhes da meta]**.
1. Clique no ícone de 3 pontos e selecione **[!UICONTROL Copiar]**.
1. Atualize qualquer uma das seguintes informações da meta copiada:
   * **Nova meta**: Este é o nome da nova meta. O padrão é o nome da meta original.
   * **Período**: O período durante o qual você deseja atingir a meta. Selecione um período no menu suspenso ou clique em Definir datas personalizadas para indicar um período personalizado. O período padrão é sempre o trimestre atual.
   * **Proprietário**: o proprietário da meta. Pode ser um usuário, equipe, grupo ou empresa. O padrão é o proprietário da meta original.
   * **Descrição**: informações adicionais sobre a meta.

1. Marque a caixa **[!UICONTROL Copiar resultados]** se a meta original tiver resultados adicionados e você quiser copiá-los para a nova meta. Os resultados da meta copiada têm o mesmo proprietário, nomes e valores medidos que os resultados da meta original.

1. Clique em **[!UICONTROL Salvar]**. A meta copiada é salva com um status de Rascunho.

   ![Uma imagem do painel [!UICONTROL Detalhes da meta] no [!DNL Workfront Goals] com a opção [!UICONTROL Copiar] ](assets/03-workfront-goals-copy-a-goal.png)

1. Clique em **[!UICONTROL Ativar]**, que atualiza o status da meta para Ativa. A meta deve ter uma atividade ou resultado associado para ser “ativada”.

1. Clique no **X** no canto superior direito do painel [!UICONTROL Detalhes da meta] para fechá-lo.

Se você copiou uma meta que não foi concluída em um período anterior e deseja continuar trabalhando nela no período seguinte, faça o seguinte:

1. Vá para a meta original em **[!UICONTROL Lista de metas]**, na seção **[!UICONTROL Check-in]** ou **[!UICONTROL Pulse]**.
1. Comente na meta para indicar que ela foi copiada e que uma meta mais atual foi criada.
1. Feche a meta original para preservar o progresso feito durante o período original. Clique no ícone de 3 pontos no painel **[!UICONTROL Detalhes da meta]** e selecione **[!UICONTROL Fechar]** no menu.
1. Atualize o valor [!UICONTROL Inicial] do novo resultado para corresponder ao valor **[!UICONTROL Alvo]** do resultado anterior, então o progresso da sua nova meta começa a ser calculado a partir do ponto alcançado no período anterior.
