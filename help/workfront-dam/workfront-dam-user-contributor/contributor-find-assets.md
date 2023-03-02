---
title: Localizar e organizar ativos no [!UICONTROL DAM DO WORKFRONT]
description: Saiba como pesquisar ativos, pesquisar em pastas, simplificar resultados de pesquisa, usar metadados e palavras-chave como filtros de pesquisa e muito mais em [!UICONTROL DAM DO WORKFRONT].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Colaborador: localizar ativos

Neste vídeo, você aprenderá a:

* Pesquisar por ativos
* Pesquisar nas pastas
* Simplifique os resultados da pesquisa
* Usar metadados e palavras-chave como filtros de pesquisa
* Exibir detalhes da pasta
* Exibir e atualizar metadados e palavras-chave de ativos

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12)

## Critérios básicos de pesquisa

Uma pesquisa básica analisa nomes de arquivos, campos de metadados, palavras-chave e conteúdo de ativos (dependendo do tipo de ativo). Ela não inclui o nome da pasta.

A maioria dos resultados da pesquisa corresponde exatamente a. Uma exceção a essa regra de &quot;correspondência exata&quot; é quando a variável [!UICONTROL DAM DO WORKFRONT] pesquisa o campo nome do arquivo. [!UICONTROL DAM DO WORKFRONT] retorna correspondências parciais de nome de arquivo, em vez de apenas correspondências exatas de nome de arquivo.

## Operadores do usuário ao pesquisar

Embora os recursos básicos de pesquisa geralmente encontrem os ativos necessários, pode ser necessário usar parâmetros de pesquisa adicionais de tempos em tempos.

### Combinações parciais

Para localizar uma correspondência parcial, adicione um asterisco ao termo de pesquisa. O asterisco só pode ser usado no final de uma palavra.

### Operador AND

Para localizar resultados contendo vários termos de pesquisa, digite E entre as palavras. As palavras podem ser encontradas em qualquer ordem. Ao pesquisar em todos os campos, ambas as palavras podem não estar presentes no mesmo campo. Por exemplo, Paris E torre encontrarão ativos que tenham ambas essas palavras em qualquer um dos campos.

### Operador OR

Use o operador OU para localizar ativos que contenham qualquer um dos termos de pesquisa. Por exemplo, Paris OU Arco encontrará ativos que têm uma das palavras, mas não necessariamente as duas.

### Frase

Para encontrar uma frase exata, use aspas duplas ao redor das palavras. Todas as palavras serão encontradas juntas e em ordem. Por exemplo, &quot;Torre Eiffel&quot; encontrará essas palavras nessa ordem exata.

### Operador negativo

Se quiser excluir uma palavra dos resultados da pesquisa, coloque um sinal de menos (-) na frente da palavra. Verifique se não há um espaço entre o sinal de menos e a palavra. Por exemplo, para excluir ativos que tenham a palavra &quot;torre&quot; nos metadados, sua pesquisa pode ser configurada como Paris -tower.

### Operador de campo vazio

Para localizar ativos que não têm informações em um campo de metadados específico, insira o campo que deseja pesquisar neste formato: ?[xxxxx]. Por exemplo, se você deseja localizar ativos que não têm palavras-chave atribuídas, insira?[palavra-chave] no campo de pesquisa.
