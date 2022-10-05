---
title: Entender as métricas de desempenho
description: As métricas de desempenho são as [!UICONTROL Método do Índice de Desempenho] ([!UICONTROL PIM]) e o [!UICONTROL Estimativa na conclusão] ([!UICONTROL EAC]).
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Entender as métricas de desempenho

Duas métricas de desempenho usadas pelos gerentes de projeto incluem o [!UICONTROL Método do Índice de Desempenho] ([!UICONTROL PIM]) e o [!UICONTROL Estimativa na conclusão] ([!UICONTROL EAC]). Os padrões de todo o sistema podem ser definidos em [!DNL Workfront] e se aplicam a projetos recém-criados. [!UICONTROL PIM] pode ser modificado em projetos individuais.

**[!UICONTROL MID]**

As configurações do [!UICONTROL PIM] controlar como [!DNL Workfront] O calcula outras métricas de desempenho do projeto, como a variável [!UICONTROL Índice de desempenho de custo] ([!UICONTROL CPI]), [!UICONTROL Índice de Desempenho da Programação de Custo] ([!UICONTROL CSI]), [!UICONTROL Índice de desempenho agendado] ([!UICONTROL SPI]), e [!UICONTROL Estimativa na conclusão] ([!UICONTROL EAC]).

Opções para o [!UICONTROL PIM] são baseadas em hora e em custo.

* **Baseado em hora** — O Workfront utiliza as horas planejadas para calcular o IPC e o EAC do projeto. O EAC do projeto é exibido como um número, em horas.
* **Baseado em custos** — A Workfront utiliza o custo da mão de obra planejado para calcular o IPC e o EAC do projeto. EAC é exibido como um valor de moeda. Ao usar essa opção, verifique se os destinatários da tarefa (usuários e/ou funções de trabalho) estão associados a taxas de custo.

**[!UICONTROL EAC]**

[!UICONTROL EAC] representa o custo total projetado da sua tarefa ou projeto quando ele é concluído. As opções são calculadas em nível de projeto e acumuladas a partir de tarefas/subtarefas.

* **Calcular no nível do projeto** — [!UICONTROL EAC] para a tarefa-mãe e o projeto são determinados utilizando as horas reais/custos reais da mão de obra em [!UICONTROL EAC] fórmulas. O cálculo inclui horas/custos e despesas reais adicionados diretamente à tarefa pai ou ao projeto.
* R **Fazer logoff de tarefas/subtarefas** — [!UICONTROL EAC] para a tarefa pai e o projeto são determinados adicionando a variável [!UICONTROL EAC] para cada tarefa filho. Esse cálculo exclui horas/custos reais adicionados diretamente a uma tarefa ou projeto pai.

O [!UICONTROL EAC] os cálculos são listados em &quot;Calcular Estimativa na Conclusão (EAC)&quot; <!-- link to article -->artigo sobre [!UICONTROL [!DNL Workfront] One].

**Métricas de desempenho: Configurações**

Para definir [!UICONTROL PIM] e [!UICONTROL EAC] padrões do sistema:

1. Selecionar **[!UICONTROL Configuração]** no menu principal.
1. Clique em **[!UICONTROL Preferências do projeto]** no menu do painel esquerdo, em seguida, clique em **[!UICONTROL Projetos]**
1. No [!UICONTROL Status do projeto] seção, localizar [!UICONTROL Método do Índice de Desempenho]. Selecione Baseado em horas ou em custo.
1. Para [!UICONTROL Estimativa na conclusão], selecione Calcular no nível do projeto ou Rolar de tarefas/subtarefas.
1. Clique em **[!UICONTROL Salvar]** na parte inferior da janela.

![Uma imagem da [!UICONTROL Preferências do projeto] tela](assets/setting-up-finances-1.png)

**Definir [!UICONTROL PIM] sobre projetos individuais**

1. Vá para a landing page de um projeto.
1. Clique em **[!UICONTROL Detalhes do projeto]** no painel esquerdo.
1. Abra o **[!UICONTROL Finanças]** seção.
1. Clique duas vezes no texto abaixo **[!UICONTROL Método do Índice de Desempenho]** para editá-lo.
1. Selecione Baseado em horas ou em custo.
1. Clique em **[!UICONTROL Salvar]** Mudanças para terminar.

![Uma imagem da [!UICONTROL Detalhes do projeto] tela](assets/setting-up-finances-2.png)

[!UICONTROL PIM] pode ser definido em um modelo de projeto, no [!UICONTROL Finanças] seção dos detalhes do template.
