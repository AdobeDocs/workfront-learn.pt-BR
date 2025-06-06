---
title: Entenda a pesquisa de ativos como colaborador
description: Saiba como pesquisar por ativos, pesquisar em pastas, otimizar resultados de pesquisa, usar metadados e palavras-chave como filtros de pesquisa no [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '407'
ht-degree: 100%

---

# Entenda a pesquisa de ativos como colaborador

Neste vídeo, você aprenderá a:

* Pesquisar ativos
* Pesquisar em pastas
* Simplifique os resultados da pesquisa
* Use metadados e palavras-chave como filtros de pesquisa
* Exiba detalhes da pasta
* Exiba e atualize metadados e palavras-chave de ativos

>[!VIDEO](https://video.tv.adobe.com/v/3453926/?quality=12&learn=on&enablevpops&captions=por_br)

## Critérios de pesquisa básica

Uma pesquisa básica analisa nomes de arquivos, campos de metadados, palavras-chave e o conteúdo de ativos (dependendo do tipo de ativo). Não inclui o nome da pasta.

A maioria dos resultados da pesquisa são correspondências exatas. Uma exceção a essa regra de “correspondência exata” ocorre quando o [!UICONTROL Workfront DAM] pesquisa o campo de nome do arquivo. O [!UICONTROL Workfront DAM] retorna correspondências parciais de nome de arquivo, em vez de apenas correspondências exatas.

## Operadores de usuário ao pesquisar

Embora os recursos básicos de pesquisa geralmente encontrem os ativos necessários, pode ser necessário usar parâmetros de pesquisa adicionais de vez em quando.

### Correspondências parciais

Para encontrar uma correspondência parcial, adicione um asterisco ao termo de pesquisa. O asterisco só pode ser usado no fim de uma palavra.

### Operador E

Para encontrar resultados que contenham vários termos de pesquisa, insira E entre as palavras. As palavras podem ser encontradas em qualquer ordem. Ao pesquisar em todos os campos, ambas as palavras podem não estar presentes no mesmo campo. Por exemplo, “Paris E torre” encontrará ativos que contenham essas palavras em qualquer um dos campos.

### Operador OU

Use o operador OU para localizar ativos que contenham qualquer um dos termos de pesquisa. Por exemplo, “Paris OU Arco” encontrará ativos que contêm uma das palavras, mas não necessariamente as duas.

### Frase

Para encontrar uma frase exata, use aspas duplas ao redor das palavras. Todas as palavras serão encontradas juntas e na ordem definida. Por exemplo, “Torre Eiffel” encontrará essas palavras nessa ordem exata.

### Operador negativo

Se quiser excluir uma palavra dos resultados da pesquisa, coloque um sinal de menos (–) antes da palavra. Certifique-se de que não haja espaço entre o sinal de menos e a palavra. Por exemplo, para excluir ativos que contenham a palavra “torre” dos metadados, a pesquisa pode ter a seguinte aparência: “Paris -torre”.

### Operador de campo vazio

Para localizar ativos que não têm informações em um campo de metadados específico, insira o campo que deseja pesquisar neste formato: ?[xxxxx]. Por exemplo, se quiser encontrar ativos que não tenham palavras-chave atribuídas, insira a[palavra-chave] no campo de pesquisa.
