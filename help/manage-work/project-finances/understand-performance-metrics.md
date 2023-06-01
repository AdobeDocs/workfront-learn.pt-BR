---
title: Compreender métricas de desempenho
description: Saiba como usar as métricas de desempenho - o [!UICONTROL Método Índice de desempenho] ([!UICONTROL PIM]) e o [!UICONTROL Estimativa no término] ([!UICONTROL EAC]).
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: 65bd26fefb280d12ec44a4923f6d96ac8d88d6fb
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Compreender métricas de desempenho

Duas métricas de desempenho usadas pelos gerentes de projeto incluem o [!UICONTROL Método Índice de desempenho] ([!UICONTROL PIM]) e o [!UICONTROL Estimativa no término] ([!UICONTROL EAC]). Os padrões do sistema podem ser definidos em [!DNL Workfront] e se aplicam a projetos recém-criados. [!UICONTROL PIM] podem ser modificados em projetos individuais.

**[!UICONTROL MID]**

As configurações para a variável [!UICONTROL PIM] controlar como [!DNL Workfront] O calcula outras métricas de desempenho do projeto, como [!UICONTROL Índice de Desempenho de Custo] ([!UICONTROL CPI]), [!UICONTROL Índice de Desempenho de Agendamento de Custo] ([!UICONTROL CSI]), [!UICONTROL Índice de desempenho do cronograma] ([!UICONTROL SPI]) e [!UICONTROL Estimativa no término] ([!UICONTROL EAC]).

Opções para o [!UICONTROL PIM] são baseados em horas e em custos.

* **Baseado em Hora** — A Workfront utiliza as horas planejadas no cálculo do CPI e EAC do projeto. O EAC do projeto é exibido como um número, em horas.
* **Baseado em Custo** — A Workfront utiliza o custo de mão de obra planejado para calcular o CPI e o EAC do projeto. EAC aparece como um valor de moeda. Ao usar essa opção, verifique se os atribuídos à tarefa (usuários e/ou funções de trabalho) estão associados às taxas de custo.

**[!UICONTROL EAC]**

[!UICONTROL EAC] representa o custo total projetado de sua tarefa ou projeto quando ele é concluído. As opções são calculadas no nível do projeto e totalizadas a partir de tarefas/subtarefas.

* **Calcular no nível do projeto** — [!UICONTROL EAC] para a tarefa-pai e o projeto são determinados usando as horas reais/custos reais de mão de obra em [!UICONTROL EAC] fórmulas. O cálculo inclui horas/custos reais e despesas adicionadas diretamente à tarefa ou ao projeto principal.
* R **Extrair de tarefas/subtarefas** — [!UICONTROL EAC] para a tarefa pai e o projeto são determinados adicionando a variável [!UICONTROL EAC] para cada tarefa filho. Esse cálculo exclui horas/custos reais adicionados diretamente a uma tarefa ou projeto principal.

A variável [!UICONTROL EAC] os cálculos estão listados em [Calcular Estimativa no Término (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**Métricas de desempenho: Configurações**

Para definir [!UICONTROL PIM] e [!UICONTROL EAC] padrões do sistema:

1. Selecionar **[!UICONTROL Configuração]** no menu principal.
1. Clique em **[!UICONTROL Preferências do projeto]** no menu do painel esquerdo, clique em **[!UICONTROL Projetos]**
1. No [!UICONTROL Status do projeto] seção, localizar [!UICONTROL Método Índice de desempenho]. Selecione Baseado em horas ou Baseado em custo.
1. Para [!UICONTROL Estimativa no término], selecione Calcular no nível do projeto ou Totalizar de tarefas/subtarefas.
1. Clique em **[!UICONTROL Salvar]** na parte inferior da janela.

![Uma imagem do [!UICONTROL Preferências do projeto] tela](assets/setting-up-finances-1.png)

**Definir [!UICONTROL PIM] em projetos individuais**

1. Vá para a landing page de um projeto.
1. Clique em **[!UICONTROL Detalhes do projeto]** no painel esquerdo.
1. Abra o **[!UICONTROL Finanças]** seção.
1. Clique duas vezes no texto abaixo **[!UICONTROL Método Índice de desempenho]** para editá-lo.
1. Selecione Baseado em horas ou Baseado em custo.
1. Clique em **[!UICONTROL Salvar]** Alterações para concluir.

![Uma imagem do [!UICONTROL Detalhes do projeto] tela](assets/setting-up-finances-2.png)

[!UICONTROL PIM] pode ser definido em um modelo de projeto, no [!UICONTROL Finanças] seção dos detalhes do modelo.
