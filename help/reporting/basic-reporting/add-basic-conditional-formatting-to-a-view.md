---
title: Adicionar formatação condicional básica
description: Neste vídeo, você aprenderá o que é formatação condicional em uma exibição e como criar e modificar a formatação condicional em [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
source-git-commit: b09d634a8b4ec32eda2663f1df04cc8bc04596a9
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Adicionar formatação condicional básica a uma exibição

Neste vídeo, você aprenderá:

* O que é formatação condicional em uma exibição
* Como criar e modificar a formatação condicional

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12)

## Atividade: Adicionar formatação condicional a uma exibição

Crie uma exibição de tarefa chamada &quot;Padrão + Andamento&quot; usando a exibição Padrão existente e adicionando essa formatação condicional à [!UICONTROL Nome] coluna.

1. Adicione uma regra de coluna que tornará o plano de fundo do campo vermelho quando o status do progresso da tarefa for Late.
1. Adicione uma regra de coluna que tornará o plano de fundo do campo amarelo quando o status do progresso estiver Atrás ou Em Risco.

Isso ajudará você a detectar tarefas com problemas sem incluir a coluna referente ao status do progresso como parte de sua visualização.

## Resposta

![Uma imagem da tela para criar uma nova regra de coluna](assets/conditional-formatting-exercise.png)

1. Em um relatório de lista de tarefas, acesse **[!UICONTROL Exibir]** e selecione **[!UICONTROL Nova exibição]**.
1. Nomeie sua exibição como &quot;Padrão + Progresso&quot;.
1. Use as colunas padrão fornecidas.
1. Selecione o [!UICONTROL Nome da tarefa] coluna. Essa é a coluna à qual você deseja aplicar a formatação condicional, de modo que ela aparecerá em vermelho ou amarelo se o status do progresso da tarefa não for Em tempo.
1. Clique em **[!UICONTROL Opções avançadas]** no canto superior direito da janela do construtor de relatórios.
1. Clique em **[!UICONTROL Adicionar uma regra para esta coluna]**.
1. Inicie a regra de coluna alterando [!UICONTROL Tarefa] > [!UICONTROL Nome] na parte superior da janela para [!UICONTROL Tarefa] > [!UICONTROL Status de progresso]. Basta clicar no botão **[!UICONTROL X]** ícone ao lado de [!UICONTROL Tarefa] > [!UICONTROL Nome] para excluí-lo do campo.
1. Digite &quot;progress&quot; no campo e selecione [!UICONTROL Status de progresso] nos termos do [!UICONTROL Tarefa] fonte do campo.
1. Selecionar **[!UICONTROL Atraso]** no campo à direita do [!UICONTROL Igual] qualificador.
1. Escolha um plano de fundo vermelho no [!UICONTROL Cor do texto] linha.
1. Clique em **[!UICONTROL Adicionar regra]** para salvar a regra da coluna.
1. Em seguida, clique em **[!UICONTROL Adicionar regra de coluna]** para adicionar outra regra.
1. Assim como antes, exclua [!UICONTROL Tarefa] > [!UICONTROL Nome] no campo de critérios. Substitua por [!UICONTROL Status de progresso] nos termos do [!UICONTROL Tarefa] fonte do campo.
1. Selecione ambos [!UICONTROL Em Risco] e [!UICONTROL Bebehind] no campo à direita do qualificador Equal .
1. Escolha um plano de fundo amarelo na [!UICONTROL Cor do texto] linha.
1. Clique em **[!UICONTROL Adicionar regra]** para salvar a regra da coluna.
1. Clique em **[!UICONTROL Salvar exibição]** para salvar a visualização.
