---
title: Ferramenta Dev
description: Aprimore suas capacidades de solucionar problemas de um cenário e facilitar configurações complexas usando a DevTool.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11057
thumbnail: KT11057.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---


# Ferramenta Dev

Melhore suas capacidades de solucionar problemas em um cenário e aliviar configurações complexas usando a ferramenta Dev.

## Visão geral do exercício

Instale e use as diferentes áreas na ferramenta Workfront Dev para aprofundar as solicitações/respostas feitas e os truques avançados de design de cenário.

>[!NOTE]
>
>A ferramenta Workfront Fusion Dev só está disponível no navegador Chrome ao usar o [Ferramenta de desenvolvedor do Chrome](https://developer.chrome.com/docs/devtools/).

![Imagem do Devtool 1](../12-exercises/assets/devtool-walkthrough-1.png)

## Etapas a seguir

**Instale a ferramenta Dev.**

1. Baixe o documento &quot;workfront-fusion-devtool.zip&quot; encontrado na pasta Fusion Exercise Files na unidade de teste.
1. Extraia os arquivos Zip para uma pasta.
1. Abra uma guia no Chrome e digite **chrome://extensions**.
1. Ative o modo Desenvolvedor usando o switch na parte superior direita e clique no botão &quot;Carregar descompactado&quot; que aparece na parte superior esquerda. Selecione a pasta que contém a ferramenta Dev (este é o local onde você a descompactou).

   ![Imagem do Devtool 2](../12-exercises/assets/devtool-walkthrough-2.png)

1. Depois de descompactada, a ferramenta de Desenvolvimento aparecerá entre suas outras extensões.

   ![Imagem do Devtool 3](../12-exercises/assets/devtool-walkthrough-3.png)

   **Use o Live Stream.**

1. Comece abrindo o cenário &quot;Usando Data Stores para sincronizar dados&quot;.
1. Abra a ferramenta Dev digitando F12 ou a função F12. Ou você pode clicar no menu de três pontos na barra de endereços do Chrome e navegar até Ferramentas do desenvolvedor.

   ![Imagem do Devtool 4](../12-exercises/assets/navigate-to-devtools.png)

1. Clique na guia Workfront Fusion e selecione Live Stream na lista à esquerda.
1. Clique em Executar uma vez para ver os eventos como ocorrem.
1. Clique em um evento para ver as guias à direita para Cabeçalhos de solicitação, Corpo da solicitação, Cabeçalhos de resposta e Corpo de resposta.

   ![Imagem do Devtool 4](../12-exercises/assets/devtool-walkthrough-4.png)

   **Usar o depurador de cenário**

1. Selecione Depurador de Cenário e clique em um módulo para ver informações sobre as operações desse módulo.

   ![Imagem do Devtool 5](../12-exercises/assets/devtool-walkthrough-5.png)

1. Navegue até a guia Histórico . Clique em Details on an execution para examinar os detalhes da operação do módulo para uma execução específica.

   ![Imagem do Devtool 6](../12-exercises/assets/devtool-walkthrough-6.png)

   **Usar as ferramentas**

1. Volte para o designer de cenário e selecione Ferramentas na ferramenta Dev. Isso exibe as ferramentas disponíveis.

   ![Imagem do Devtool 7](../12-exercises/assets/devtool-walkthrough-7.png)

+ Foco em um módulo - Localize e abra um módulo rapidamente usando a ID do módulo.
+ Localizar módulos por mapeamento - Pesquise um cenário usando uma palavra-chave para localizar valores e/ou chaves mapeadas em módulos.
+ Obter metadados do aplicativo - Consulte os metadados do aplicativo selecionado em um cenário.
+ Copiar mapeamento - copia o mapeamento de um módulo para outro. Você também pode clonar o módulo no designer.
+ Copiar filtro - Copia um filtro. O filtro é sempre atribuído ao módulo à direita.
+ Trocar conexão - a ferramenta pega a conexão do módulo selecionado e define a mesma conexão com todos os módulos do mesmo aplicativo no cenário. Isso é útil se você precisar alterar a conexão em um cenário concluído. Evite perder todo o mapeamento e economize tempo usando essa ferramenta.
+ Variável de troca - Localiza todas as ocorrências da variável fornecida em todo o cenário ou em um módulo e as substitui pelo novo. Não há suporte para curingas. Se você tiver mapeado acidentalmente um valor em todo o cenário, isso pode ajudá-lo a trocar facilmente o valor correto.
+ Trocar aplicativo - Troque o aplicativo especificado por outro.
+ Base 64 - Codifique os dados inseridos em Base64 ou decodifice Base64. Útil quando você deseja pesquisar dados específicos na solicitação codificada.
+ Copiar nome do módulo - Copia o nome do módulo selecionado para a área de transferência.
+ Remap Source (Fonte de mapeamento) - Altere a fonte de mapeamento de um módulo para outro. Primeiro, é necessário adicionar o módulo para usar como módulo de origem à rota em um cenário.
+ Migrar SO - feito especificamente para atualizar módulos Google Sheets (herdados) para a versão mais recente das Google Sheets. Ele adiciona uma nova versão do módulo logo após a versão herdada do módulo na rota de cenário.
