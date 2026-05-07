---
title: Criar prompts personalizados usando o modo de texto
description: Aprenda o que é uma solicitação personalizada, como criá-la usando o modo de texto e alguns exemplos que você pode usar em relatórios do Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-08-05T00:00:00.000Z'
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: cec4c78b-dd2b-46ec-b824-6ca30f0eb7b2
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:58:55.263Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 207
ht-degree: 94%

---

# Criar prompts personalizados usando o modo de texto

Neste vídeo, você aprenderá:

* O que é uma solicitação personalizada
* Como criar uma solicitação personalizada usando o modo de texto
* Alguns exemplos que você pode usar nos relatórios

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on&enablevpops=0)

## Atividades “Criar prompts personalizados”


### Atividade: criar solicitações personalizadas

1. Crie uma solicitação personalizada que mostre os seguintes status do projeto no menu suspenso de solicitações:
   * Em Planejamento
   * Em Andamento
   * Concluídos
   * Parado
1. Modifique a solicitação para mostrar os projetos atuais que expiram neste mês.

### Respostas

1. Suas solicitações personalizadas devem ter uma aparência semelhante a esta e usar o seguinte modo de texto:

   ![Uma imagem da tela de criação de um novo filtro no modo de texto](assets/cp-01.png)

   Após salvar a solicitação personalizada, o menu suspenso da solicitação deverá ter esta aparência:

1. O modo de texto da solicitação personalizada deve ter esta aparência:

![Uma imagem da tela de criação de um novo filtro no modo de texto](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

E o rótulo suspenso para solicitações ativas deve ser atualizado para refletir a alteração no código, desta forma:

![Uma imagem da tela de criação de um novo filtro no modo de texto](assets/cp-02a.png)
