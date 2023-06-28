---
title: Configurar preferências de problema padrão global
description: Saiba como definir preferências de problemas para problemas convertidos, datas reais e acesso a problemas.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Configurar preferências globais de problema padrão

Várias configurações em todo o sistema estabelecem padrões para o comportamento dos problemas em determinadas circunstâncias no [!DNL Workfront].

A prática recomendada é deixar os padrões globais como estão e permitir que os gerentes de projeto façam os ajustes necessários no nível do projeto ou nos modelos do projeto.

As preferências globais do problema podem ser ajustadas, mas recomenda-se que você e seus [!DNL Workfront] o consultor do discute quais configurações são necessárias para as necessidades de workflows, processos e relatórios de sua organização. Seu consultor também pode ajudá-lo a entender o que acontecerá se determinadas configurações forem alteradas.

As preferências de problemas permitem que os administradores do sistema controlem as opções quando os problemas são convertidos em tarefas ou projetos, como as datas reais são calculadas e quem recebe acesso ao projeto quando os problemas são atribuídos. Vamos observar onde estão essas configurações [!DNL Workfront].

## Preferências de problema convertido

Essas configurações controlam o que acontece com um problema quando ele é convertido em uma tarefa ou um projeto no [!DNL Workfront].

![[!UICONTROL Tarefas e problemas] janela de preferências com [!UICONTROL Problemas] seção realçada](assets/admin-fund-issue-prefs-converting.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda a **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Tarefas e problemas]**.
1. Role para a **[!UICONTROL Problemas]** seção.
1. Clique nas opções desejadas.
1. Salve quando terminar.

Vamos analisar as opções nesta seção para que você possa escolher as opções apropriadas para sua organização.

* **[!UICONTROL Atualizar automaticamente o status de Problema resolvível quando o status do Objeto de resolução é alterado]**

  Essa configuração permite correlacionar a resolução da ocorrência original com a resolução do novo objeto (tarefa ou projeto).

  Com essa configuração ativada (marcada), você pode criar status de problemas personalizados que tenham a mesma chave de status que um status de tarefa ou projeto. Quando a tarefa ou o projeto (o objeto que pode ser resolvido) é definido para o status personalizado, a alteração também é exibida no status do problema.

  Quando desativado, o status do objeto de resolução é definido automaticamente para o status padrão, em vez de personalizados.

  Para que essa configuração tenha efeito, a variável &quot;[!UICONTROL Conservar o problema original e vincular a sua resolução à tarefa]&quot; deve ser selecionada.

* **[!UICONTROL Manter o problema original e vincular a resolução à tarefa/projeto]**

  Quando o problema é convertido, isso informa [!DNL Workfront] para manter os problemas originais. O status do problema muda conforme o status da tarefa ou do projeto é alterado. Quando a tarefa ou o projeto estiver marcado como concluído, o problema será marcado como resolvido.

  Se essa opção não estiver marcada, o problema original será excluído e somente a tarefa ou o projeto convertido permanecerá.

  Essa configuração afeta relatórios sobre problemas originalmente registrados em um projeto ou que vêm por uma [!DNL Workfront] fila de solicitações.

* **[!UICONTROL Permitir que contato primário tenha acesso à tarefa/projeto]**

  Isso dá à pessoa que criou o problema original acesso à tarefa ou ao projeto criado durante a conversão. Eles podem revisar o trabalho, fazer atualizações e se manter informados sobre o progresso.

* **[!UICONTROL Permitir que estas configurações sejam alteradas durante a conversão]**

  Quando selecionada, essa opção significa as configurações padrão para &quot;[!UICONTROL Manter problema original]&quot; e &quot;[!UICONTROL Permitir contato primário]&quot; pode ser alterado pelo usuário que converte o problema. Se quiser que os padrões permaneçam inalterados, desmarque essa opção.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Preferências de datas reais

Há vários tipos de datas usadas em [!DNL Workfront]. As datas reais são um &quot;carimbo de data e hora&quot; que [!DNL Workfront] é gerado quando ocorrem determinadas alterações de status.

A variável [!UICONTROL Data do Início Efetivo] O carimbo de data e hora é criado quando o status do problema muda de Novo para outro status. A variável [!UICONTROL Data de término efetivo] carimbo de data e hora é quando o status do problema muda para um status que indica que está fechado.

É importante observar que essa preferência controla as configurações de data real para tarefas e problemas.

![[!UICONTROL Tarefas e problemas] janela de preferências com [!UICONTROL Datas Efetivas] seção realçada](assets/admin-fund-issue-prefs-actual-dates.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda a **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Tarefas e problemas]**.
1. Role para a **[!UICONTROL Datas Efetivas]** seção.
1. Selecione a opção desejada para o **[!UICONTROL Data do Início Efetivo]** — [!UICONTROL Agora] (a data e a hora atuais) ou [!UICONTROL A data de início planejada] (o [!UICONTROL Data do Início Efetivo] corresponde à data de início definida nos detalhes da ocorrência).
1. Agora selecione a opção para a variável **[!UICONTROL Data de término efetivo]** — [!UICONTROL Agora] (a data e a hora atuais) ou [!UICONTROL A Data de Término Planejada] (o [!UICONTROL Data do Início Efetivo] corresponde à data definida nos detalhes da ocorrência).
1. Salve quando terminar.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Acesso ao problema

A variável [!UICONTROL Access] as configurações para problemas controlam o acesso que um usuário recebe quando recebe um problema no Workfront. Essas configurações controlam o acesso ao próprio problema, além do acesso ao projeto ao qual o problema está associado.

Antes de alterar essas configurações, discuta com sua equipe qualquer necessidade de fluxo de trabalho ou processo [!DNL Workfront] e sua equipe interna de governança.

![[!UICONTROL Tarefas e problemas] janela de preferências com [!UICONTROL Quando alguém é designado a um PROBLEMA] seção realçada](assets/admin-fund-issue-prefs-access-1.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda a **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecionar **[!UICONTROL Tarefas e problemas]**.
1. Role para a **[!UICONTROL Access]** e localize o &quot;[!UICONTROL Quando alguém é designado a um PROBLEMA]&quot;.
1. Definir o acesso de compartilhamento para o problema em si — [!UICONTROL Exibir], [!UICONTROL Contribute]ou [!UICONTROL Gerenciar]. [!DNL Workfront] A recomenda deixar as opções avançadas como estão.
1. Marque a caixa se o destinatário da ocorrência também tiver acesso ao projeto
1. Em seguida, selecione o acesso de compartilhamento para o projeto — [!UICONTROL Exibir], [!UICONTROL Contribute]ou [!UICONTROL Gerenciar]. À medida que você define o [!UICONTROL Opções avançadas], lembre-se dos fluxos de trabalho e das necessidades de acesso de sua organização.
1. Salve quando terminar.

![[!UICONTROL Access] janela mostrando [!UICONTROL Contribute] opções](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
