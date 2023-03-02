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
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 2%

---

# Criar prompts personalizados

Neste vídeo, você aprenderá:

* O que é um prompt personalizado
* Como criar um prompt personalizado usando o modo de texto
* Alguns exemplos que você pode usar nos relatórios

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12)

## Atividade: criar prompts personalizados

1. Crie um prompt personalizado que mostre os seguintes status do projeto no menu suspenso de prompts:
   * Em Planejamento
   * Em Andamento
   * Concluídos
   * Parado
1. Modifique o prompt para mostrar os projetos atuais que estão vencidos este mês.

## Respostas

1. Seus prompts personalizados devem ser semelhantes a este e ter o seguinte modo de texto:

   ![Uma imagem da tela para criar um novo filtro no modo de texto](assets/cp-01.png)

   Depois de salvar o prompt personalizado, o menu suspenso do prompt deverá ter esta aparência:

1. O modo de texto no seu prompt personalizado deve ser semelhante a:

![Uma imagem da tela para criar um novo filtro no modo de texto](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

E o rótulo suspenso para prompts ativos deve ser atualizado para refletir a alteração no código, desta forma:

![Uma imagem da tela para criar um novo filtro no modo de texto](assets/cp-02a.png)
