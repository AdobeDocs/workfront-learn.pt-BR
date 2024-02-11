---
title: Definir configurações padrão da conta de prova
description: Saiba como definir configurações de conta padrão que se aplicam a todas as provas e usuários de prova.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 58%

---

# Definir configurações padrão da conta de prova

Estabeleça configurações de conta padrão que se apliquem a todas as provas e usuários de prova (como configurações de país, idioma e fuso horário). Se você tiver usuários em vários fusos horários ou países, poderá ajustar essas configurações no perfil do usuário de cada indivíduo, se necessário.

![Janela de configurações da conta de prova](assets/proof-system-setups-default-account-settings.png)

1. Selecione **[!UICONTROL Revisão]** no [!DNL Workfront's] [!UICONTROL Menu principal].
1. Selecione **[!UICONTROL Configurações da conta]** na barra de navegação superior.
1. Selecione a guia **[!UICONTROL Detalhes]**.
1. Acesse o campo [!UICONTROL País] e selecione **[!UICONTROL Editar]**. Escolha como padrão o país onde a maioria dos usuários de prova estão localizados.
1. **[!UICONTROL Salve]** essa configuração.
1. Acesse o campo [!UICONTROL Idioma padrão] e selecione **[!UICONTROL Editar]**. Escolha como padrão o idioma que a maioria dos usuários de prova usará.
1. **[!UICONTROL Salve]** essa configuração.
1. Acesse o campo [!UICONTROL Fuso horário padrão] e selecione **[!UICONTROL Editar]**. Escolha como padrão o fuso horário utilizado pela maioria dos usuários de prova. Este será o fuso horário reconhecido pelos fluxos de trabalho de prova que forem configurados manualmente. Isso também se aplicará a modelos de fluxo de trabalho de prova, porém, é possível definir um fuso horário diferente para cada modelo.
1. **[!UICONTROL Salve]** essa configuração.

## Práticas recomendadas


| Prática recomendada | Aqui está o porquê |
|---|---|
| Ajuste as configurações de back-end de revisão, para que os usuários vejam os prazos no formato de 12 horas. | Selecione a opção F j, Y, gi:a nas configurações de revisão para usuários que queiram ver os prazos/horários das revisões no formato AM/PM. Para áreas que usam um relógio de 12 horas, isso ajuda na clareza do prazo. <br> <br>Observação: essa configuração é encontrada acessando o Menu principal do Workfront > Revisão de texto > Configurações da conta > Usuários > e editando o campo Formato da data para cada usuário. |
| Estabeleça um prazo de revisão padrão como parte das configurações do sistema. | Quando um prazo de prova padrão é definido (a data de upload + x número de dias úteis), se o criador da prova esquecer de adicionar um prazo, a Workfront aplicará automaticamente esse prazo a todas as provas carregadas. <br> <br>Observação: essa configuração é encontrada no menu principal do Workfront > Revisão > Configurações da conta > Configurações > Padrões de prova > Campo prazo (+ dias úteis). |
| Oculte a opção de revisão de prova “Não relevante”. | Essa opção de decisão muitas vezes causa confusão entre os aprovadores, pois muitas vezes as organizações não definem quando a opção “Não relevante” deve ser usada. A opção “Não relevante” geralmente indica que a revisão não é relevante para o destinatário da revisão e que ele não precisa tomar nenhuma decisão de aprovação ou rejeição. Ao selecionar Não relevante, permite que o fluxo de trabalho de prova continue.<br> <br>A opção Not Relevant não é necessária na maioria dos workflows de prova.<br> <br>Observação: essa configuração é encontrada indo até o menu principal do Workfront > Revisão > Configurações da conta > Decisões. |
| Não reordene as opções de decisão de revisão nas configurações de revisão. | Cada configuração de decisão de revisão contém um valor/peso específico que, se reordenado, pode causar confusão nas suas configurações de revisão. A ordem de decisão e o valor/peso são usados como acionadores de ativação do estágio de prova e nos relatórios.<br> <br>Observação: essa configuração é encontrada indo até o menu principal do Workfront > Revisão > Configurações da conta > Decisões. |
| Defina os padrões do usuário para funções de revisão e alertas por email. | Essas configurações são preenchidas automaticamente ao atribuir um fluxo de trabalho de prova, acelerar o processo e contribuir para a consistência entre fluxos de trabalho de prova.<br> <br>Observação: as configurações padrão do usuário são encontradas ao acessar o Menu principal do Workfront > Revisão de texto > Configurações da conta > Usuários > e selecionar o usuário para o qual definir padrões. |
