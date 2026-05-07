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
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:07:23.288Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 318
ht-degree: 100%

---

# Entenda as diretivas de manipulação de erros

Neste vídeo, você aprenderá:

* As três diretivas do manipulador de erros que permitem que a execução continue
* As duas diretivas do manipulador de erros que interrompem a execução

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on&enablevpops=1)

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
