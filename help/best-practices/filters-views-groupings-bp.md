---
title: 'Prática recomendada: filtros, visualizações e agrupamentos'
description: Explore as práticas recomendadas de especialistas do Adobe Workfront sobre a configuração, gerenciamento e uso de filtros, visualizações e agrupamentos do Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: ht
source-wordcount: '785'
ht-degree: 100%

---

# Prática recomendada: filtros, visualizações e agrupamentos

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, primeiro você encontrará uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem se aprofundar nos detalhes do “porquê”.

A seção “Por que essas práticas recomendadas?” , encontrada após a lista resumida, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta ou recurso que você deve considerar implementar na sua instância do Workfront.

</br>
</br>

## Práticas recomendadas sobre filtros, visualizações e agrupamentos

* Reduza o número de relatórios personalizados que você cria utilizando filtros, visualizações e agrupamentos para obter os dados necessários em uma lista de objetos.

* Use os controles de lista em modelos de layout para ocultar filtros, visualizações e agrupamentos desnecessários em objetos usados com frequência (projetos, tarefas, programas etc.).

* Compartilhe filtros, exibições e agrupamentos personalizados que são relevantes para os fluxos de trabalho e processos da sua organização através dos controles de lista nos modelos de layout.

* Ao criar filtros para o status do projeto, tarefa ou problema, use a origem/nome de campo “(objeto)>>Status igual a” com o modificador Igual, em vez do campo “Projeto>>Status”.

</br>
</br>

## Por que essas práticas são recomendadas?

**Prática recomendada**

Reduza o número de relatórios personalizados que você cria utilizando filtros, visualizações e agrupamentos para obter os dados necessários em uma lista de objetos.

**Entenda o porquê**

Criar relatórios de uso único para cada segmento de dados que você deseja ver é um processo demorado e desorganiza o sistema do Workfront.

Para obter instruções sobre como criar relatórios com prompts, consulte o capítulo &quot;Como configurar e usar prompts de relatório&quot; no vídeo [Entender as configurações do relatório](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/report-settings.html?lang=pt-BR) .

Para obter instruções sobre como criar relatórios com prompts personalizados, consulte [Criar prompts personalizados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/custom-prompts.html?lang=pt-BR).

</br>
</br>

**Prática recomendada**

Use os controles de lista em modelos de layout para ocultar filtros, visualizações e agrupamentos desnecessários em objetos usados com frequência (projetos, tarefas, programas etc.).

**Entenda o porquê**

Menos é mais. Ocultar opções de filtros, visualizações e agrupamentos que não são relevantes para os fluxos de trabalho diários dos usuários restringe as listas, o que torna mais fácil e rápido encontrar o item necessário.

Para obter instruções sobre como ocultar filtros, visualizações ou agrupamentos com modelos de layout, consulte [Personalizar listas de relatórios com modelos de layout](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html?lang=pt-BR).

</br>
</br>

**Prática recomendada**

Compartilhe filtros, exibições e agrupamentos personalizados que são relevantes para os fluxos de trabalho e processos da sua organização através dos controles de lista nos modelos de layout.

**Entenda o porquê**

Se você criou filtros, visualizações e agrupamentos que exibem informações específicas sobre os processos diários dos usuários, é fácil compartilhá-los através dos modelos de layout. Isso garante que todas as pessoas atribuídas a esse modelo de layout tenham opções de filtros, visualizações e agrupamentos relevantes para seus fluxos de trabalho.

Personalizar as informações que você deseja exibir aos usuários através dos modelos de layout também economiza o tempo de admins de sistema e de grupo, visto que não precisarão compartilhar cada opção de filtro, visualização ou agrupamento individualmente.

Para obter instruções sobre como compartilhar filtros, exibições ou agrupamentos com modelos de layout, consulte [Personalizar listas de relatórios com modelos de layout](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html?lang=pt-BR).

</br>
</br>

**Prática recomendada**

Ao criar filtros para o status do projeto, tarefa ou problema, use a origem/nome de campo “(objeto)>>Status igual a” com o modificador Igual, em vez do campo “Projeto>>Status”.

**Entenda o porquê**

Usando o campo “(objeto)>>Equivale a”, você inclui todos os status personalizados que têm esse status específico atribuído ao campo “Equivale a” nas configurações de status. Enquanto que configurar o filtro como “(objeto)>>Status > Igual” requer que você selecione status específicos para o filtro. Isto pode dificultar a manutenção do processo, pois você precisará levar em conta esses novos status em vários filtros. Cada filtro precisaria ser aberto e atualizado com o novo status.

Por exemplo, se quiser ver todos os projetos atuais, você pode configurar seu filtro como “Projeto>>Status > Igual > Atual”. Mas se alguém adicionar um status personalizado chamado Ativo e dizer que é equivalente a Atual, esse filtro não encontrará projetos com o status Ativo. No entanto, se você usar “Projeto>>Status igual a > Igual > Atual”, o filtro localizará objetos com o status Atual ou Ativo, pois ambos incluem o status Atual no campo Igual a.
