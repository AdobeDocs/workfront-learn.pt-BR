---
title: Prática recomendada - Verificação linguística
description: Explore as recomendações de práticas recomendadas dos especialistas do Adobe Workfront sobre como configurar, gerenciar e usar provas no Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
kt: 10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Prática recomendada - Verificação linguística

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de prova no Workfront

* Reserve tempo para criar modelos de fluxo de trabalho de prova.

* Desative a configuração &quot;Enviar emails do Workfront quando um comentário é feito em uma prova&quot; nas configurações do Workfront.

* Use somente Leitura ou Revisor para a configuração &quot;Funções para não destinatários que abrem uma prova de documento&quot; no Workfront.

* Ajuste as configurações de back-end de prova para que os usuários vejam os prazos em um formato de relógio de 12 horas.

* Estabeleça um prazo de prova padrão como parte das configurações do sistema.

* Ocultar a opção de decisão de prova não relevante.

* Não reordene as opções de decisão de prova nas configurações de prova.

* Defina padrões do usuário para funções de prova e alertas de email.

* Defina a função de prova do criador de prova como Revisor.

* Evite usar a função de prova de Aprovador .

* Evite a opção de alerta de email All Activity proof .

</br>
</br>

## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Reserve tempo para criar modelos de fluxo de trabalho de prova.

**Veja o porquê**

Além de acelerar e simplificar o processo de criação e atribuição de prova, os modelos fornecem consistência em workflows de prova para tipos semelhantes de ativos. Eles também garantem que a cada recipient de prova seja atribuída a função de prova adequada e o alerta por email, e que um prazo tenha sido definido.

</br>
</br>

**Prática recomendada**

Desative a configuração &quot;Enviar emails do Workfront quando um comentário é feito em uma prova&quot; nas configurações do Workfront.



**Veja o porquê**

Quando essa configuração é ativada (o que é por padrão), os usuários têm o potencial de obter várias notificações por email para cada comentário em uma prova, uma a partir da funcionalidade de prova e outra a partir do próprio Workfront. Essas notificações duplicadas geram interrupção e confusão na notificação por email, bem como uma caixa de entrada de email completa, o que pode resultar em usuários ignorarem as notificações de prova recebidas. O que, por sua vez, poderia significar a perda de prazos.



**Observação**: Esta configuração é encontrada no Menu principal do Workfront > Configuração > Email > Revisar e aprovar.

</br>
</br>

**Prática recomendada**

Use somente Leitura ou Revisor para a configuração &quot;Funções para não destinatários que abrem uma prova de documento&quot; no Workfront.



**Veja o porquê**

As outras opções para essa configuração exigem uma decisão de prova, que pode descarrilar seu fluxo de trabalho de prova. Geralmente, as pessoas que não são adicionadas ao workflow de prova precisam apenas exibir a prova ou fazer comentários, não aprovar a prova, portanto, as opções Somente leitura ou Revisor são a melhor opção.



**Observação**: Esta configuração é encontrada no Menu principal do Workfront > Configuração > Revisar e aprovar.

</br>
</br>

**Prática recomendada**

Ajuste as configurações de back-end de prova para que os usuários vejam os prazos em um formato de relógio de 12 horas.



**Veja o porquê**

Selecione a opção F j, Y, gi:a nas configurações de prova para usuários que desejam ver prazos/horas de prova em um formato AM/PM. Para áreas que usam um relógio de 12 horas, isso ajuda na clareza do prazo.



**Observação**: Essa configuração é encontrada indo até o Menu principal do Workfront > Verificação linguística > Configurações da conta > Usuários > e editando o campo Formato da data para cada usuário.

</br>
</br>

**Prática recomendada**

Estabeleça um prazo de prova padrão como parte das configurações do sistema.



**Veja o porquê**

Quando um prazo de prova padrão é definido, a data de upload + x número de dias úteis, se o criador de prova se esquecer de adicionar um prazo, o Workfront aplica automaticamente esse prazo a todas as provas enviadas por upload.



**Observação**: Essa configuração é encontrada indo até o campo Menu principal do Workfront > Verificação linguística > Configurações da conta > Configurações > Padrões de prova > Prazo final (+ dias úteis) .

</br>
</br>


**Prática recomendada**

Ocultar a opção de decisão de prova não relevante.



**Veja o porquê**

Essa opção de decisão geralmente causa confusão entre aprovadores, já que as organizações geralmente não definem quando a opção Não relevante deve ser usada. A opção Não relevante geralmente indica que a prova não é relevante para o destinatário da prova e não é necessário tomar uma decisão aprovada ou rejeitada. Ao selecionar Não relevante, isso permite que o fluxo de trabalho de prova continue.


A opção Não relevante não é necessária na maioria dos workflows de prova.

**Observação**: Essa configuração é encontrada indo até o Menu principal do Workfront > Verificação linguística > Configurações da conta > Decisões.

</br>
</br>

**Prática recomendada**

Não reordene as opções de decisão de prova nas configurações de prova.



**Veja o porquê**

Cada configuração de decisão de prova contém um valor/peso específico que, se reordenado, pode gerar confusão nas configurações de prova. A ordem de decisão e o valor/peso são usados como acionadores de ativação de estágio de prova e no relatório.



**Observação**: Essa configuração é encontrada indo até o Menu principal do Workfront > Verificação linguística > Configurações da conta > Decisões.

</br>
</br>

**Prática recomendada**

Defina padrões do usuário para funções de prova e alertas de email.



**Veja o porquê**

Essas configurações são preenchidas automaticamente ao atribuir um workflow de prova, acelerar o processo e contribuir para a consistência entre workflows de prova.



**Observação**: As configurações padrão do usuário são encontradas ao acessar o Menu principal do Workfront > Verificação linguística > Configurações da conta > Usuários > e selecionar o usuário para definir padrões.

</br>
</br>

**Prática recomendada**

Defina a função de prova do criador de prova como Revisor.



**Veja o porquê**

A função de prova do revisor garante que o criador de prova possa fazer comentários e acessar comentários deixados por outras pessoas. Na maioria das vezes, o criador de prova não é obrigado a tomar uma decisão em uma prova que carregou. As funções de prova de Aprovador, Revisor e Aprovador, Autor ou Moderador exigem que seja tomada uma decisão. Se o criador de prova receber uma dessas funções de prova, mas nunca tomar uma decisão, isso pode afetar negativamente os prazos de prova.

</br>
</br>

**Prática recomendada**

Evite usar a função de prova de Aprovador .



**Veja o porquê**

A função de prova de Aprovador não permite que o usuário faça comentários nessa prova. Isso poderia levar um usuário a rejeitar a prova, sem nenhuma explicação, pois não poderia fazer comentários. Em vez disso, use a função de prova Revisor e Aprovador para que o usuário possa fornecer feedback.

</br>
</br>

**Prática recomendada**

Evite a opção de alerta de email All Activity proof .

**Veja o porquê**

Essa opção envia uma notificação por email de prova sempre que algo ocorrer com uma prova, um comentário é feito, uma resposta é postada, uma decisão é tomada etc. O recipient basicamente está vendo a atividade de prova conforme ocorre.

Para proprietários e criadores de prova, o alerta por email Decisões funciona melhor para fluxos de trabalho de prova em vários estágios e a Decisão Final funciona melhor para fluxos de trabalho de único estágio. Geralmente, todos os outros podem ser definidos como Desativado, a menos que desejam ser notificados de outras pessoas que fazem comentários ou decisões (nesse caso, uma das opções de email resumidas pode funcionar melhor).
