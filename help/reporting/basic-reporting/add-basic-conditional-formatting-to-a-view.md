---
title: Adicionar formatação condicional básica
description: Saiba como usar as regras de coluna para alterar a cor do texto, a formatação e as cores do plano de fundo em um relatório ou exibição, com base nos critérios definidos.
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Adicionar formatação condicional básica a uma exibição

A formatação condicional é feita criando regras de coluna. As regras de coluna permitem formatar uma coluna de uma maneira específica com base nos critérios definidos.

Neste vídeo, você aprenderá:

* O que é formatação condicional em uma exibição
* Como criar e modificar a formatação condicional

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12)

## Atividade: adicionar formatação condicional a uma exibição

Crie uma exibição de tarefa chamada &quot;Padrão + Progresso&quot; usando a exibição Padrão existente e adicionando essa formatação condicional no [!UICONTROL Nome] coluna.

1. Adicione uma regra de coluna que tornará o campo vermelho em segundo plano quando o status de progresso da tarefa for Late.
1. Adicione uma regra de coluna que tornará o plano de fundo do campo amarelo quando o status do progresso estiver Atrás ou Em Risco.

Isso ajudará você a detectar tarefas com problemas sem incluir a coluna de status do progresso como parte da visualização.

## Resposta

![Uma imagem da tela para criar uma nova regra de coluna](assets/conditional-formatting-exercise.png)

1. Em um relatório de lista de tarefas, vá para a **[!UICONTROL Exibir]** e selecione **[!UICONTROL Nova visualização]**.
1. Nomeie sua visualização como &quot;Padrão + Progresso&quot;.
1. Use as colunas padrão fornecidas.
1. Selecione o [!UICONTROL Nome da tarefa] coluna. Essa é a coluna à qual você deseja aplicar a formatação condicional, para que apareça vermelha ou amarela se o status de progresso da tarefa não for No Prazo.
1. Clique em **[!UICONTROL Opções avançadas]** no canto superior direito da janela do report builder.
1. Clique em **[!UICONTROL Adicionar uma Regra para esta Coluna]**.
1. Iniciar a regra de coluna alterando [!UICONTROL Tarefa] > [!UICONTROL Nome] na parte superior da janela para [!UICONTROL Tarefa] > [!UICONTROL Status do progresso]. Basta clicar no link **[!UICONTROL X]** ícone ao lado de [!UICONTROL Tarefa] > [!UICONTROL Nome] para excluí-lo do campo.
1. Digite &quot;progress&quot; no campo e selecione [!UICONTROL Status do progresso] no [!UICONTROL Tarefa] origem do campo.
1. Selecionar **[!UICONTROL Atrasado]** no campo à direita da [!UICONTROL Igual] qualificador.
1. Escolha um plano de fundo vermelho no [!UICONTROL Cor do texto] linha.
1. Clique em **[!UICONTROL Adicionar regra]** para salvar a regra de coluna.
1. Agora clique em **[!UICONTROL Adicionar regra de coluna]** novamente para adicionar outra regra.
1. Assim como antes, excluir [!UICONTROL Tarefa] > [!UICONTROL Nome] no campo de critérios. Substituir por [!UICONTROL Status do progresso] no [!UICONTROL Tarefa] origem do campo.
1. Selecionar ambos [!UICONTROL Em Risco] e [!UICONTROL Atrás] no campo à direita do qualificador Equal.
1. Escolha um fundo amarelo no [!UICONTROL Cor do texto] linha.
1. Clique em **[!UICONTROL Adicionar regra]** para salvar a regra de coluna.
1. Clique em **[!UICONTROL Salvar visualização]** para salvar a visualização.
