---
title: Criar expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS
description: Aprenda a usar e criar as expressões ADD em um campo calculado no Adobe  [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 100%

---

# Criar expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

Neste vídeo, você aprenderá:

* O que as expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS e ADDYEAR calculam
* Como criar uma expressão de dados ADDWEEKDAYS em um campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on&enablevpops)

## Exemplos adicionais

Veja abaixo algumas expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS e ADDYEAR adicionais que clientes do Adobe Workfront criaram.

**Deveria ter sido concluída até**

O cliente deseja saber quando a tarefa deveria ter sido concluída com base na data de início efetiva e na duração planejada. A data de conclusão projetada não funcionará neste caso porque pode ser alterada se a tarefa estiver atrasada, e a data de conclusão planejada não ajuda se houver atrasos nas tarefas anteriores.

A expressão criada foi: ADDDAYS({actualStartDate},{durationMinutes}/480)

O tempo no campo Duração é armazenado em minutos. Portanto, nesta expressão, o campo Duração não pode ser independente se o tempo for refletido em dias. Para que isso aconteça, a Duração deve ser dividida por 480 minutos (480 minutos = 8 horas = 1 dia)

É por isso que o segundo slot de valor contém (Duration/480).


**Data de conclusão da fatura**

Este exemplo inclui não apenas o uso da expressão ADDDAYS, mas também um campo personalizado previamente criado e salvo no formulário personalizado.

O cliente está capturando a data em que uma fatura é enviada por meio de um campo de data personalizado intitulado “Data de envio da fatura”.

Depois de enviada, a fatura deve ser preenchida e arquivada no prazo de 30 dias. Para gerar automaticamente essa data de conclusão e arquivamento, um campo calculado ADDDAYS é usado junto com o campo personalizado “Data de envio da fatura”. A expressão deve ter esta aparência:

ADDDAYS({DE:Invoice Submission Date},30)
