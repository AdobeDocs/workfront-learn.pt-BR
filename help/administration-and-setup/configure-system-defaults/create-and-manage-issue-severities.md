---
title: Criar e gerenciar gravidade do problema
description: Saiba como configurar e gerenciar gravidade de problemas.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: 5d385de5cdcee0d433304c09507ba6bb5b0a10e6
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 3%

---

# Criar e gerenciar as severidades de problemas

## Introdução às severidades de emissão

Uma severidade pode ser usada para indicar a gravidade de um problema ou como ele pode afetar o trabalho que está sendo feito.

![[!UICONTROL Gravidade] no menu [!UICONTROL Detalhes do problema] janela](assets/admin-fund-severity-issue-details.png)

O [!UICONTROL Gravidade] pode ser acessado na variável [!UICONTROL Detalhes do problema]. Também pode ser incluído nas exibições de coluna em listas e em relatórios personalizados.

[!DNL Workfront] tem cinco severidades padrão:

* [!UICONTROL Cosmética]
* [!UICONTROL Causa Confusão]
* [!UICONTROL Problema com Solução]
* [!UICONTROL Problema Sem Solução]
* [!UICONTROL Erro Fatal]

Os administradores do sistema podem renomear essas severidades padrão ou criar novas, se necessário.

As severidades estão disponíveis apenas para problemas em [!DNL Workfront].

## Criar e gerenciar as severidades de problemas

Como administrador do sistema, você pode criar novas severidades, se necessário, para concluir o fluxo de trabalho do problema.

![[!UICONTROL Severidades] em [!UICONTROL Configuração]](assets/admin-fund-severity-section.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda o **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Severidades]**.
1. Clique em **[!UICONTROL Adicionar uma nova gravidade]**.
1. Atribua à severidade um nome que corresponda ao uso desejado.
1. O **[!UICONTROL Importância]** corresponde à gravidade do problema. O número mais alto corresponde à severidade mais alta. O [!UICONTROL Importância] deve ser único.
1. Selecione uma cor para a sua prioridade. Usado em relatórios de gráfico e outros locais em [!DNL Workfront].
1. Designar uma das opções de gravidade como **[!UICONTROL Gravidade padrão]**. Isso é aplicado automaticamente a todos os novos problemas no Workfront.
1. Inclua uma descrição da gravidade, como como ela será usada.
1. Clique fora dos campos para salvar.

![[!UICONTROL Severidades] lista](assets/admin-fund-severity-new.png)

### Modificação de severidades

Se uma severidade não se tornar mais relevante para os fluxos de trabalho de emissão, ela poderá ser renomeada, oculta ou excluída.

Se uma severidade não for mais necessária, [!DNL Workfront] A recomenda ocultar a severidade (clique no botão [!UICONTROL Ocultar] caixa ao lado dele na área de configuração). Isso remove a opção de gravidade do menu suspenso do problema, mas mantém a severidade nos dados históricos para que ainda esteja disponível para fins de relatório.

![[!UICONTROL Ocultar] coluna realçada em [!UICONTROL Severidades] em [!UICONTROL Configuração]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] recomenda que **não** exclua uma severidade que tenha sido usada em problemas anteriores. Quando você exclui uma severidade, ela solicita que você substitua outra severidade. Isso pode alterar os dados históricos e afetar os relatórios.

![Excluir janela de severidade](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
