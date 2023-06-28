---
title: Compreender várias taxas de cobrança
description: Saiba como substituir as taxas de faturamento do sistema em um projeto.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Compreender várias taxas de cobrança

Dentro de [!DNL Workfront], um gerente de projeto pode sobrepor as taxas de faturamento do sistema em um projeto específico. Anteriormente, quando a nova taxa de cobrança era aplicada ao projeto, ela não afetava apenas as horas futuras, mas as horas já registradas no projeto.

Com [!DNL Workfront]Com o novo recurso de cobrança múltipla da, o gerente de projeto pode decidir que período de tempo uma taxa de cobrança deve ser aplicada. Dessa forma, se uma taxa tiver sido negociada ou alterada, o gerente de projeto poderá determinar quando essa taxa deverá entrar em vigor.

## Alterar a taxa de cobrança

1. Acesse a página de aterrissagem do projeto. Selecionar **[!UICONTROL Taxas de cobrança]** no painel esquerdo.

   ![Uma imagem de seleção [!UICONTROL Taxas de cobrança] in [!DNL Workfront]](assets/project-finances-1.png)

1. No **[!UICONTROL Taxas de cobrança]** clique na guia **[!UICONTROL Adicionar taxa de cobrança]** botão. Selecionar **[!UICONTROL Novo preço]** na lista suspensa.

   ![Uma imagem de seleção [!UICONTROL Novo preço] in [!DNL Workfront]](assets/project-finances-2.png)

1. A variável [!UICONTROL Novo preço] é exibida. No **[!UICONTROL Função de trabalho]** selecione a função de trabalho à qual a nova taxa de cobrança será aplicada.

   ![Uma imagem de seleção de funções de trabalho em uma nova taxa de cobrança no [!DNL Workfront]](assets/project-finances-3.png)

1. Depois que a função de trabalho for selecionada, a variável [!UICONTROL Taxa de Cobrança Padrão] e a variável [!UICONTROL Taxa de cobrança 1] é exibido. Informe a nova taxa de faturamento no [!UICONTROL Taxa de cobrança 1] campo. Se essa taxa de cobrança se aplicar a todo o projeto (horas passadas, presentes e futuras registradas), clique no link **[!UICONTROL Salvar]** botão.

   ![Uma imagem de como salvar uma nova taxa de cobrança que se aplica a todo o projeto em [!DNL Workfront]](assets/project-finances-5.png)

1. Se a nova taxa de cobrança se aplicar somente por um determinado período, clique no link **[!UICONTROL Adicionar taxa]** botão. A variável [!UICONTROL Data Final da Taxa de Cobrança 1] e a variável [!UICONTROL Taxa de cobrança 2] são exibidos. Informe a Data Final para [!UICONTROL Taxa de cobrança 1]. Não é possível inserir uma Data inicial para [!UICONTROL Taxa de cobrança 1] porque o sistema supõe que ele iniciou no início do projeto.

   ![Uma imagem da criação de uma nova taxa de cobrança que se aplica a um determinado período, começando no início do projeto em [!DNL Workfront]](assets/project-finances-6.png)

1. Se esse não for o caso:

   * Insira a taxa de cobrança padrão para [!UICONTROL Taxa de cobrança 1].
   * Selecione a data final para [!UICONTROL Taxa de cobrança 1] ([!UICONTROL Taxa de Cobrança Padrão]).
   * A data de início para [!UICONTROL Taxa de cobrança 2] será automaticamente definido para o dia seguinte [!UICONTROL Taxa de cobrança 1] termina.
   * Informe a taxa de faturamento desejada nas [!UICONTROL Taxa de cobrança 2] seção.
   * Continue a adicionar taxas de cobrança, conforme necessário, clicando no link **[!UICONTROL Adicionar taxa]** botão.
   * Quando terminar, clique em **[!UICONTROL Salvar]**.
   * Todas as taxas de cobrança serão exibidas no [!UICONTROL Taxas de cobrança] no projeto.

   ![Uma imagem da criação de novas taxas de faturamento que se aplicam a diferentes períodos no [!DNL Workfront]](assets/project-finances-7.png)
