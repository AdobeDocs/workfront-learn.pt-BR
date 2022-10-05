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
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# Crie expressões ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

Neste vídeo, você aprenderá:

* O que as expressões ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR calculam
* Como criar uma expressão de dados ADDWEEKDAYS em um campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## Exemplos adicionais

Abaixo estão alguns Adobe de expressões ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR adicionais [!DNL Workfront] Os clientes do criaram.

**Deveria ter sido feito por**

O cliente queria saber quando a tarefa deveria ter sido concluída com base na Data de início real e na Duração planejada. A Data de Conclusão Projetada não funcionará nesse caso porque pode ser movida se a tarefa estiver atrasada e a Data de Conclusão Planejada não ajudará se houver atrasos em tarefas anteriores.

A expressão criada foi ADDDAYS(Data de Início Real,(Duração/480))

O tempo no campo Duration é armazenado em minutos. Portanto, nesta expressão, o campo Duration não pode ficar sozinho se o tempo for refletido em dias. Para isso, a Duração deve ser dividida por 480 minutos (480 minutos = 8 horas = 1 dia)

É por isso que o segundo slot de valor contém (Duration/480).


**Data de conclusão da fatura**

Esse exemplo inclui outro campo calculado, já criado e salvo no sistema, na expressão .

O cliente estava capturando a data em que a fatura foi enviada por meio de um campo de data personalizado, intitulado &quot;Data de envio da fatura&quot;, no formulário personalizado. Depois de enviado, eles têm 30 dias para concluir e arquivar a fatura. Para produzir automaticamente essa data de conclusão e arquivamento, eles criaram um campo calculado usando ADDDAYS e o campo Data de Envio da NFF. A expressão tinha esta aparência:

ADDDAYS(Data de Envio da NFF, 30)
