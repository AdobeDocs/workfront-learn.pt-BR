---
title: Entender o modo de texto básico para filtros
description: Saiba qual é o modo de texto, qual é o caso de camel e algum modo de texto "plug and play" básico que você pode usar nos filtros de relatório em [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 83c7379a5398c78cea31a4571b34fd5b64bce027
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Entender o modo de texto básico para filtros

Neste vídeo, você aprenderá:

* O modo de texto é
* Qual é o caso do camelo?
* Algum modo de texto &quot;plug and play&quot; básico que você pode usar nos filtros de relatório

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

O modo de texto a seguir excluirá tarefas em que um usuário marcou &quot;Concluído com a minha parte&quot;. Tudo o que você precisa fazer é criar um filtro de tarefa, adicionar as regras de filtro desejadas, alternar para o modo de texto e colar o código abaixo após qualquer modo de texto que você ver no filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Atividade: Perguntas sobre o modo de texto

1. Como você escreveria o caso de camelo para o campo intitulado &quot;Inserido por ID&quot;?
1. Em um relatório de Ocorrência , crie um filtro para mostrar os problemas que foram marcados como fechados, mas que estão pendentes de aprovação.

## Respostas

1. O caso de camelo para o campo &quot;Inserido por ID&quot; deve ser escrito da seguinte maneira — enteredByID
1. O modo de texto deve ter esta aparência no filtro de relatório de problemas:

   ![Uma imagem da tela para criar um novo filtro no modo de texto](assets/btm-answer.png)
