---
title: Configurar preferências padrão globais de problema
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
workflow-type: ht
source-wordcount: '885'
ht-degree: 100%

---

# Configurar preferências padrão globais de problema

Várias configurações em todo o sistema estabelecem padrões para o comportamento dos problemas em determinadas circunstâncias no [!DNL Workfront].

A prática recomendada é deixar os padrões globais como estão e permitir que os gerentes de projeto façam os ajustes necessários no nível do projeto ou nos modelos do projeto.

As preferências globais de problemas podem ser ajustadas, mas é recomendado que você e o seu consultor do [!DNL Workfront] discutam quais configurações são necessárias para os fluxos de trabalho, processos e necessidades de relatórios da sua organização. Seu consultor também pode ajudá-lo a entender o que acontece se determinadas configurações forem alteradas.

As preferências de problemas permitem que os administradores do sistema controlem as opções quando os problemas são convertidos em tarefas ou projetos, como as datas reais são calculadas e quem obtém acesso ao projeto quando os problemas são atribuídos. Vamos ver onde essas configurações estão localizadas no [!DNL Workfront].

## Preferências de problemas convertidos

Essas configurações controlam o que acontece com um problema quando ele é convertido em uma tarefa ou um projeto no [!DNL Workfront].

A janela Preferências de ![[!UICONTROL tarefas e problemas] com a seção [!UICONTROL Problemas] destacada](assets/admin-fund-issue-prefs-converting.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda a seção **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecione **[!UICONTROL Tarefas e problemas]**.
1. Role até a seção **[!UICONTROL Problemas]**.
1. Clique nas opções desejadas.
1. Salve quando terminar.

Vamos analisar as opções nesta seção para que você possa escolher as opções adequadas para sua organização.

* **[!UICONTROL Atualizar automaticamente o status de Problema resolvível quando o status de Objeto de resolução é alterado]**

  Esta configuração permite correlacionar a resolução do problema original com a resolução do novo objeto (tarefa ou projeto).

  Com essa configuração habilitada (marcada), você pode criar status personalizados de problemas que tenham a mesma chave de status de uma tarefa ou projeto. Quando a tarefa ou projeto (objeto resolvível) é definido com o status personalizado, a alteração também é mostrada no status do problema.

  Quando desabilitada, o status do objeto de resolução é definido automaticamente com o status padrão, em vez dos status personalizados.

  Para que esta configuração tenha algum efeito, a opção “[!UICONTROL Manter problema original e vincular sua resolução à tarefa]” deve ser selecionada.

* **[!UICONTROL Manter problema original e vincular a resolução à tarefa/projeto]**

  Quando o problema é convertido, isso instrui o [!DNL Workfront] a manter os problemas originais. O status do problema muda conforme o status da tarefa ou do projeto é alterado. Quando a tarefa ou o projeto estiver marcado como concluído, o problema será marcado como resolvido.

  Se essa opção não estiver marcada, o problema original será excluído e somente a tarefa ou o projeto convertido permanecerá.

  Esta configuração afeta o relatório de problemas registrados originalmente em um projeto ou que surgem por meio de uma fila de solicitações do [!DNL Workfront].

* **[!UICONTROL Permitir que o contato principal tenha acesso à tarefa/projeto]**

  Isso concede à pessoa que criou o problema original acesso à tarefa ou projeto criado durante a conversão. Elas podem revisar o trabalho, fazer atualizações e se manter informadas sobre o progresso.

* **[!UICONTROL Permitir que estas configurações sejam alteradas durante a conversão]**

  Quando selecionada, esta opção significa que as configurações padrão para “[!UICONTROL Manter problema original]” e “[!UICONTROL Permitir contato principal]” podem ser alteradas pelo usuário que converte o problema. Se quiser que os padrões permaneçam inalterados, desmarque essa opção.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Preferências de datas reais

Existem vários tipos de datas usadas no [!DNL Workfront]. As datas reais são um “carimbo de data/hora” gerado pelo [!DNL Workfront] quando ocorrem determinadas alterações de status.

O carimbo de data e hora [!UICONTROL Data de início efetivo] é criado quando o status do problema muda de Novo para outro status. O carimbo de data e hora [!UICONTROL Data real de conclusão] ocorre quando o status do problema muda para um status que indica que ele está encerrado.

É importante observar que esta preferência controla as configurações de data reais para tarefas e problemas.

Janela de preferências ![[!UICONTROL Tarefas e problemas] com a seção [!UICONTROL Datas reais] destacada](assets/admin-fund-issue-prefs-actual-dates.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda a seção **[!UICONTROL Preferências do projeto]** no painel do menu esquerdo.
1. Selecione **[!UICONTROL Tarefas e problemas]**.
1. Role até a seção **[!UICONTROL Datas reais]**.
1. Selecione a opção desejada para **[!UICONTROL Data de início efetivo]** — [!UICONTROL Agora] (a data e hora atuais) ou[!UICONTROL A data de início planejada] (a [!UICONTROL Data de início efetivo] corresponde à data de início definida nos detalhes do problema).
1. Agora selecione a opção para **[!UICONTROL Data conclusão efetiva]** — [!UICONTROL Agora] (a data e hora atuais) ou [!UICONTROL A data de conclusão planejada] (a [!UICONTROL Data de início efetivo] corresponde à data definida nos detalhes do problema).
1. Salve quando terminar.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Acesso ao problema

As configurações de [!UICONTROL Acesso] para problemas controlam o acesso concedido a um usuário quando um problema é atribuído a ele no Workfront. Essas configurações controlam o acesso ao próprio problema, além do acesso ao projeto ao qual o problema está associado.

Antes de alterar essas configurações, discuta quaisquer necessidades de fluxo de trabalho ou processo com os consultores do [!DNL Workfront] e sua equipe de governança interna.

Janela de preferências ![[!UICONTROL Tarefas e problemas] com a seção [!UICONTROL Quando alguém é atribuído a um PROBLEMA] destacada](assets/admin-fund-issue-prefs-access-1.png)

1. Clique em **[!UICONTROL Configuração]** no **[!UICONTROL Menu principal]**.
1. Expanda a seção **[!UICONTROL Preferências do projeto]** no painel de menu esquerdo.
1. Selecione **[!UICONTROL Tarefas e problemas]**.
1. Role a tela até a seção **[!UICONTROL Acesso]** e encontre a opção “[!UICONTROL Quando alguém é atribuído a um PROBLEMA]”.
1. Defina o acesso de compartilhamento para o problema em si: [!UICONTROL Visualizar],[!UICONTROL  Contribuir] ou [!UICONTROL Gerenciar]. O [!DNL Workfront] recomenda deixar as opções avançadas como estão.
1. Marque a caixa se o responsável pelo problema também deve ter acesso ao projeto
1. Em seguida, selecione o acesso de compartilhamento para o projeto: [!UICONTROL Visualizar],[!UICONTROL Contribuir] ou [!UICONTROL Gerenciar]. À medida que você define as [!UICONTROL Opções avançadas], lembre-se dos fluxos de trabalho e das necessidades de acesso da sua organização.
1. Salve quando terminar.

Janela de ![[!UICONTROL Acesso] mostrando as opções [!UICONTROL Contribuir]](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
