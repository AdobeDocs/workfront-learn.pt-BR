---
title: Detalhes da prova explicados
description: Saiba mais sobre os detalhes por trás de uma prova em [!DNL  Workfront] através do painel de resumo e [!UICONTROL Detalhes do documento] página.
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
kt: 10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 0%

---

# Visão geral dos detalhes da prova

## Exibir detalhes da prova

Como gerente ou proprietário de prova, você pode pesquisar mais a fundo os detalhes por trás de uma prova por meio do painel de resumo e da variável [!UICONTROL Detalhes do documento] página. Comece encontrando sua prova no [!UICONTROL Documentos] de um projeto, tarefa ou problema.

### Painel Resumo

O painel de resumo fornece uma visão geral de alto nível dos detalhes básicos da prova. Use o ícone para expandir o painel quando precisar e recolha quando não precisar. Você pode até mesmo passar o mouse sobre a miniatura da prova para abri-la ou baixá-la.

![Uma imagem da [!UICONTROL Documentos] de um projeto com uma prova selecionada e o painel de resumo expandido. O ícone do painel de resumo e o painel de resumo são destacados.](assets/document-summary.png)

Observação: O [!UICONTROL Aprovações] no painel de resumo é para **documento** aprovações e **não é** vinculado ao processo de revisão e aprovação de prova sobre o qual você tem aprendido neste curso. Os dois processos são separados em [!DNL Workfront].

### [!UICONTROL Detalhes do Documento]

Se você precisar de mais informações sobre a prova, a variável [!UICONTROL Detalhes do documento] O link direciona você para a &quot;página&quot; da prova em [!DNL Workfront].

![Uma imagem da página da prova em [!DNL  Workfront].](assets/document-details.png)

É importante observar que a capacidade de ver informações relacionadas ao processo de revisão depende de suas permissões de revisão de texto em [!DNL Workfront].

Na página da prova, você pode acessar essas seções no menu do painel esquerdo:

* **Atualizações —** Os comentários feitos no visualizador de prova aparecem aqui, com uma tag &quot;comentário de prova&quot;. Você também pode fazer comentários no arquivo, da mesma forma que faz comentários em uma tarefa ou projeto (esses comentários não aparecem no visualizador de prova).
* **Aprovações —** Esta seção destina-se a aprovações de documentos e não aprovações de prova. Os dois tipos de aprovações são processos separados em [!DNL Workfront] e não vincular. Se você estiver usando workflows de prova para suas revisões e aprovações, não usará esta seção.
* **Todas as versões —** Rastreie e gerencie o histórico de versões da prova. Talvez seja mais fácil acessar essas informações no painel de resumo do [!UICONTROL Documentos] lista.
* **Forms personalizada —** Os formulários personalizados são usados em provas para capturar informações específicas da organização. Essas informações podem ser passadas com o arquivo para sistemas integrados de armazenamento de documentos, como [!DNL Workfront] DAM ou [!DNL Adobe’s] AEM. Os formulários personalizados são configurados pelo [!DNL Workfront] administrador de sistema ou administrador de grupo. Fale com sua equipe ou com seus administradores para saber se você usará formulários personalizados em provas.
* **Fluxo de trabalho de prova —** Gerencie ou modifique o workflow atribuído à prova. Você pode abrir esta janela usando o [!UICONTROL Fluxo de trabalho de prova] na prova na [!UICONTROL Documentos] também. Saiba como fazer alterações no workflow com o vídeo Edit a proof workflow .

Vamos analisar mais detalhadamente duas das seções: [!UICONTROL Configurações do visualizador de prova] e [!UICONTROL Atividade de revisão de texto].

### [!UICONTROL Configurações do visualizador de provas]

Essas configurações ajudam a controlar o acesso à prova.

![Uma imagem da [!UICONTROL Configurações do visualizador de prova] na página da prova com o [!UICONTROL Configurações do visualizador de prova] realçada no menu do painel esquerdo.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Exigir logon. Esta prova não pode ser compartilhada com usuários convidados] —** A prova só pode ser compartilhada com pessoas que tenham uma [!DNL Workfront] licença de prova.
* **[!UICONTROL Exigir a assinatura eletrônica das decisões] —** Ao compartilhar uma prova, isso requer que o recipient tenha permissões de prova em [!DNL Workfront] e faz com que eles &quot;assinem eletronicamente&quot; a prova inserindo sua senha de prova quando tomam uma decisão de prova. (Observação: A senha de prova é diferente da sua [!DNL Workfront] senha. A senha de prova não é facilmente acessível, portanto, a maioria dos destinatários não saberá essa senha.) [!DNL Workfront] A recomenda falar com seu [!DNL Workfront] consultor antes de usar esse recurso.
* **[!UICONTROL Bloquear a prova quando todas as decisões necessárias forem tomadas ]—** Isto bloqueia a prova de quaisquer outros comentários, respostas, decisões, etc., uma vez tomada qualquer decisão sobre a prova. Isso bloqueia toda a versão da prova, não apenas um estágio específico do fluxo de trabalho de prova.
* **[!UICONTROL Permitir download do arquivo original] —** Os recipients da prova podem baixar o arquivo de origem original da prova no visualizador de prova (a opção está no menu do painel direito).
* **[!UICONTROL Permitir compartilhamento de prova via URL público ou código incorporado] —** Os recipients de prova podem compartilhar um link de prova acessível publicamente com qualquer pessoa.
* **[!UICONTROL Permitir a assinatura de prova via URL público ou código incorporado] —** Qualquer pessoa que receba o URL público pode se adicionar à prova com seu endereço de email e nome (se não for um usuário de prova) ou seu endereço de email e senha de prova (se for um usuário de prova). (Observação: A senha de prova não é a mesma que uma [!DNL Workfront] password.)

Essas mesmas configurações podem ser definidas quando a prova é carregada na variável [!UICONTROL Configurações de prova] na parte inferior da janela de upload.

![Uma imagem da [!UICONTROL Configurações de prova] na parte inferior da janela de upload.](assets/proof-settings-on-upload-page.png)

### [!UICONTROL Atividade de revisão de texto]

Esta página rastreia toda a atividade que aconteceu na prova, além das mensagens de email que foram enviadas em relação a essa prova.

![Uma imagem da [!UICONTROL Atividade de revisão de texto] da página da prova com a [!UICONTROL Atividade de revisão de texto] realçada no menu do painel esquerdo.](assets/proofing-activity-in-details.png)

O [!UICONTROL Atividade] carimbos de data e hora da seção quando comentários e decisões são feitos, além de quem os fez. Ele também rastreia o início dos estágios do fluxo de trabalho de prova, quando um recipient abriu uma prova pela primeira vez e outras informações que um gerente ou proprietário de prova desejará saber. Esses detalhes podem ser úteis quando você está tentando descobrir coisas como, por que um estágio de fluxo de trabalho de prova nunca foi iniciado, por exemplo.

O [!UICONTROL Mensagens] carimbos de data e hora da seção quando alertas de email e mensagens eram enviados aos recipients, que os enviaram e o conteúdo da mensagem. Isso pode ser útil na solução de problemas se alguém disser que não recebeu um email sobre uma prova. Você pode verificar se e quando um email foi enviado.

[!DNL Workfront] A recomenda que o gerente de prova e o proprietário da prova se familiarizem com as informações nessas duas seções. Quando você combina essas informações com a compreensão de como ler o [!UICONTROL SOCD] na barra de progresso, você pode realmente entender e gerenciar suas provas, independentemente de onde elas estejam no fluxo de trabalho de prova.

Quando terminar de trabalhar no [!UICONTROL Detalhes do documento] use a trilha de navegação para retornar ao [!UICONTROL Documentos] do projeto, tarefa ou emissão à qual a prova está anexada.

![Uma imagem da navegação estrutural no cabeçalho.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
