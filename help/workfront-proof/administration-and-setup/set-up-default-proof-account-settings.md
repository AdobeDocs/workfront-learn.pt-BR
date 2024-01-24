---
title: Definir configurações padrão da conta de prova
description: Saiba como definir configurações de conta padrão que se aplicam globalmente a todos os usuários de provas e provas.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Definir configurações padrão da conta de prova

Estabeleça configurações padrão da conta que se aplicam globalmente a todos os usuários de provas e provas — país, idioma e fuso horário. Se você tiver usuários em vários fusos horários ou países, poderá ajustar essas configurações no perfil do usuário de cada indivíduo, se necessário.

![Janela de configurações de conta para revisão de texto](assets/proof-system-setups-default-account-settings.png)

1. Selecionar **[!UICONTROL Prova]** de [!DNL Workfront's] [!UICONTROL Menu principal].
1. Selecionar **[!UICONTROL Configurações da conta]** na barra de navegação superior.
1. Selecione o **[!UICONTROL Detalhes]** guia.
1. Ir para [!UICONTROL País] e selecione **[!UICONTROL Editar]**. Escolha o país em que a maioria dos usuários da prova está como padrão.
1. Selecionar **[!UICONTROL Salvar]** para essa configuração.
1. Vá para a [!UICONTROL Idioma padrão] e selecione **[!UICONTROL Editar]**. Escolha o idioma que a maioria dos usuários de prova usará como padrão.
1. Selecionar **[!UICONTROL Salvar]** para essa configuração.
1. Vá para a [!UICONTROL Padrão de fuso horário] e selecione **[!UICONTROL Editar]**. Escolha o fuso horário em que a maioria dos usuários da prova estará como padrão. Esse será o fuso horário reconhecido por workflows de prova configurados manualmente. Ela também se aplica a modelos de fluxo de trabalho de prova, mas cada modelo pode ter um fuso horário definido.
1. Selecionar **[!UICONTROL Salvar]** para essa configuração.

## Práticas recomendadas


| Prática recomendada | Aqui está o porquê |
|---|---|
| Ajuste as configurações de back-end da prova para que os usuários vejam os prazos em um formato de relógio de 12 horas. | Selecione a opção F j, Y, gi:a nas configurações de prova para usuários que desejam ver prazos/horas de prova em um formato AM/PM. Para áreas que usam um relógio de 12 horas, isso ajuda na clareza do prazo. <br> <br>Observação: essa configuração é encontrada acessando o Menu principal do Workfront > Revisão de texto > Configurações da conta > Usuários > e editando o campo Formato da data para cada usuário. |
| Estabeleça um prazo de prova padrão como parte das configurações do sistema. | Quando um prazo de prova padrão é definido (a data de upload + x número de dias úteis), se o criador da prova esquecer de adicionar um prazo, a Workfront aplicará automaticamente esse prazo a todas as provas carregadas. <br> <br>Observação: essa configuração é encontrada no menu principal do Workfront > Revisão > Configurações da conta > Configurações > Padrões de prova > Campo prazo (+ dias úteis). |
| Oculte a opção Não relevante para decisão de prova. | Essa opção de decisão geralmente causa confusão entre aprovadores, já que as organizações geralmente não definem quando a opção Não relevante deve ser usada. A opção Não relevante geralmente indica que a prova não é relevante para o recipient da prova e que ele não precisa tomar uma decisão aprovada ou rejeitada. Ao selecionar Não relevante, permite que o fluxo de trabalho de prova continue.<br> <br>A opção Not Relevant não é necessária na maioria dos workflows de prova.<br> <br>Observação: essa configuração é encontrada indo até o menu principal do Workfront > Revisão > Configurações da conta > Decisões. |
| Não reordene as opções de decisão da prova nas configurações de prova. | Cada configuração de decisão de prova contém um valor/peso específico que, se reordenado, pode causar confusão nas configurações da prova. A ordem de decisão e o valor/peso são usados como acionadores de ativação do estágio de prova e nos relatórios.<br> <br>Observação: essa configuração é encontrada indo até o menu principal do Workfront > Revisão > Configurações da conta > Decisões. |
| Defina os padrões do usuário para funções de prova e alertas de email. | Essas configurações são preenchidas automaticamente ao atribuir um fluxo de trabalho de prova, acelerar o processo e contribuir para a consistência entre fluxos de trabalho de prova.<br> <br>Observação: as configurações padrão do usuário são encontradas ao acessar o Menu principal do Workfront > Revisão de texto > Configurações da conta > Usuários > e selecionar o usuário para o qual definir padrões. |
