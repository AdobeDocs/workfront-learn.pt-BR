---
title: Entender as diretivas de manipulação de erros
description: Saiba mais sobre as diretivas do manipulador de erros que permitem que a execução continue e aquelas que interrompem a execução, em [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Entender as diretivas de manipulação de erros

Neste vídeo, você aprenderá:

* As três diretivas de manipulador de erros que permitem que a execução continue
* As duas diretivas de manipulador de erros que interrompem a execução

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12)

## Diretivas — o cenário continua

### Retomar

* Uma saída substituta é especificada e fornecida ao módulo que encontra um erro.
* Os módulos subsequentes são processados.
* O status de execução do cenário é marcado como &quot;sucesso&quot;.

![Uma imagem de uma diretiva Retomar](assets/troubleshooting-and-error-handling-2.png)

### Interrupção

* O estado da execução do cenário é armazenado na fila de execuções incompletas em que o erro pode ser resolvido manualmente. Há, no entanto, algumas exceções que são mencionadas aqui.
* Os módulos subsequentes não são processados.
* Se houver pacotes não processados, a execução do cenário continuará normalmente.
* O status de execução do cenário é marcado como &quot;aviso&quot;.

![Uma imagem de uma diretiva de Interrupção](assets/troubleshooting-and-error-handling-3.png)

### Ignorar

* O erro é ignorado e os módulos subsequentes não são processados.
* Se houver pacotes não processados, a execução do cenário continuará normalmente.
* O status de execução do cenário é marcado como &quot;sucesso&quot;.

![Uma imagem de uma diretiva Ignore](assets/troubleshooting-and-error-handling-4.png)

## Diretivas — interrupções de cenário

### Reversão

* A execução do cenário é interrompida imediatamente e uma fase de reversão é iniciada em todos os módulos em uma tentativa de revertê-los a seu estado inicial.
* Os módulos subsequentes não são processados.
* Exceto alguns tipos de erro, o cenário é desativado após o &quot;número de erros consecutivos&quot; especificado nas configurações de Cenário.
* O status de execução do cenário é marcado como &quot;erro&quot;.

>[!NOTE]
>
>Esse é o comportamento padrão se nenhuma rota de manipulador de erros estiver anexada ao módulo e a configuração &quot;Permitir armazenamento de execuções incompletas&quot; nas configurações de Cenário não estiver marcada.

![Uma imagem de uma diretiva de reversão](assets/troubleshooting-and-error-handling-5.png)

### Confirmar

* O erro é ignorado e os módulos subsequentes não são processados.
* Se houver pacotes não processados, a execução do cenário continuará normalmente.
* O status de execução do cenário é marcado como &quot;sucesso&quot;.

![Uma imagem de uma diretiva de submissão](assets/troubleshooting-and-error-handling-6.png)
