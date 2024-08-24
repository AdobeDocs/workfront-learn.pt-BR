---
title: Entenda as várias taxas de faturamento
description: Saiba como modificar as taxas de faturamento do sistema em um projeto.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
hide: true
source-git-commit: d7347d41099e0faf6b47a6fe0e58091105e4e41d
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 93%

---

# Entenda as várias taxas de faturamento

No [!DNL Workfront], gerentes de projeto têm a capacidade de modificar as taxas de faturamento do sistema em um projeto específico. Anteriormente, quando a nova taxa de faturamento era aplicada ao projeto, isso afetava não apenas as horas futuras, mas também as horas já registradas no projeto.

Com o novo recurso de cobrança múltipla de [!DNL Workfront], o gerente de projeto pode decidir o período de tempo em que uma taxa de cobrança deve ser aplicada. Dessa forma, se uma taxa tiver sido negociada ou alterada, o(a) gerente do projeto poderá determinar quando essa taxa deverá entrar em vigor.

## Alterar a taxa de faturamento

1. Vá para a landing page do projeto. Selecione **[!UICONTROL Taxas de faturamento]** no painel esquerdo.

   ![Uma imagem mostrando a seleção de [!UICONTROL Taxas de faturamento] no [!DNL Workfront]](assets/project-finances-1.png)

1. Na guia **[!UICONTROL Taxas de faturamento]**, clique no botão **[!UICONTROL Adicionar taxa de faturamento]**. Selecione **[!UICONTROL Nova taxa de faturamento]** no menu suspenso.

   ![Uma imagem mostrando a seleção de uma [!UICONTROL Nova taxa de faturamento] no [!DNL Workfront]](assets/project-finances-2.png)

1. A caixa de diálogo [!UICONTROL Nova taxa de faturamento] é exibida. No menu suspenso **[!UICONTROL Função no trabalho]**, selecione a função à qual a nova taxa de faturamento será aplicada.

   ![Uma imagem mostrando a seleção de funções de trabalho em uma nova taxa de faturamento no [!DNL Workfront]](assets/project-finances-3.png)

1. Uma vez selecionada a função, os campos [!UICONTROL Taxa de faturamento padrão] e [!UICONTROL Taxa de faturamento 1] são exibidos. Insira a nova taxa de faturamento no campo [!UICONTROL Taxa de faturamento 1]. Se essa taxa de faturamento se aplicar a todo o projeto (horas passadas, presentes e futuras registradas), clique no botão **[!UICONTROL Salvar]**.

   ![Uma imagem na qual uma nova taxa de faturamento que se aplica a todo o projeto no [!DNL Workfront]](assets/project-finances-5.png) é salva

1. Se a nova taxa de faturamento se aplica apenas a um determinado período, clique no botão **[!UICONTROL Adicionar taxa]**. Os campos [!UICONTROL Data final da taxa de faturamento 1] e [!UICONTROL Taxa de faturamento 2] serão exibidos. Insira a data final da [!UICONTROL Taxa de faturamento 1]. Você não pode inserir uma data inicial para a [!UICONTROL Taxa de faturamento 1] porque o sistema entende que ela começou no início do projeto.

   ![Uma imagem mostrando a criação de uma nova taxa de faturamento que se aplica a um determinado período, começando no início do projeto do [!DNL Workfront]](assets/project-finances-6.png)

1. Se esse não for o caso:

   * Insira a taxa de faturamento padrão para a [!UICONTROL Taxa de faturamento 1].
   * Selecione a data final para a [!UICONTROL Taxa de faturamento 1] ([!UICONTROL Taxa de faturamento padrão]).
   * A data inicial da [!UICONTROL Taxa de faturamento 2] será automaticamente definida para o dia seguinte ao término da [!UICONTROL Taxa de faturamento 1].
   * Insira a taxa de faturamento desejada na seção [!UICONTROL Taxa de faturamento 2].
   * Se necessário, continue adicionando taxas de faturamento clicando no botão **[!UICONTROL Adicionar taxa]**.
   * Quando concluído, clique em **[!UICONTROL Salvar]**.
   * Todas as taxas de faturamento serão exibidas na guia [!UICONTROL Taxas de faturamento] do projeto.

   ![Uma imagem mostrando a criação de novas taxas de faturamento que se aplicam aos diferentes períodos no [!DNL Workfront]](assets/project-finances-7.png)
