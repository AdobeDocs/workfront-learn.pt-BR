---
title: Criar solicitações personalizadas
description: Aprenda o que é uma solicitação personalizada, como criá-la usando o modo de texto e alguns exemplos que você pode usar em relatórios do Workfront.
activity: use
feature: Text Mode Reporting
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 98%

---

# Criar solicitações personalizadas

Neste vídeo, você aprenderá:

* O que é uma solicitação personalizada
* Como criar uma solicitação personalizada usando o modo de texto
* Alguns exemplos que você pode usar nos relatórios

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## Criar atividades de prompts personalizadas

[Clique aqui](/help/assets/create-custom-prompts-activities.pdf) para baixar um PDF desta página.

## Atividade: criar solicitações personalizadas

1. Crie uma solicitação personalizada que mostre os seguintes status do projeto no menu suspenso de solicitações:
   * Em Planejamento
   * Em Andamento
   * Concluídos
   * Parado
1. Modifique a solicitação para mostrar os projetos atuais que expiram neste mês.

## Respostas

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
