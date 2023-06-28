---
title: Criar e gerenciar severidades de problemas
description: Saiba como configurar e gerenciar severidades de problemas.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 3%

---

# Criar e gerenciar severidades de problemas

## Introdução às severidades do problema

Uma severidade pode ser usada para indicar a gravidade de um problema ou como ele pode afetar o trabalho que está sendo feito.

![[!UICONTROL Severidade] no menu [!UICONTROL Detalhes do problema] janela](assets/admin-fund-severity-issue-details.png)

A variável [!UICONTROL Severidade] o campo pode ser acessado no campo [!UICONTROL Detalhes do problema]. Ele também pode ser incluído em exibições de coluna em listas e em relatórios personalizados.

[!DNL Workfront] tem cinco severidades padrão:

* [!UICONTROL Cosmética]
* [!UICONTROL Causa Confusão]
* [!UICONTROL Problema com Solução]
* [!UICONTROL Problema Sem Solução]
* [!UICONTROL Erro Fatal]

Os administradores do sistema podem renomear essas severidades padrão ou criar novas, se necessário.

As severidades estão disponíveis somente para problemas no [!DNL Workfront].

## Criar e gerenciar severidades de problemas

Como administrador do sistema, você pode criar novas severidades, se necessário, para concluir o workflow do problema.

![[!UICONTROL Severidades] página em [!UICONTROL Configuração]](assets/admin-fund-severity-section.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda a **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Severidades]**.
1. Clique em **[!UICONTROL Adicionar uma nova severidade]**.
1. Nomeie a severidade de acordo com o uso pretendido.
1. A variável **[!UICONTROL Importância]** O número de corresponde à gravidade do problema. O número mais alto corresponde à severidade mais alta. A variável [!UICONTROL Importância] O número deve ser exclusivo.
1. Selecione uma cor para sua prioridade. Isso é usado em relatórios de gráficos e outros locais no [!DNL Workfront].
1. Designar uma das opções de severidade como **[!UICONTROL Severidade Padrão]**. Isso é aplicado automaticamente a todas as novas questões no Workfront.
1. Inclua uma descrição da gravidade, como como ela será usada.
1. Clique fora dos campos para salvar.

![[!UICONTROL Severidades] lista](assets/admin-fund-severity-new.png)

### Modificação de severidades

Se uma severidade não se tornar mais relevante para os workflows de problemas, ela poderá ser renomeada, oculta ou excluída.

Se uma severidade não for mais necessária, [!DNL Workfront] A recomenda ocultar a severidade (clique no link [!UICONTROL Ocultar] (ao lado dele, na área configuração). Isso remove a opção de gravidade do menu suspenso sobre o problema, mas retém a gravidade dos dados históricos para que ainda esteja disponível para fins de relatório.

![[!UICONTROL Ocultar] coluna realçada em [!UICONTROL Severidades] página em [!UICONTROL Configuração]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] recomenda que você **não** excluir uma severidade que tenha sido usada em problemas anteriores. Quando você exclui uma severidade, ela solicita que você substitua outra severidade. Isso pode alterar os dados históricos e afetar os relatórios.

![Excluir janela de severidade](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
