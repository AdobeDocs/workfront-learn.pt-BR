---
title: Exercício sobre webhooks
description: Saiba como criar, acionar e gerenciar cenários iniciados por webhook.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
recommendations: noDisplay,catalog
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Exercício sobre webhooks

Saiba como criar, acionar e gerenciar cenários iniciados por webhook.

## Visão geral do exercício

O objetivo deste cenário é criar um aplicativo a ser vendido para lojas de conveniência para que elas possam determinar facilmente se um(a) cliente tem ou não idade suficiente para comprar bebidas alcoólicas. O(a) operador(a) do caixa precisa apenas registrar o nome e a data de nascimento do(a) cliente em um URL fornecido. Isso acionará o cenário que calculará a resposta e a retornará ao solicitante.

1. O cenário consiste em três webhooks.
1. O módulo acionador é um webhook personalizado que escuta a publicação.
1. Ao receber uma publicação, ela será enviada para um dos próximos módulos.
1. O módulo seguinte retorna uma resposta ao solicitante.

   ![Webhooks - Imagem 1](../12-exercises/assets/webhooks-walkthrough-1.png)

## Etapas a serem seguidas

**Configure o webhook do acionador.**

1. Crie um novo cenário e nomeie-o como “Usar webhooks”.
1. Para o acionador, adicione o módulo de webhook personalizado do aplicativo Webhooks.
1. Clique em Adicionar para criar um novo webhook.
1. Digite o nome de webhook “Aplicativo de idade para beber”.
1. Deixe as restrições de IP em branco, o que significa que qualquer pessoa pode enviar dados para ele.
1. Clique em Salvar.


   ![Webhooks - Imagem 2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. De volta ao painel de mapeamento de webhooks, um URL foi criado para este webhook específico. Clique em “Copiar endereço para a área de transferência” para copiar esse URL.
1. Clique em OK.
1. Clique em Executar uma vez.
1. Use o URL no Postman para enviar um nome e data de nascimento para seu webhook personalizado. Para obter instruções sobre como configurar o Postman, consulte o tutorial [Passo a passo dos webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=pt-BR).

   **O painel do módulo Webhooks deve ter esta aparência:**

   ![Webhooks - Imagem 3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **O webhook agora estará acompanhando os dados para determinar a estrutura deles.**

1. Você pode definir a estrutura de dados do conteúdo que espera obter (as estruturas de dados serão discutidas posteriormente). Se você não definir uma estrutura de dados, o Fusion determinará a estrutura de dados automaticamente quando a publicação for enviada.
1. No Postman, envie para o URL copiado. A publicação deve incluir dados básicos de formulário. Para este exemplo, você precisa de três campos: Nome, Data de nascimento e clientToken.

   ![Webhooks - Imagem 4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. Depois de clicar em Enviar do Postman, você deverá receber uma indicação de que a publicação foi aceita.
1. Esse é o ponto em que o cenário mostrará que a estrutura de dados foi determinada com sucesso.
1. Você pode ver que os dados foram recebidos abrindo o inspetor de execução.

   ![Webhooks - Imagem 5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **Configurar roteamento para tokens de cliente.**

1. Adicione um roteador ao módulo acionador.
1. No caminho superior, adicione um módulo de resposta de webhook. Esse será o nosso caminho para quando o token do cliente não corresponder.
1. Defina o status como 401.
1. Defina o corpo como {&quot;error&quot;: &quot;Failed to authenticate request.  Please check your clientToken&quot;}.

   ![Webhooks - Imagem 6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. Crie um filtro entre o roteador e o módulo de resposta do webhook. Nomeie-o como “O token de cliente não corresponde.”
1. Para a Condição, use o campo clientToken do módulo acionador e faça uma comparação numérica “Diferente de” com o número 5121933.

   ![Webhooks - Imagem 7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. No caminho inferior, adicione outro módulo de resposta de webhook. Esse será o nosso caminho para quando o token de cliente corresponder.
1. Defina o status como 200.
1. Ao configurar o Corpo, use as funções do painel de mapeamento para testar se a pessoa tem 21 anos ou mais. Se tiverem, retorne “Você tem idade suficiente para beber!”, caso contrário, retorne “Você está sem sorte…”

   ![Webhooks - Imagem 9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. Crie um filtro entre o roteador e o módulo de resposta do webhook no caminho inferior. Nomeie-o como “O token de cliente corresponde.”
1. Para a Condição, use o campo clientToken do módulo acionador e faça uma comparação numérica “Igual a” com o número 5121933.


   ![Webhooks - Imagem 8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. Clique no botão Agendamento em Executar uma vez para ativar seu cenário para que sempre que houver uma nova publicação ela seja recebida, siga qualquer caminho e gere uma resposta.
