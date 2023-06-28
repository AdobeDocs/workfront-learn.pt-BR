---
title: Webhooks
description: Saiba como criar, acionar e gerenciar cenários iniciados por webhook.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Webhooks

Saiba como criar, acionar e gerenciar cenários iniciados por webhook.

## Visão geral do exercício

O objetivo deste cenário é criar um aplicativo para vender para lojas de conveniência, para que possam determinar facilmente se um cliente tem idade suficiente para comprar álcool. O operador de caixa precisa apenas postar o nome e a data de nascimento do cliente em um URL fornecido. Essa publicação acionará o cenário que calculará a resposta e a retornará ao solicitante.

1. O cenário consiste em três webhooks.
1. O módulo acionador é um webhook personalizado que escuta uma publicação.
1. Ao receber um post, ele o direcionará para um dos próximos módulos.
1. O módulo seguinte retorna uma resposta ao solicitante.

   ![Webhooks Imagem 1](../12-exercises/assets/webhooks-walkthrough-1.png)

## Etapas a serem seguidas

**Configure o webhook do acionador.**

1. Crie um novo cenário e nomeie-o como &quot;Usando webhooks&quot;.
1. Para o acionador, adicione o módulo Webhook personalizado no aplicativo Webhooks.
1. Clique em Adicionar para criar um novo Webhook.
1. Insira o nome do Webhook de &quot;Aplicativo de idade de consumo&quot;.
1. Deixe as restrições de IP em branco, o que significa que qualquer pessoa pode enviar dados para ele.
1. Clique em Salvar.


   ![Imagem 2 do Webhooks](../12-exercises/assets/webhooks-walkthrough-2.png)

1. De volta ao painel de mapeamento Webhooks, um URL foi criado para este webhook específico. Clique em &quot;Copiar endereço para a área de transferência&quot; para copiar esse URL.
1. Clique em OK.
1. Clique em Executar uma vez.
1. Use o URL no Postman para enviar um nome e uma data de nascimento para seu webhook personalizado. Para obter instruções sobre como configurar o Postman, consulte [Apresentação dos Webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=en) tutorial.

   **O painel do módulo Webhooks deve ter esta aparência:**

   ![Imagem 3 do Webhooks](../12-exercises/assets/webhooks-walkthrough-3.png)

   **O webhook agora está em um estado em que escuta os dados para determinar a estrutura de dados.**

1. Você pode definir a estrutura de dados do payload que espera obter (as estruturas de dados serão discutidas posteriormente). Se você não definir uma estrutura de dados, o Fusion determinará a estrutura de dados automaticamente quando a publicação for enviada.
1. No lado do Postman, você deseja enviar para o URL copiado. A publicação deve incluir dados básicos do formulário. Para este exemplo, você precisa de três campos: Nome, Data de nascimento e clientToken.

   ![Webhooks Imagem 4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. Depois de clicar em Enviar do Postman, você deve receber uma indicação de que a publicação foi aceita.
1. Esse é o ponto em que o cenário mostrará que a estrutura de dados foi determinada com sucesso.
1. Você pode ver que os dados foram recebidos abrindo o inspetor de execução.

   ![Imagem 5 do Webhooks](../12-exercises/assets/webhooks-walkthrough-5.png)

   **Configurar roteamento para tokens de cliente.**

1. Adicione um roteador ao módulo de acionamento.
1. No caminho superior, adicione um módulo de resposta do Webhook. Esse será o nosso caminho para quando o token do cliente não corresponder.
1. Defina o status como 401.
1. Defina o corpo como {&quot;error&quot;: &quot;Failed to authenticate request. Verifique seu clientToken&quot;}.

   ![Imagem 6 do Webhooks](../12-exercises/assets/webhooks-walkthrough-6.png)

1. Crie um filtro entre o roteador e o módulo de resposta do Webhook. Nomeie de &quot;O token do cliente não corresponde&quot;.
1. Para a Condição, use o campo clientToken do módulo do acionador e faça uma comparação numérica &quot;Not equal to&quot; com o número 5121933.

   ![Imagem 7 do Webhooks](../12-exercises/assets/webhooks-walkthrough-7.png)

1. No caminho inferior, adicione outro módulo de resposta do Webhook. Esse será o nosso caminho para quando o token do cliente corresponder.
1. Defina o status como 200.
1. Ao configurar o Corpo, use as funções do painel de mapeamento para testar se a pessoa tem 21 anos ou mais. Se forem, devolva &quot;Você tem idade suficiente para beber!&quot;, caso contrário devolva &quot;Você está sem sorte...&quot;

   ![Imagem 9 do Webhooks](../12-exercises/assets/webhooks-walkthrough-9.png)

1. Crie um filtro entre o roteador e o módulo de resposta do Webhook no caminho inferior. Nomeie de &quot;O token do cliente corresponde&quot;.
1. Para a Condição, use o campo clientToken do módulo do acionador e faça uma comparação numérica &quot;Igual a&quot; com o número 5121933.


   ![Imagem 8 do Webhooks](../12-exercises/assets/webhooks-walkthrough-8.png)

1. Clique no botão Scheduling (Agendamento) em Run once (Executar uma vez) para ativar o cenário e, a qualquer momento, receber uma nova publicação, percorrer qualquer um dos caminhos e gerar uma resposta.
