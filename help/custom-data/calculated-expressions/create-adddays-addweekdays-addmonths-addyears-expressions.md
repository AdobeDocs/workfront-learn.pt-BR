---
title: Criar expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS
description: Saiba como usar e criar as expressões ADD em um campo calculado no Adobe [!DNL Workfront].
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
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Criar expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

Neste vídeo, você aprenderá:

* O que as expressões ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR calculam
* Como criar uma expressão de dados ADDWEEKDAYS em um campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## Exemplos adicionais

Abaixo estão algumas expressões adicionais de ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR que os clientes da Adobe Workfront criaram.

**Deve ter sido concluída por**

O cliente queria saber quando a tarefa deveria ter sido concluída com base na Data de início efetiva e na Duração planejada. A Data de conclusão projetada não funcionará nesse caso, pois poderá ser movida se a tarefa estiver atrasada e a Data de conclusão planejada não ajudará se houver atrasos nas tarefas anteriores.

A expressão criada foi ADDDAYS({atualStartDate},{durationMinutes}/480)

O tempo no campo Duration é armazenado em minutos. Portanto, nessa expressão, o campo Duration não pode ficar sozinho se o tempo for refletido em dias. Para que isso aconteça, a Duração deve ser dividida por 480 minutos (480 minutos = 8 horas = 1 dia)

É por isso que o segundo slot de valor contém (Duration/480).


**Data de conclusão da fatura**

Este exemplo inclui não apenas a expressão ADDDAYS, mas um campo personalizado criado anteriormente e salvo no formulário personalizado.

O cliente está capturando a data em que uma fatura é enviada por meio de um campo de data personalizado intitulado &quot;Data de envio da fatura&quot;.

Após o envio, a fatura deve ser preenchida e arquivada no prazo de 30 dias. Para produzir automaticamente essa data de conclusão e arquivamento, um campo calculado ADDDAYS é usado junto com o campo personalizado &quot;Data de envio da fatura&quot;. A expressão tem esta aparência:

ADDDAYS({DE:Data de envio da fatura},30)
