---
title: Crie expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS
description: Saiba como usar e criar expressões ADD em um campo calculado no Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Crie expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

Neste vídeo, você aprenderá:

* O que as expressões ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR calculam
* Como criar uma expressão de dados ADDWEEKDAYS em um campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## Exemplos adicionais

Abaixo estão alguns ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR adicionais que os clientes da Adobe Workfront criaram.

**Deveria ter sido feito por**

O cliente queria saber quando a tarefa deveria ter sido concluída com base na Data de início real e na Duração planejada. A Data de Conclusão Projetada não funcionará nesse caso porque pode ser movida se a tarefa estiver atrasada e a Data de Conclusão Planejada não ajudará se houver atrasos em tarefas anteriores.

A expressão criada foi ADDDAYS({atualStartDate},{durationMinutes}/480)

O tempo no campo Duration é armazenado em minutos. Portanto, nesta expressão, o campo Duration não pode ficar sozinho se o tempo for refletido em dias. Para isso, a Duração deve ser dividida por 480 minutos (480 minutos = 8 horas = 1 dia)

É por isso que o segundo slot de valor contém (Duration/480).


**Data de conclusão da fatura**

Esse exemplo inclui não apenas a expressão ADDDAYS, mas um campo personalizado criado e salvo no formulário personalizado.

O cliente está capturando a data em que uma NFF é enviada por meio de um campo de data personalizado intitulado &quot;Data de Envio da NFF&quot;.

Depois de enviada, a fatura deve ser preenchida e arquivada no prazo de 30 dias. Para produzir automaticamente essa data de conclusão e arquivamento, um campo calculado ADDDAYS é usado junto com o campo personalizado &quot;Data de Envio da NFF&quot;. A expressão tem esta aparência:

ADDDAYS({DE:Invoice Submission Date},30)
