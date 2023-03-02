---
title: Criar e compartilhar um formulário personalizado
description: Saiba como criar um formulário personalizado, adicionar campos exclusivos ao formulário, organizar campos usando seções e lógica e compartilhar formulários com usuários.
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
thumbnail: 335172.png
kt: 8909
exl-id: b37334c7-67d0-4359-9537-dc26843582d1
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 5%

---

# Criar e compartilhar um formulário personalizado

Neste vídeo, você aprenderá a:

* Determine quais objetos usar para o formulário
* Adicionar campos exclusivos em vários formatos
* Organizar campos usando seções e lógica
* Compartilhar formulários com outros usuários

>[!VIDEO](https://video.tv.adobe.com/v/335172/?quality=12)

## Formulários personalizados funcionam com vários tipos de objetos

Ao clicar no botão [!UICONTROL Novo formulário personalizado] você pode selecionar quantos objetos quiser usar com um único formulário personalizado. Todos os campos adicionados a este formulário estarão disponíveis para qualquer um dos objetos selecionados quando o formulário personalizado for anexado a eles.

![Janela de formulário personalizado mostrando o [!UICONTROL Novo formulário personalizado] opções de objeto](assets/create-custom-form.png)

Ao editar um formulário personalizado, você pode ver todos os tipos de objeto selecionados. Você pode adicionar ou excluir tipos de objetos desta lista.

![Janela de formulário personalizado mostrando os tipos de objeto selecionados durante a edição do formulário](assets/edit-custom-form.png)

Talvez você queira criar um formulário personalizado do tipo projeto e problema. Quando anexado a um problema, você pode preencher qualquer um dos campos relacionados ao problema. Posteriormente, se você decidir converter o problema em um projeto, o formulário personalizado será carregado automaticamente no projeto e os dados inseridos nos campos do formulário personalizado de problema estarão disponíveis para visualização ou edição no formulário personalizado do projeto.

## Opções de campo personalizado

**[!UICONTROL Rótulo] e [!UICONTROL Nome] campos**

A variável [!UICONTROL Rótulo] e [!UICONTROL Nome] os campos em um campo personalizado atendem a diferentes objetivos. [!UICONTROL Rótulo] é o nome do campo que os usuários verão no [!DNL Workfront]. [!UICONTROL Nome] O é o que pode ser usado com integrações, como API.

![Janela de formulário personalizado sendo exibida [!UICONTROL Rótulo] e [!UICONTROL Nome] campos](assets/custom-forms-field-label-and-name.png)

Isso oferece a flexibilidade de alterar o rótulo voltado para o usuário para corresponder às alterações em sua organização, sem afetar as integrações ou outras conexões que dependem de um nome de campo específico.

**[!UICONTROL Campo de texto com formatação]**

A variável [!UICONTROL Campo de texto com formatação ]O contém ferramentas básicas de marcação de texto que permitem aos usuários adicionar negrito, itálico ou sublinhado no texto enquanto preenchem o campo em um formulário personalizado.

![Janela de formulário personalizado sendo exibida [!UICONTROL Campo de texto com formatação] opção](assets/custom-forms-text-field-with-formatting.png)

O campo também tem um limite de 15.000 caracteres, permitindo bastante espaço para fornecer informações vitais e usar a formatação para facilitar a leitura para os outros.

**[!UICONTROL Typeahead] campo**

A variável [!UICONTROL Typeahead] permite que o sistema preencha automaticamente uma lista de opções com base no objeto selecionado para o campo.

![Janela de formulário personalizado sendo exibida [!UICONTROL Typeahead] opção de campo](assets/custom-forms-typeahead-1.png)

Por exemplo, se você criar um [!UICONTROL Typeahead] chamado &quot;Nome de aprovação do gerente de marketing&quot; e selecione [!UICONTROL Usuário] como o tipo de objeto referenciado, uma lista de nomes de usuários é exibida quando um usuário preenche esse campo em um formulário personalizado. A variável [!UICONTROL Typeahead] O campo destina-se a conectar seus dados personalizados às informações capturadas no sistema e eliminar a necessidade de manter manualmente muitas opções nos campos suspensos.

![Janela de formulário personalizado sendo exibida [!UICONTROL Typeahead] menu suspenso](assets/custom-forms-typeahead-2.png)
