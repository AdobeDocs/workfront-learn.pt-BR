---
title: Entender os filtros de problemas internos
description: Saiba como revisar filtros de problemas internos para ver como eles são criados e criar seu próprio filtro de problemas no [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336819.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9085
exl-id: c1bdea98-e70a-4e93-935c-b8f7754afa21
source-git-commit: 83c7379a5398c78cea31a4571b34fd5b64bce027
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Entender os filtros de problemas internos

Neste vídeo, você:

* Analise os filtros de problemas internos para ver como eles são criados
* Saiba mais sobre alguns elementos úteis de relatório de problemas
* Saiba como criar seu próprio filtro de problemas

>[!VIDEO](https://video.tv.adobe.com/v/336819/?quality=12)

## Atividade: Criar um relatório de problemas

Você deseja ver todos os problemas que ainda precisam ser resolvidos em todos os projetos ativos de sua propriedade, incluindo problemas com um objeto de resolução. Crie um relatório de problema e o nomeie como &quot;Problemas não resolvidos em projetos que eu possuo&quot;.

## Resposta

Veja como o filtro deve ser:

![Uma imagem da tela para criar um filtro de problema](assets/opening-built-in-issue-filters-1.png)

No filtro interno &quot;Meus problemas em aberto&quot;, uma das regras de filtro excluía quaisquer problemas em que houvesse um objeto de resolução. O raciocínio por trás disso é que você não precisa se preocupar com esses problemas. Alguém já criou um projeto, tarefa ou problema que os resolverá, então o que é que se preocupar? Mas eles ainda não foram resolvidos e, em nosso exemplo, estamos incluindo eles para facilitar a identificação e a verificação de como estão.

Para fazer isso, é necessário adicionar uma coluna na guia view para &quot;Issue > Resolving Object&quot;. Isso mostra o nome do objeto de resolução, se houver, se for um projeto, tarefa ou problema. Clicar no nome leva você ao objeto de resolução.

Talvez você queira agrupar a lista com base no nome do projeto.

É assim que o relatório deve ser:

![Uma imagem de um relatório de ocorrência](assets/opening-built-in-issue-filters-2.png)
