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
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T22:32:59.006Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 276
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
