---
title: Localizar e organizar ativos em [!UICONTROL Workfront DAM]
description: Saiba como pesquisar ativos, pesquisar em pastas, simplificar resultados de pesquisa, usar metadados e palavras-chave como filtros de pesquisa e muito mais em [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
source-git-commit: d1f5c4a558f737cb8188e209a16b91b67d32285c
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

Uma pesquisa básica observa nomes de arquivo, campos de metadados, palavras-chave e conteúdo do ativo (dependendo do tipo de ativo). Ela não inclui o nome da pasta.

A maioria dos resultados da pesquisa são correspondências exatas. Uma exceção para essa regra de &quot;correspondência exata&quot; é quando a variável [!UICONTROL Workfront DAM] pesquisa o campo filename . [!UICONTROL Workfront DAM] retorna correspondências de nome de arquivo parciais, em vez de apenas correspondências exatas de nome de arquivo.

## Operadores de usuário ao pesquisar

Embora os recursos básicos de pesquisa frequentemente encontrem os ativos necessários, talvez seja necessário usar outros parâmetros de pesquisa ocasionalmente.

### Correspondências parciais

Para encontrar uma correspondência parcial, adicione um asterisco ao termo de pesquisa. O asterisco só pode ser usado no final de uma palavra.

### Operador AND

Para encontrar resultados contendo vários termos de pesquisa, insira E entre as palavras. As palavras podem ser encontradas em qualquer ordem. Ao pesquisar em todos os campos, ambas as palavras podem não estar presentes no mesmo campo. Por exemplo, Paris E torre encontrarão ativos que têm ambas as palavras em qualquer um dos campos.

### Operador OR

Use o operador OU para localizar ativos que contenham qualquer um dos termos de pesquisa. Por exemplo, Paris OU Arco encontrará ativos que tenham uma das palavras, mas não necessariamente ambas.

### Frase

Para encontrar uma frase exata, use aspas duplas ao redor das palavras. Todas as palavras serão encontradas juntas e em ordem. Por exemplo, &quot;Torre Eiffel&quot; encontrará essas palavras na ordem exata.

### Operador negativo

Se desejar excluir uma palavra dos resultados da pesquisa, coloque um sinal de menos (-) na frente da palavra. Certifique-se de que não haja um espaço entre o sinal de menos e a palavra. Por exemplo, para excluir ativos que têm a palavra &quot;torre&quot; nos metadados, sua pesquisa pode ser configurada como torre de Paris.

### Operador de campo vazio

Para localizar ativos que não tenham informações em um campo de metadados específico, insira o campo que deseja pesquisar nesse formato: ?[xxxxx]. Por exemplo, se você deseja encontrar ativos que não têm palavras-chave atribuídas, digite ?[palavra-chave] no campo de pesquisa.
