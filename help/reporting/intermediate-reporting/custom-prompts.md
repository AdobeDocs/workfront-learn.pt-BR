---
title: Criar prompts personalizados
description: Saiba o que é um prompt personalizado, como criar um prompt personalizado usando o modo de texto e alguns exemplos que você pode usar nos relatórios no Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 2%

---

# Criar prompts personalizados

Neste vídeo, você aprenderá:

* O que é um prompt personalizado
* Como criar um prompt personalizado usando o modo de texto
* Alguns exemplos que podem ser usados em seus relatórios

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12)

## Atividade: Criar prompts personalizados

1. Crie um prompt personalizado que mostre os seguintes status do projeto no menu suspenso do prompt:
   * Em Planejamento
   * Em Andamento
   * Concluídos
   * Parado
1. Modifique o prompt para mostrar os projetos atuais que devem ocorrer este mês.

## Respostas

1. Os prompts personalizados devem ser semelhantes a este e ter o seguinte modo de texto:

   ![Uma imagem da tela para criar um novo filtro no modo de texto](assets/cp-01.png)

   Depois de salvar o prompt personalizado, o menu suspenso do prompt deverá ter a seguinte aparência:

1. O modo de texto no prompt personalizado deve ser semelhante a:

![Uma imagem da tela para criar um novo filtro no modo de texto](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

E o rótulo suspenso para prompts ativos deve ser atualizado para refletir a alteração no código desta forma:

![Uma imagem da tela para criar um novo filtro no modo de texto](assets/cp-02a.png)
