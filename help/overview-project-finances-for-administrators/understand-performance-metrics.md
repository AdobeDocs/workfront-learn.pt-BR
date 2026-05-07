---
title: Entenda as métricas de desempenho
description: 'Aprenda a usar as métricas de desempenho: o [!UICONTROL Método de índice de desempenho] ([!UICONTROL PIM]) e a [!UICONTROL Estimativa de conclusão] ([!UICONTROL EAC]).'
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
hide: true
exl-id: a7dbd937-0caa-4eb6-bb5d-bff6705e2972
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:02:44.647Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 445
ht-degree: 100%

---

# Entenda as métricas de desempenho

Duas métricas de desempenho usadas por gerentes de projeto incluem o [!UICONTROL Método de índice de desempenho] ([!UICONTROL PIM]) e a [!UICONTROL Estimativa de conclusão] ([!UICONTROL EAC]). É possível definir configurações padrão para todo o sistema do [!DNL Workfront] e aplicá-las a projetos recém-criados. O [!UICONTROL PIM] pode então ser modificado em projetos individuais.

**[!UICONTROL MID]**

As configurações do [!UICONTROL PIM] controlam como o [!DNL Workfront] calcula outras métricas de desempenho do projeto, como o [!UICONTROL Índice de desempenho de custos] ([!UICONTROL CPI]),[!UICONTROL  Índice de desempenho do cronograma de custos] ([!UICONTROL CSI]),[!UICONTROL  Índice de desempenho do cronograma ] ([!UICONTROL SPI]) e [!UICONTROL Estimativa de conclusão] ([!UICONTROL EAC]).

As opções do [!UICONTROL PIM] são baseadas em horas e em custos.

* **Baseado em horas**: o Workfront usa as horas planejadas no cálculo do CPI e da EAC do projeto. A EAC do projeto é exibida como um número, em horas.
* **Baseado em custos**: o Workfront usa o custo do trabalho planejado no cálculo do CPI e da EAC do projeto. A EAC é exibida como um valor monetário. Ao usar esta opção, verifique se os responsáveis pelas tarefas (usuários e/ou funções) estão associados às taxas de custo.

**[!UICONTROL EAC]**

A [!UICONTROL EAC] representa o custo total projetado de sua tarefa ou projeto após a conclusão. As opções são calculadas no nível do projeto e totalizadas a partir de tarefas e subtarefas.

* **Calcular no nível do projeto**: a [!UICONTROL EAC] da tarefa principal e do projeto é determinada usando as horas efetivas e custos reais de trabalho nas fórmulas da [!UICONTROL EAC]. O cálculo inclui horas e custos efetivos, bem como despesas adicionadas diretamente à tarefa principal ou projeto.
* T **otal de tarefas e subtarefas**: a [!UICONTROL EAC] da tarefa principal e do projeto é determinada pela soma da [!UICONTROL EAC] de cada tarefa derivada. Este cálculo exclui horas e custos efetivos adicionados diretamente a uma tarefa principal ou projeto.

Os cálculos de [!UICONTROL EAC] estão listados em [Calcular estimativa de conclusão (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=br).

**Métricas de desempenho: configurações**

Para definir os padrões do sistema para [!UICONTROL PIM] e [!UICONTROL EAC]:

1. Selecione **[!UICONTROL Configurar]** no menu principal.
1. Clique em **[!UICONTROL Preferências do projeto]** no menu do painel esquerdo e selecione **[!UICONTROL Projetos]**
1. Na seção [!UICONTROL Status do projeto], encontre [!UICONTROL Método de índice de desempenho]. Selecione Baseado em horas ou Baseado em custos.
1. Em [!UICONTROL Estimativa de conclusão], selecione Calcular no nível do projeto ou Total das tarefas e subtarefas.
1. Clique em **[!UICONTROL Salvar]** na parte inferior da janela.

![Uma imagem da tela [!UICONTROL Preferências do projeto]](assets/setting-up-finances-1.png)

**Definir o [!UICONTROL PIM] em projetos individuais**

1. Acesse a página de destino de um projeto.
1. Clique em **[!UICONTROL Detalhes do projeto]** no painel esquerdo.
1. Abra a seção **[!UICONTROL Finanças]**.
1. Clique duas vezes no texto abaixo de **[!UICONTROL Método de índice de desempenho]** para editá-lo.
1. Selecione Baseado em horas ou Baseado em custos.
1. Clique em **[!UICONTROL Salvar alterações]** para finalizar.

![Uma imagem da tela [!UICONTROL Detalhes do projeto]](assets/setting-up-finances-2.png)

O [!UICONTROL PIM] pode ser definido para um modelo de projeto na seção [!UICONTROL Finanças] dos detalhes do modelo.
