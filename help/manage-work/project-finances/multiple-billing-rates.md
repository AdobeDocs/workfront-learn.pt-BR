---
title: Entender várias taxas de faturamento
description: No Workfront, um gerente de projeto pode substituir as taxas de faturamento do sistema em um projeto específico.
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
kt: 10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Entender várias taxas de faturamento

Within [!DNL Workfront], um gerente de projeto tem a capacidade de substituir as taxas de faturamento do sistema em um projeto específico. Anteriormente, quando a nova taxa de faturamento era aplicada ao projeto, ela não afetava apenas horas futuras, mas horas já registradas no projeto.

Com [!DNL Workfront]O novo recurso de taxa de faturamento múltipla do , o gerente do projeto pode decidir qual período de tempo uma taxa de faturamento deve ser aplicada. Dessa forma, se uma taxa tiver sido negociada ou alterada, o gerente do projeto poderá determinar quando essa taxa deve entrar em vigor.

## Alterar a taxa de faturamento

1. Vá para a landing page do projeto. Selecionar **[!UICONTROL Taxas de Faturamento]** no painel esquerdo.

   ![Uma imagem de seleção [!UICONTROL Taxas de Faturamento] em [!DNL Workfront]](assets/project-finances-1.png)

1. No **[!UICONTROL Taxas de Faturamento]** clique no botão **[!UICONTROL Adicionar Taxa de Faturamento]** botão. Selecionar **[!UICONTROL Nova Taxa de Faturamento]** na lista suspensa.

   ![Uma imagem de seleção [!UICONTROL Nova Taxa de Faturamento] em [!DNL Workfront]](assets/project-finances-2.png)

1. O [!UICONTROL Nova Taxa de Faturamento] será exibida. No **[!UICONTROL Função da Tarefa]** selecione a função de trabalho à qual a nova taxa de faturamento será aplicada.

   ![Uma imagem de seleção de funções de trabalho em uma nova taxa de faturamento em [!DNL Workfront]](assets/project-finances-3.png)

1. Depois que a função de trabalho é selecionada, a variável [!UICONTROL Taxa de Faturamento Padrão] e [!UICONTROL Taxa de Faturamento 1] for exibido. Insira a nova taxa de faturamento no [!UICONTROL Taxa de Faturamento 1] campo. Se essa taxa de faturamento se aplicar a todo o projeto (horas passadas, presentes e futuras registradas), clique no botão **[!UICONTROL Salvar]** botão.

   ![Uma imagem de salvar uma nova taxa de faturamento que se aplica a todo o projeto em [!DNL Workfront]](assets/project-finances-5.png)

1. Se a nova taxa de faturamento se aplicar apenas por um determinado período de tempo, clique no botão **[!UICONTROL Taxa de adição]** botão. O [!UICONTROL Taxa de Faturamento 1 Data Final] e [!UICONTROL Taxa de Faturamento 2] campos são exibidos. Informe a Data Final para [!UICONTROL Taxa de Faturamento 1]. Não é possível inserir uma Data Inicial para [!UICONTROL Taxa de Faturamento 1] porque o sistema parte do princípio de que foi iniciado no início do projeto.

   ![Uma imagem da criação de uma nova taxa de faturamento que se aplica a um determinado período de tempo, começando no início do projeto em [!DNL Workfront]](assets/project-finances-6.png)

1. Caso contrário:

   * Informe a taxa de faturamento padrão para [!UICONTROL Taxa de Faturamento 1].
   * Selecione a Data Final para [!UICONTROL Taxa de Faturamento 1] ([!UICONTROL Taxa de Faturamento Padrão]).
   * A data inicial para [!UICONTROL Taxa de Faturamento 2] será automaticamente definido como no dia seguinte [!UICONTROL Taxa de Faturamento 1] termina.
   * Insira a taxa de faturamento desejada na variável [!UICONTROL Taxa de Faturamento 2] seção.
   * Continue a adicionar as taxas de faturamento, conforme necessário, clicando no botão **[!UICONTROL Taxa de adição]** botão.
   * Quando terminar, clique em **[!UICONTROL Salvar]**.
   * Todas as Taxas de Faturamento serão mostradas na [!UICONTROL Taxas de Faturamento] no projeto.
   ![Uma imagem da criação de novas taxas de faturamento que se aplicam aos diferentes períodos de tempo em [!DNL Workfront]](assets/project-finances-7.png)
