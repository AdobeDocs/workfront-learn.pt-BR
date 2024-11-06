---
title: 'Prática recomendada: revisão'
description: Conheça as sugestões de práticas recomendadas por especialistas do Adobe Workfront para configurar, gerenciar e usar revisões no Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: af71439e222061cf468b78dfe1807f0b4893c52a
workflow-type: tm+mt
source-wordcount: '1182'
ht-degree: 91%

---

# Prática recomendada: revisão

## O que é uma “prática recomendada” do Adobe Workfront?

As práticas recomendadas são diretrizes para um curso de ação eficaz e eficiente; elas podem ser facilmente adotadas por qualquer usuário da empresa e replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para um determinado assunto. Use essas práticas recomendadas como uma base para orientar as configurações e o uso do sistema do Workfront.

## Navegar nesta página

Ao percorrer esta página, primeiro você encontrará uma lista resumida de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem se aprofundar nos detalhes do “porquê”.

A seção “Por que essas práticas recomendadas?” , encontrada após a lista resumida, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta ou recurso que você deve considerar implementar na sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para revisão no Workfront

* Reserve um tempo para criar modelos de fluxo de trabalho de revisão.

* Desative a configuração &quot;Enviar emails do Workfront quando um comentário for feito em uma prova&quot; nas configurações do Workfront.

* Use Somente leitura ou Revisor para a configuração “Funções para não destinatários que abrirem uma prova de documento” no Workfront.

* Ajuste as configurações de back-end de revisão, para que os usuários vejam os prazos no formato de 12 horas.

* Estabeleça um prazo de revisão padrão como parte das configurações do sistema.

* Oculte a opção de revisão de prova “Não relevante”.

* Não reordene as opções de decisão de revisão nas configurações de revisão.

* Defina os padrões do usuário para funções de revisão e alertas por email.

* Defina a função de prova do(a) criador(a) da revisão como “Revisor”.

* Evite usar a função de revisão “Aprovador”.

* Evite a opção de alerta por email de revisão “Todas as atividades”.

</br>
</br>

## Por que essas práticas são recomendadas?

**Prática recomendada**

Reserve um tempo para criar modelos de fluxo de trabalho de revisão.

**Entenda o porquê**

Além de acelerar e simplificar o processo de criação e atribuição de revisões, os modelos também fornecem consistência em workflows de revisão para tipos semelhantes de ativo. Eles também garantem que cada recipient da revisão receba a função de revisão e o alerta por email adequados, e que um prazo tenha sido definido.

</br>
</br>

**Prática recomendada**

Desative a configuração &quot;Enviar emails do Workfront quando um comentário for feito em uma prova&quot; nas configurações do Workfront.



**Entenda o porquê**

Quando essa configuração está habilitada (por padrão), os usuários têm a possibilidade de receber diversas notificações por email para cada comentário em uma revisão, uma da funcionalidade de revisão e outra do próprio Workfront. Essas notificações duplicadas levam à interrupção e confusão das notificações por email, bem como a uma caixa de entrada de email cheia, o que pode fazer com que os usuários ignorem as notificações de revisão recebidas. O que, por sua vez, pode significar prazos perdidos.



**Observação**: esta configuração do Workfront é encontrada em Menu principal > Configuração > Email > Revisão e aprovação.

</br>
</br>

**Prática recomendada**

Use Somente leitura ou Revisor para a configuração “Funções para não destinatários que abrirem uma prova de documento” no Workfront.



**Entenda o porquê**

Todas as outras opções dessa configuração exigem que uma decisão de revisão seja tomada, o que pode atrapalhar seu fluxo de trabalho de revisão. Geralmente, as pessoas que não são adicionadas ao fluxo de trabalho da revisão só precisam visualizar a revisão ou fazer comentários, não aprovar a revisão; portanto, as opções “Somente leitura” ou “Revisor” são a sua melhor escolha.



**Observação**: esta configuração do Workfront é encontrada em Menu principal > Configuração > Revisão e aprovação.

</br>
</br>

**Prática recomendada**

Ajuste as configurações de back-end de revisão, para que os usuários vejam os prazos no formato de 12 horas.



**Entenda o porquê**

O padrão é um formato de relógio de 24 horas, que pode ser confuso para aqueles que não estão familiarizados com ele. Para alterar o formato, vá para o menu principal do Workfront > Revisão de texto > Configurações da conta > Usuários. Clique duas vezes em um usuário para selecionar um e, em seguida, edite o campo Formato de data na seção Configurações pessoais. Você precisará selecionar cada usuário, um de cada vez, para alterá-los.

</br>
</br>

**Prática recomendada**

Estabeleça um prazo de revisão padrão como parte das configurações do sistema.



**Entenda o porquê**

Quando um prazo de revisão padrão é definido (a data de upload x a quantidade de dias úteis), se o criador da revisão se esquecer de adicionar um prazo, o Workfront aplicará automaticamente esse prazo a todas as revisões carregadas.



**Observação**: esta configuração do Workfront é encontrada em Menu principal > Revisão > Configurações da conta > Configurações > Padrões de revisão > Prazo (+ dias úteis).

</br>
</br>


**Prática recomendada**

Oculte a opção de revisão de prova “Não relevante”.



**Entenda o porquê**

Essa opção de decisão muitas vezes causa confusão entre os aprovadores, pois muitas vezes as organizações não definem quando a opção “Não relevante” deve ser usada. A opção “Não relevante” geralmente indica que a revisão não é relevante para o destinatário da revisão e que ele não precisa tomar nenhuma decisão de aprovação ou rejeição. Selecionar “Não relevante” permite que o fluxo de trabalho de revisão continue.


A opção “Não relevante” não é necessária na maioria dos workflows de revisão.

**Observação**: esta configuração do Workfront é encontrada em Menu principal > Revisão > Configurações da conta > Decisões.

</br>
</br>

**Prática recomendada**

Não reordene as opções de decisão de revisão nas configurações de revisão.



**Entenda o porquê**

Cada configuração de decisão de revisão contém um valor/peso específico que, se reordenado, pode causar confusão nas suas configurações de revisão. A ordem de decisão e o valor/peso são usados como desencadeadores de ativação do estágio de revisão e nos relatórios.



**Observação**: esta configuração do Workfront é encontrada em Menu principal > Revisão > Configurações da conta > Decisões.

</br>
</br>

**Prática recomendada**

Defina os padrões do usuário para funções de revisão e alertas por email.



**Entenda o porquê**

Essas configurações são preenchidas automaticamente quando um fluxo de trabalho de revisão é atribuído, acelerando o processo e contribuindo para a consistência entre os workflows de revisão.



**Observação**: as configurações padrão do usuário são encontradas acessando o Menu principal do Workfront > Revisão > Configurações da conta > Usuários > e selecionando o usuário para o qual deseja definir os padrões.

</br>
</br>

**Prática recomendada**

Defina a função de prova do(a) criador(a) da revisão como “Revisor”.



**Entenda o porquê**

A função de prova “Revisor” garante que o criador da prova possa fazer comentários e acessar comentários feitos por outras pessoas. Na maioria das vezes, o(a) criador(a) da revisão não tem a obrigação de tomar uma decisão sobre a revisão que carregou. As funções de prova “Aprovador”, “Revisor e Aprovador”, “Autor” ou “Moderador” exigem a tomada de uma decisão. Se o criador da prova receber uma dessas funções, mas não tomar nenhum decisão, isso poderá afetar negativamente os prazos das provas.

</br>
</br>

**Prática recomendada**

Evite usar a função de revisão “Aprovador”.



**Entenda o porquê**

A função “Aprovador” não permite que o usuário faça comentários nesta prova. Isso poderia levar um usuário a rejeitar a prova, sem qualquer explicação, pois não seria possível fazer comentários. Utilize a função de prova “Revisor e Aprovador” para que o usuário possa fornecer feedback.

</br>
</br>

**Prática recomendada**

Evite a opção de alerta por email de revisão “Todas as atividades”.

**Entenda o porquê**

Esta opção envia uma notificação por email sobre a prova sempre que algo acontece, como quando um comentário é feito, uma resposta é postada, uma decisão é tomada etc. O recipient essencialmente vê a atividade da prova conforme ela acontece.

Para proprietários e criadores de provas, o alerta por email de Decisões funciona melhor para workflows de prova de vários estágios e a Decisão final funciona melhor para workflows de estágio único. Geralmente, todos os outros usuários podem ser definidos como Desabilitados, a menos que queiram ser notificados sobre comentários ou decisões de outras pessoas (nesse caso, uma das opções de resumo por email pode funcionar melhor).
