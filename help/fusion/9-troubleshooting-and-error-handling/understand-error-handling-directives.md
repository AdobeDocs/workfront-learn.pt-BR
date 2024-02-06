---
title: Entenda as diretivas de manipulação de erros
description: Aprenda sobre as diretivas do manipulador de erros que permitem que a execução continue, bem como as que a interrompem no  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '318'
ht-degree: 100%

---

# Entenda as diretivas de manipulação de erros

Neste vídeo, você aprenderá:

* As três diretivas do manipulador de erros que permitem que a execução continue
* As duas diretivas do manipulador de erros que interrompem a execução

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on)

## Diretivas - O cenário continua

### Retomar

* Uma saída substituta é especificada e fornecida ao módulo que encontra um erro.
* Os módulos subsequentes são processados.
* O status de execução do cenário é marcado como “sucesso”.

![Uma imagem de uma diretiva Retomar](assets/troubleshooting-and-error-handling-2.png)

### Interrupção

* O estado de execução do cenário é armazenado na fila de execuções incompletas, onde o erro pode ser resolvido manualmente. No entanto, existem algumas exceções que são mencionadas aqui.
* Os módulos subsequentes não são processados.
* Se houver pacotes não processados, a execução do cenário continuará normalmente.
* O status de execução do cenário é marcado como “aviso”.

![Uma imagem de uma diretiva de interrupção](assets/troubleshooting-and-error-handling-3.png)

### Ignorar

* O erro é ignorado e os módulos subsequentes não são processados.
* Se houver pacotes não processados, a execução do cenário continuará normalmente.
* O status de execução do cenário é marcado como “sucesso”.

![Uma imagem de uma diretiva Ignorar](assets/troubleshooting-and-error-handling-4.png)

## Diretivas - Interrupções de cenário

### Reversão

* A execução do cenário é interrompida imediatamente e uma fase de reversão é iniciada em todos os módulos, na tentativa de revertê-los ao seu estado inicial.
* Os módulos subsequentes não são processados.
* Exceto no caso de alguns tipos de erros, o cenário é desativado após o “número de erros consecutivos” especificado nas Configurações do cenário.
* O status de execução do cenário é marcado como “erro”.

>[!NOTE]
>
>Este é o comportamento padrão se nenhuma rota do manipulador de erros estiver anexada ao módulo e a configuração “Permitir armazenamento de execuções incompletas” não estiver marcada nas Configurações do cenário.

![Uma imagem de uma diretiva de reversão](assets/troubleshooting-and-error-handling-5.png)

### Confirmar

* O erro é ignorado e os módulos subsequentes não são processados.
* Se houver pacotes não processados, a execução do cenário continuará normalmente.
* O status de execução do cenário é marcado como “sucesso”.

![Uma imagem de uma diretiva de confirmação](assets/troubleshooting-and-error-handling-6.png)
