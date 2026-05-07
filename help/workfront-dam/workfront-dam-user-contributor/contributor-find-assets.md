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
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:25:54.114Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 407
ht-degree: 89%

---

# Entenda a pesquisa de ativos como colaborador

Neste vídeo, você aprenderá a:

* Pesquisar ativos
* Pesquisar em pastas
* Simplifique os resultados da pesquisa
* Use metadados e palavras-chave como filtros de pesquisa
* Exiba detalhes da pasta
* Exiba e atualize metadados e palavras-chave de ativos

>[!VIDEO](https://video.tv.adobe.com/v/3453926/?captions=por_br&quality=12&learn=on&enablevpops=1)

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

Para localizar ativos que não têm informações em um campo de metadados específico, insira o campo que deseja pesquisar neste formato: ?[xxxxx]. Por exemplo, se você deseja encontrar ativos que não têm palavras-chave atribuídas, digite ?[palavra-chave] no campo de pesquisa.
