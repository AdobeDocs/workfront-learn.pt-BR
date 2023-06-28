---
title: Ferramenta de desenvolvimento
description: Melhore suas habilidades para solucionar problemas de um cenário e facilitar configurações complexas usando o DevTool.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11057
thumbnail: KT11057.png
exl-id: 13080212-26cf-4e5f-8f0b-fc59a6f66eb1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Ferramenta de desenvolvimento

Aprimore suas habilidades para solucionar problemas de um cenário e facilitar configurações complexas usando a ferramenta Dev.

## Visão geral do exercício

Instale e use as diferentes áreas na ferramenta de Desenvolvimento do Workfront para aprofundar as solicitações/respostas feitas e os truques avançados de design de cenários.

>[!NOTE]
>
>A ferramenta Workfront Fusion Dev só está disponível no navegador Chrome ao usar o [Ferramenta de desenvolvedor do Chrome](https://developer.chrome.com/docs/devtools/).

![Devtool Imagem 1](../12-exercises/assets/devtool-walkthrough-1.png)

## Etapas a serem seguidas

**Instale a ferramenta Dev.**

1. Baixe o documento &quot;workfront-fusion-devtool.zip&quot; encontrado na pasta Arquivos do Fusion Exercise na unidade de teste.
1. Extraia os arquivos Zip para uma pasta.
1. Abra uma guia no Chrome e insira **chrome://extensions**.
1. Alterne para o modo Desenvolvedor usando o switch no canto superior direito e clique no botão &quot;Carregar desempacotado&quot; que aparece no canto superior esquerdo. Selecione a pasta que contém a ferramenta Dev (foi aqui que você a descompactou).

   ![Devtool Imagem 2](../12-exercises/assets/devtool-walkthrough-2.png)

1. Depois de descompactada, a ferramenta de Desenvolvimento é exibida entre suas outras extensões.

   ![Devtool Imagem 3](../12-exercises/assets/devtool-walkthrough-3.png)

   **Use o Live Stream.**

1. Comece abrindo o cenário &quot;Usando armazenamentos de dados para sincronizar dados&quot;.
1. Abra a ferramenta Dev digitando F12 ou a função F12. Ou você pode clicar no menu de três pontos na barra de endereços do Chrome e navegar até Ferramentas do desenvolvedor.

   ![Devtool Imagem 4](../12-exercises/assets/navigate-to-devtools.png)

1. Clique na guia Workfront Fusion e selecione Live Stream na lista à esquerda.
1. Clique em Executar uma vez para ver os eventos à medida que ocorrem.
1. Clique em um evento para ver as guias à direita para Cabeçalhos de solicitação, Corpo de solicitação, Cabeçalhos de resposta e Corpo de resposta.

   ![Devtool Imagem 4](../12-exercises/assets/devtool-walkthrough-4.png)

   **Usar o Scenario Debugger**

1. Selecione Scenario Debugger e clique em um módulo para ver informações sobre as operações desse módulo.

   ![Devtool Imagem 5](../12-exercises/assets/devtool-walkthrough-5.png)

1. Clique na guia Histórico. Clique em Detalhes em uma execução para examinar os detalhes da operação do módulo para uma execução específica.

   ![Devtool Imagem 6](../12-exercises/assets/devtool-walkthrough-6.png)

   **Usar as Ferramentas**

1. Volte para o designer de cenários e selecione Ferramentas na ferramenta Desenvolvimento. Isso exibe as ferramentas disponíveis.

   ![Devtool Imagem 7](../12-exercises/assets/devtool-walkthrough-7.png)

+ Focar em um módulo - Encontre e abra um módulo rapidamente usando a ID do módulo.
+ Localizar módulo(s) por mapeamento - Pesquise um cenário usando uma palavra-chave para localizar valores e/ou chaves mapeados em módulos.
+ Obter metadados do aplicativo - Veja os metadados do aplicativo selecionado em um cenário.
+ Copiar mapeamento - Copia o mapeamento de um módulo para outro. Você também pode clonar o módulo no designer.
+ Copiar filtro - Copia um filtro. O filtro é sempre atribuído ao módulo à direita.
+ Trocar conexão - A ferramenta pega a conexão do módulo selecionado e define a mesma conexão para todos os módulos do mesmo aplicativo no cenário. Isso é útil se você precisar alterar a conexão em um cenário concluído. Evite perder todo o mapeamento e economize tempo usando essa ferramenta.
+ Variável de troca - Localiza todas as ocorrências da variável fornecida em todo o cenário ou em um módulo e as substitui pela nova. Não há suporte para curingas. Se você tiver mapeado acidentalmente um valor durante todo o cenário, isso pode ajudá-lo a trocar facilmente pelo valor correto.
+ Trocar aplicativo - Troca o aplicativo fornecido por outro.
+ Base 64 - Codifique os dados inseridos em Base64 ou decodifique Base64. Útil quando você deseja pesquisar por dados específicos na solicitação codificada.
+ Copiar nome do módulo - Copia o nome do módulo selecionado para a área de transferência.
+ Remapear origem - Altere a origem do mapeamento de um módulo para outro. Você precisa primeiro adicionar o módulo a ser usado como um módulo de origem para a rota em um cenário.
+ Migrar SO - feito especificamente para atualizar os módulos do Google Sheets (herdados) para a versão mais recente do Google Sheets. Ele adiciona uma nova versão do módulo logo após a versão herdada do módulo na rota do cenário.
