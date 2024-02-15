---
title: Configurar o mapeamento de metadados
description: Saiba como configurar o mapeamento de metadados para o [!UICONTROL Workfront DAM].
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: ht
source-wordcount: '275'
ht-degree: 100%

---

# Configurar o mapeamento de metadados

Informações relacionadas ao [!DNL Workfront] sobre um ativo podem ser transferidas do [!DNL Workfront] para o [!UICONTROL Workfront DAM] com o ativo. A opção de mapeamento de metadados na área [!UICONTROL Configuração] do [!DNL Workfront] permite essa transferência de informações.

Fale com o seu consultor do [!DNL Workfront] para saber quais são as práticas recomendadas para a configuração do mapeamento de metadados.

Você precisa ser a pessoa responsável pela administração do [!DNL Workfront] e do [!UICONTROL Workfront DAM] para configurar o mapeamento de metadados. Antes de começar, você precisa conectar as suas contas do [!DNL Workfront] e do [!UICONTROL Workfront DAM].

## Conectar contas

1. Faça logon no [!DNL Workfront].
1. Abra um projeto, tarefa ou problema, e clique na guia **[!UICONTROL Documentos]**.
1. Clique no botão **[!UICONTROL Adicionar novo]** e selecione **[!UICONTROL Do Workfront DAM]** no menu suspenso.
1. Digite o seu nome de logon e senha na caixa de autorização do [!UICONTROL Workfront DAM] que aparece.
1. Em seguida, clique em **[!UICONTROL Sim]** para dar ao [!DNL Workfront] acesso à conta do [!UICONTROL DAM].
1. Se necessário, atualize a página para atualizar o acesso ao [!UICONTROL Workfront DAM].

Com essa conexão estabelecida, agora você pode começar a mapear metadados entre os dois sistemas. Certifique-se de já ter criado os campos de metadados necessários no [!UICONTROL Workfront DAM] antes de começar a mapear.

## Configurar o mapeamento

1. Faça logon no [!DNL Workfront].
1. Selecione **[!UICONTROL Configuração]** no [!UICONTROL Menu principal].
1. Expanda a seção **[!UICONTROL Documentos]** no menu do painel esquerdo.
1. Então, clique em **[!UICONTROL Mapeamento de metadados]**.
1. No campo do Workfront, digite a origem do campo do [!DNL Workfront] a ser mapeado.
1. Em seguida, selecione o campo de metadados correspondente ou de destino do **[!UICONTROL Workfront DAM]**.
1. Clique no botão **[!UICONTROL Adicionar mapeamento]**.
1. Você verá a [!UICONTROL Origem do campo do Workfront] e o [!UICONTROL Campo de destino do Workfront DAM] no gráfico exibido na parte inferior da janela.
1. Repita o procedimento para todos os campos de metadados desejados.

![Uma captura de tela da tela [!UICONTROL Mapeamento de metadados] no [!DNL Workfront]](assets/01-metadata-mapping.png)
