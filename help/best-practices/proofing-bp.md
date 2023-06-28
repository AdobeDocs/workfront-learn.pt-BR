---
title: Prática recomendada - Prova
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre a configuração, gerenciamento e uso de provas no Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Prática recomendada - Prova

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Prova nas práticas recomendadas do Workfront

* Reserve tempo para criar modelos de fluxo de trabalho de provas.

* Desative a configuração &quot;Enviar emails do Workfront quando um comentário for feito em uma prova&quot; nas configurações do Workfront.

* Use somente leitura ou Revisor para a configuração &quot;Funções para não destinatários que abrem uma prova de documento&quot; no Workfront.

* Ajuste as configurações de back-end da prova para que os usuários vejam os prazos em um formato de relógio de 12 horas.

* Estabeleça um prazo de prova padrão como parte das configurações do sistema.

* Oculte a opção Não relevante para decisão de prova.

* Não reordene as opções de decisão da prova nas configurações de prova.

* Defina os padrões do usuário para funções de prova e alertas de email.

* Defina a função de prova do criador da prova como Revisor.

* Evite usar a função de prova Aprovador.

* Evite a opção de alerta por email de prova de Todas as atividades.

</br>
</br>

## Por que essas práticas recomendadas?

**Prática recomendada**

Reserve tempo para criar modelos de fluxo de trabalho de provas.

**Veja o porquê**

Os modelos não apenas aceleram e simplificam o processo de criação e atribuição de provas, como também fornecem consistência entre fluxos de trabalho de prova para tipos semelhantes de ativos. Elas também garantem que cada recipient de prova receba a função de prova e o alerta de email adequados, e que um prazo tenha sido definido.

</br>
</br>

**Prática recomendada**

Desative a configuração &quot;Enviar emails do Workfront quando um comentário for feito em uma prova&quot; nas configurações do Workfront.



**Veja o porquê**

Quando essa configuração estiver ativada (que é por padrão), os usuários têm o potencial de obter várias notificações por email para cada comentário em uma prova, uma da funcionalidade de prova e outra do próprio Workfront. Essas notificações duplicadas causam confusão e interrupção de notificações por email, bem como uma caixa de entrada de email completa, que pode resultar no ignoramento de notificações de prova recebidas pelos usuários. O que, por sua vez, poderia significar o não cumprimento de prazos.



**Nota**: essa configuração é encontrada no Menu principal do Workfront > Configuração > Email > Revisão e aprovação.

</br>
</br>

**Prática recomendada**

Use somente leitura ou Revisor para a configuração &quot;Funções para não destinatários que abrem uma prova de documento&quot; no Workfront.



**Veja o porquê**

As outras opções dessa configuração exigem que seja tomada uma decisão de prova, o que pode prejudicar seu fluxo de trabalho de prova. Geralmente, as pessoas que não são adicionadas ao fluxo de trabalho de prova precisam apenas visualizar a prova ou fazer comentários, não aprovar realmente a prova, portanto, as opções Somente leitura ou Revisor são a melhor opção.



**Nota**: essa configuração é encontrada no Menu principal do Workfront > Configuração > Revisão e aprovação.

</br>
</br>

**Prática recomendada**

Ajuste as configurações de back-end da prova para que os usuários vejam os prazos em um formato de relógio de 12 horas.



**Veja o porquê**

Selecione a opção F j, Y, gi:a nas configurações de prova para usuários que desejam ver prazos/horas de prova em um formato AM/PM. Para áreas que usam um relógio de 12 horas, isso ajuda na clareza do prazo.



**Nota**: essa configuração é encontrada acessando o Menu principal do Workfront > Revisão > Configurações da conta > Usuários > e editando o campo Formato de data para cada usuário.

</br>
</br>

**Prática recomendada**

Estabeleça um prazo de prova padrão como parte das configurações do sistema.



**Veja o porquê**

Quando um prazo de prova padrão é definido (a data de upload + x número de dias úteis), se o criador da prova esquecer de adicionar um prazo, a Workfront aplicará automaticamente esse prazo a todas as provas carregadas.



**Nota**: essa configuração é encontrada no campo Menu principal do Workfront > Revisão > Configurações da conta > Configurações > Padrões de prova > Prazo final (+ dias úteis).

</br>
</br>


**Prática recomendada**

Oculte a opção Não relevante para decisão de prova.



**Veja o porquê**

Essa opção de decisão geralmente causa confusão entre aprovadores, já que as organizações geralmente não definem quando a opção Não relevante deve ser usada. A opção Não relevante geralmente indica que a prova não é relevante para o recipient da prova e que ele não precisa tomar uma decisão aprovada ou rejeitada. Ao selecionar Não relevante, permite que o fluxo de trabalho de prova continue.


A opção Not Relevant não é necessária na maioria dos workflows de prova.

**Nota**: essa configuração é encontrada acessando o Menu principal do Workfront > Revisão > Configurações da conta > Decisões.

</br>
</br>

**Prática recomendada**

Não reordene as opções de decisão da prova nas configurações de prova.



**Veja o porquê**

Cada configuração de decisão de prova contém um valor/peso específico que, se reordenado, pode causar confusão nas configurações da prova. A ordem de decisão e o valor/peso são usados como acionadores de ativação do estágio de prova e nos relatórios.



**Nota**: essa configuração é encontrada acessando o Menu principal do Workfront > Revisão > Configurações da conta > Decisões.

</br>
</br>

**Prática recomendada**

Defina os padrões do usuário para funções de prova e alertas de email.



**Veja o porquê**

Essas configurações são preenchidas automaticamente ao atribuir um fluxo de trabalho de prova, acelerar o processo e contribuir para a consistência entre fluxos de trabalho de prova.



**Nota**: as configurações padrão do usuário são encontradas ao acessar o Menu principal do Workfront > Revisão de texto > Configurações da conta > Usuários > e selecionar o usuário para o qual definir os padrões.

</br>
</br>

**Prática recomendada**

Defina a função de prova do criador da prova como Revisor.



**Veja o porquê**

A função de prova Revisor garante que o criador da prova possa fazer comentários e acessar comentários deixados por outros. Na maioria das vezes, o criador da prova não é obrigado a tomar uma decisão sobre uma prova que carregou. As funções de prova Aprovador, Revisor e Aprovador, Autor ou Moderador exigem que seja tomada uma decisão. Se o criador da prova receber uma dessas funções de prova, mas nunca tomar uma decisão, isso poderá afetar negativamente os prazos de prova.

</br>
</br>

**Prática recomendada**

Evite usar a função de prova Aprovador.



**Veja o porquê**

A função de Aprovador de prova não permite que o usuário faça comentários nesta prova. Isso pode levar um usuário a rejeitar a prova, sem qualquer explicação, porque não pode fazer comentários. Em vez disso, use a função de prova Revisor e Aprovador para que o usuário possa fornecer feedback.

</br>
</br>

**Prática recomendada**

Evite a opção de alerta por email de prova de Todas as atividades.

**Veja o porquê**

Essa opção envia uma notificação por email de prova sempre que algo acontece com uma prova: um comentário é feito, uma resposta é postada, uma decisão é tomada, etc. O recipient está essencialmente vendo a atividade de prova à medida que ela acontece.

Para proprietários e criadores de provas, o alerta por email de Decisões funciona melhor para fluxos de trabalho de prova de vários estágios e a Decisão final funciona melhor para fluxos de trabalho de estágio único. Geralmente, todos os outros podem ser definidos como Desativado, a menos que queiram ser notificados sobre outras pessoas que estejam fazendo comentários ou tomando decisões (nesse caso, uma das opções de resumo de email pode funcionar melhor).
