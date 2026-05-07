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
TQID: https://experienceleague.adobe.com/22KjuMtDdhm9A6JohWlThfOHwKcegLwT3nuFO--70N4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 275
ht-degree: 97%

---

# Criar expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

Neste vídeo, você aprenderá:

* O que as expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS e ADDYEAR calculam
* Como criar uma expressão de dados ADDWEEKDAYS em um campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on&enablevpops=1)

## Exemplos adicionais

Veja abaixo algumas expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS e ADDYEAR adicionais que clientes do Adobe Workfront criaram.

**Deveria ter sido concluída até**

O cliente deseja saber quando a tarefa deveria ter sido concluída com base na data inicial real e na duração planejada. A data de conclusão projetada não funcionará neste caso porque pode ser alterada se a tarefa estiver atrasada, e a data de conclusão planejada não ajuda se houver atrasos nas tarefas anteriores.

A expressão criada foi ADDDAYS({actualStartDate},{durationMinutes}/480)

O tempo no campo Duração é armazenado em minutos. Portanto, nesta expressão, o campo Duração não pode ser independente se o tempo for refletido em dias. Para que isso aconteça, a Duração deve ser dividida por 480 minutos (480 minutos = 8 horas = 1 dia)

É por isso que o segundo slot de valor contém (Duration/480).


**Data de conclusão da fatura**

Este exemplo inclui não apenas o uso da expressão ADDDAYS, mas também um campo personalizado previamente criado e salvo no formulário personalizado.

O cliente está capturando a data em que uma fatura é enviada por meio de um campo de data personalizado intitulado “Data de envio da fatura”.

Depois de enviada, a fatura deve ser preenchida e arquivada no prazo de 30 dias. Para gerar automaticamente essa data de conclusão e arquivamento, um campo calculado ADDDAYS é usado junto com o campo personalizado “Data de envio da fatura”. A expressão deve ter esta aparência:

ADDDAYS({DE:Invoice Submission Date},30)
