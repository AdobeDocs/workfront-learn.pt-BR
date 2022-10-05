---
title: Entenda as diretivas de tratamento de erros
description: Saiba mais sobre as diretivas do manipulador de erros que permitem a continuação da execução e as que interrompem a execução, em [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Entender diretivas de tratamento de erros

Neste vídeo, você aprenderá:

* As três diretivas do manipulador de erros que permitem continuar a execução
* As duas diretivas do manipulador de erros que interrompem a execução

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12)

## Diretivas — O cenário continua

### Retomar

* Uma saída substituta é especificada e fornecida ao módulo que encontra um erro.
* Os módulos subsequentes são processados.
* O status de execução do cenário é marcado como &quot;sucesso&quot;.

![Uma imagem de uma diretiva Resume](assets/troubleshooting-and-error-handling-2.png)

### Quebra

* O estado da execução do cenário é armazenado na fila de execuções incompletas, onde o erro pode ser resolvido manualmente. Há, no entanto, algumas exceções que aqui são mencionadas.
* Os módulos subsequentes não são processados.
* Se houver pacotes não processados, a execução do cenário continuará normalmente.
* O status de execução do cenário é marcado como &quot;aviso&quot;.

![Uma imagem de uma diretiva Break](assets/troubleshooting-and-error-handling-3.png)

### Ignorar

* O erro é ignorado e os módulos subsequentes não são processados.
* Se houver pacotes não processados, a execução do cenário continuará normalmente.
* O status de execução do cenário é marcado como &quot;sucesso&quot;.

![Uma imagem de uma diretiva Ignore](assets/troubleshooting-and-error-handling-4.png)

## Diretivas — Cenário interrompe

### Reversão

* A execução do cenário é interrompida imediatamente e uma fase de reversão é iniciada em todos os módulos na tentativa de revertê-los para o estado inicial.
* Os módulos subsequentes não são processados.
* Com alguns tipos de erro, o cenário é desativado após o &quot;número de erros consecutivos&quot; especificado nas Configurações do cenário.
* O status de execução do cenário é marcado como &quot;erro&quot;.

>[!NOTE]
>
>Esse é o comportamento padrão se nenhuma rota do manipulador de erros estiver anexada ao módulo e a configuração &quot;Permitir o armazenamento de execuções incompletas&quot; nas configurações de Cenário não estiver marcada.

![Uma imagem de uma diretiva de reversão](assets/troubleshooting-and-error-handling-5.png)

### Confirmar

* O erro é ignorado e os módulos subsequentes não são processados.
* Se houver pacotes não processados, a execução do cenário continuará normalmente.
* O status de execução do cenário é marcado como &quot;sucesso&quot;.

![Uma imagem de uma diretiva Commit](assets/troubleshooting-and-error-handling-6.png)
