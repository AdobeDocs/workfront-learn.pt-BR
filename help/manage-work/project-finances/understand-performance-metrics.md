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
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '433'
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
