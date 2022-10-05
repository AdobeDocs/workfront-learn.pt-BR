---
title: Configurar preferências de ocorrência padrão global
description: Saiba como definir preferências de edição para problemas convertidos, datas reais e acesso a problemas.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 3ded3fe9d8b97b1c11cb382f8088930842399c98
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Configurar preferências de problema padrão global

Várias configurações em todo o sistema estabelecem padrões para o comportamento dos problemas em determinadas circunstâncias em [!DNL Workfront].

A prática recomendada é deixar os padrões globais como estão e permitir que os gerentes de projeto façam os ajustes necessários no nível do projeto ou nos modelos do projeto.

As preferências globais de edição podem ser ajustadas, mas é recomendável que você e sua [!DNL Workfront] consultor discute quais configurações são necessárias para os fluxos de trabalho, processos e necessidades de relatórios de sua organização. Seu consultor também pode ajudá-lo a entender o que acontecerá se determinadas configurações forem alteradas.

As preferências de edição permitem que os administradores do sistema controlem as opções quando os problemas são convertidos em tarefas ou projetos, como as datas reais são calculadas e quem obtém acesso ao projeto quando os problemas são atribuídos. Vamos analisar onde essas configurações estão [!DNL Workfront].

## Preferências de problema convertidas

Essas configurações controlam o que acontece com um problema quando ele é convertido em uma tarefa ou projeto no [!DNL Workfront].

![[!UICONTROL Tarefas e problemas] janela preferências com [!UICONTROL Problemas] seção realçada](assets/admin-fund-issue-prefs-converting.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda o **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Tarefas e problemas]**.
1. Role para **[!UICONTROL Problemas]** seção.
1. Clique nas opções desejadas.
1. Salve quando terminar.

Vamos analisar as opções nesta seção para que você possa escolher as opções apropriadas para sua organização.

* **[!UICONTROL Atualizar automaticamente o status do Problema Resolvível quando o status do Objeto Resolvendo Alterações]**

   Essa configuração permite correlacionar a resolução do problema original à resolução do novo objeto (tarefa ou projeto).

   Com essa configuração ativada (marcada), é possível criar status de problema personalizado que tenham a mesma chave de status que uma tarefa ou status do projeto. Quando a tarefa ou o projeto (o objeto resolvível) é definido como status personalizado, a alteração também é exibida no status da ocorrência.

   Quando desativado, o status de resolução do objeto é definido automaticamente para o status padrão, em vez de personalizado.

   Para que essa configuração tenha qualquer efeito, o &quot;[!UICONTROL Mantenha o problema original e vincule sua resolução à tarefa]&quot; deve ser selecionada.

* **[!UICONTROL Manter o problema original e vincular a resolução à tarefa/projeto]**

   Quando o problema é convertido, isso informa [!DNL Workfront] para manter os problemas originais. O status do problema muda conforme o status da tarefa ou do projeto é alterado. Depois que a tarefa ou o projeto for marcado como concluído, o problema será marcado como resolvido.

   Se essa opção não estiver marcada, o problema original será excluído e somente a tarefa ou o projeto convertido permanecerá.

   Essa configuração afeta os relatórios sobre problemas originalmente conectados a um projeto ou que vêm de um [!DNL Workfront] fila de solicitações.

* **[!UICONTROL Permitir que o Contato Principal tenha acesso à tarefa/projeto]**

   Isso dá à pessoa que criou o problema original acesso à tarefa ou projeto criado durante a conversão. Eles podem revisar o trabalho, fazer atualizações e permanecer informados sobre o progresso.

* **[!UICONTROL Permitir que estas configurações sejam alteradas durante a conversão]**

   Quando selecionada, essa opção significa que as configurações padrão de &quot;[!UICONTROL Manter problema original]&quot; e &quot;[!UICONTROL Permitir Contato Principal]&quot; pode ser alterado pelo usuário que está convertendo o problema. Se desejar que os padrões permaneçam inalterados, desmarque essa opção.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Preferências de datas reais

Existem vários tipos de datas usadas em todo o [!DNL Workfront]. As datas reais são um &quot;carimbo de data e hora&quot; que [!DNL Workfront] gera quando determinadas alterações de status ocorrem.

O [!UICONTROL Data de início real] o carimbo de data e hora é criado quando o status do problema muda de New para outro status. O [!UICONTROL Data de conclusão real] timestamp é quando o status do problema muda para um status que indica que foi fechado.

É importante observar que essa preferência controla as configurações de data reais tanto para tarefas quanto para problemas.

![[!UICONTROL Tarefas e problemas] janela preferências com [!UICONTROL Datas reais] seção realçada](assets/admin-fund-issue-prefs-actual-dates.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda o **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Tarefas e problemas]**.
1. Role para **[!UICONTROL Datas reais]** seção.
1. Selecione a opção desejada para a **[!UICONTROL Data de início real]** — [!UICONTROL Agora] (a data e hora atuais) ou [!UICONTROL A Data Inicial Planejada] (a) [!UICONTROL Data de início real] corresponde à data de início definida nos detalhes da ocorrência).
1. Em seguida, selecione a opção para o **[!UICONTROL Data de conclusão real]** — [!UICONTROL Agora] (a data e hora atuais) ou [!UICONTROL A Data de Conclusão Planejada] (a) [!UICONTROL Data de início real] corresponde à data definida nos detalhes da emissão).
1. Salve quando terminar.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Acesso à emissão

O [!UICONTROL Acesso] as configurações para problemas controlam o acesso que um usuário recebe quando recebe um problema no Workfront. Essas configurações controlam o acesso ao próprio problema, além do acesso ao projeto ao qual o problema está associado.

Antes de alterar essas configurações, discuta qualquer necessidade de fluxo de trabalho ou processo com seu [!DNL Workfront] consultores e sua equipe interna de controle.

![[!UICONTROL Tarefas e problemas] janela preferências com [!UICONTROL Quando alguém é atribuído a um PROBLEMA] seção realçada](assets/admin-fund-issue-prefs-access-1.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda o **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Tarefas e problemas]**.
1. Role para **[!UICONTROL Acesso]** e localize o &quot;[!UICONTROL Quando alguém é atribuído a um PROBLEMA]&quot;.
1. Definir o acesso de compartilhamento para o próprio problema — [!UICONTROL Exibir], [!UICONTROL Contribute]ou [!UICONTROL Gerenciar]. [!DNL Workfront] A recomenda deixar as opções avançadas como estão.
1. Marque a caixa se o responsável pelo problema também tiver acesso ao projeto
1. Em seguida, selecione o acesso de compartilhamento do projeto — [!UICONTROL Exibir], [!UICONTROL Contribute]ou [!UICONTROL Gerenciar]. Conforme você define a variável [!UICONTROL Opções avançadas], lembre-se dos fluxos de trabalho e das necessidades de acesso de sua organização.
1. Salve quando terminar.

![[!UICONTROL Acesso] janela mostrando [!UICONTROL Contribute] opções](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
