---
title: Prática recomendada - Licenças e níveis de acesso
description: Explore as recomendações de práticas recomendadas dos especialistas da Adobe Workfront sobre como configurar, gerenciar e usar licenças e níveis de acesso do Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 0%

---

# Prática recomendada - Licenças e níveis de acesso

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As melhores práticas são orientações que representam uma linha de ação eficaz e eficiente; sejam adotados facilmente por você e pelos usuários em sua empresa; e podem ser replicados com êxito em toda a organização.

À medida que você revisa essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas para o tópico. Use essas práticas recomendadas como estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegar nesta página

Ao rolar por essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite que você revise as recomendações sem entrar nos detalhes de &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas estão sendo usadas?&quot; , encontrada após a lista de alto nível, fornece mais detalhes sobre algumas práticas recomendadas e por que elas são consideradas como um processo, ferramenta etc., você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas de licenças e níveis de acesso

* Comece com menos acesso para usuários ao configurar níveis de acesso.

* Ao atribuir licenças de Revisão e Solicitação, normalmente o padrão é Revisar, pois fornece ao usuário mais permissões no Adobe Workfront.

* Desmarque a caixa de seleção &quot;Compartilhar todo o sistema&quot; em cada objeto em todos os níveis de acesso, a menos que você deseje especificamente que esses usuários possam fazê-lo.

* Considere ativar a configuração &quot;Nunca permitir que usuários excluam comentários&quot; em Definir restrições adicionais em um nível de acesso.

* Limite o número de administradores de sistema em favor de administradores de grupo.

* Copie um nível de acesso existente e faça modificações, em vez de criar um novo nível de acesso do zero.

* Documente o que cada nível de acesso pode fazer na caixa Descrição.

* Limite-se somente aos níveis de acesso necessários para atingir suas metas de trabalho, idealmente quatro ou cinco que capturem as necessidades da maioria dos usuários do sistema.

* Atribua pelo menos dois usuários ao nível global de acesso do administrador do sistema.

* Restrinja o que os usuários podem fazer com itens do Workfront por meio do compartilhamento, em vez de remover um recurso em um nível de acesso.

</br>
</br>


## Por que essas práticas recomendadas estão presentes?

**Prática recomendada**

Comece com menos acesso para usuários ao configurar níveis de acesso.



**Veja o porquê**

Inicie os usuários com o acesso mínimo que eles precisarão para fazer seu trabalho. Se eles não puderem realizar suas tarefas devido a direitos de acesso insuficientes, normalmente solicitarão acesso adicional. Conceder aos usuários acesso excessivo imediatamente pode levar a problemas de segurança. Além disso, é sempre melhor dar aos usuários mais acesso do que remover o acesso.

</br>
</br>



**Prática recomendada**

Ao atribuir licenças de Revisão e Solicitação, normalmente o padrão é Revisar, pois fornece ao usuário mais permissões no Adobe Workfront.



**Veja o porquê**

Embora as licenças de Revisão e Solicitação possam ser atribuídas a um número ilimitado de usuários no Workfront, as licenças de Solicitação estão limitadas a apenas fazer e atualizar solicitações. Uma licença de Revisão tem mais acesso a projetos e tarefas do que uma licença de Solicitação, bem como a possibilidade de visualizar portfólios e programas, editar documentos e acessar ferramentas de gerenciamento de recursos.

</br>
</br>

**Prática recomendada**

Desmarque a caixa de seleção &quot;Compartilhar todo o sistema&quot; em cada objeto em todos os níveis de acesso, a menos que haja um motivo específico para os usuários poderem compartilhar o sistema inteiro.



**Veja o porquê**

O compartilhamento de um objeto em todo o sistema geralmente é usado como uma multa para permitir que determinados usuários vejam itens no Workfront. Isso acontece quando a estrutura de grupo do Workfront está ausente ou quando as permissões de compartilhamento não são totalmente compreendidas. Quando os itens são compartilhados no sistema, significa que todos podem ver o item compartilhado. Dependendo do tipo de informação que está sendo mantida no sistema, isso pode levar a problemas de privacidade.



Por exemplo, você pode estar trabalhando com vários fornecedores dentro do Workfront para verificar o progresso, fornecer aprovações etc. Se a caixa de seleção &quot;Compartilhar sistema inteiro&quot; for uma opção, que pode ser selecionada ou definida como padrão, disponibilizando informações para todos os fornecedores.



Ao desmarcar a opção completamente, você faz com que seja um usuário, com permissão para compartilhar, que deve determinar a pessoa ou pessoas específicas — por meio de uma empresa, grupo ou equipe — com as quais deseja compartilhar o objeto.

</br>
</br>

**Prática recomendada**

Considere ativar a configuração &quot;Nunca permitir que usuários excluam comentários&quot; em Definir restrições adicionais em um nível de acesso.



**Veja o porquê**

Ativar essa opção garante que as comunicações anteriores não sejam removidas da Workfront. Algumas organizações exigem que o histórico completo de comentários seja mantido para fins de auditoria.

</br>
</br>

**Prática recomendada**

Limite o número de administradores de sistema em favor de administradores de grupo.



**Veja o porquê**

Os administradores de sistema têm acesso a tudo no Workfront, inclusive às configurações globais do sistema. Os administradores do grupo de configurações podem acessar são controlados pelo administrador do sistema e se aplicam somente a esse grupo específico.



Ter administradores de grupo permite que os administradores do sistema deleguem muitas responsabilidades, permitindo que eles se concentrem em itens de imagem maiores, em vez da manutenção diária do Workfront. Os administradores de grupo podem manter-se mais facilmente em contato com as necessidades de seus grupos, o que oferece melhor serviço aos usuários.

</br>
</br>


**Prática recomendada**

Copie um nível de acesso existente e faça modificações, em vez de criar um novo nível de acesso do zero.



**Veja o porquê**

A cópia de um nível de acesso existente fornece uma base consistente para novos níveis de acesso, garantindo que as configurações iniciais sejam idênticas. Isso também economiza tempo, pois os administradores do sistema não precisarão configurar um nível de acesso totalmente do zero.

</br>
</br>

**Prática recomendada**

Documente o que cada nível de acesso pode fazer na caixa Descrição.



**Veja o porquê**

Seja detalhado com a descrição, listando as configurações para cada tipo de objeto. Isso ajuda os administradores do sistema — presentes e futuros — a saber exatamente o que cada nível de acesso faz sem precisar mergulhar no próprio nível de acesso para analisar as configurações.



Isso também pode facilitar a comparação dos níveis de acesso ao analisá-los em um relatório. O campo de descrição pode ser adicionado rapidamente à exibição para ver rapidamente como elas diferem e, possivelmente, por que um nível de acesso diferente foi criado.

</br>
</br>

**Prática recomendada**

Limite-se somente aos níveis de acesso necessários para atingir suas metas de trabalho, idealmente quatro ou cinco que capturem as necessidades da maioria dos usuários do sistema.


**Veja o porquê**

O nível de acesso garante que, quando um objeto do Workfront é compartilhado com um usuário, ele tenha os direitos necessários para editá-lo, excluí-lo etc. Você pode tornar os níveis de acesso mais gerais, pois o compartilhamento em itens individuais pode ser configurado para ser mais específico.


Além disso, ter menos níveis de acesso pode facilitar a manutenção de um sistema sem desorganização e a implementação de uma estratégia, o que também pode levar a uma integração mais rápida quando as pessoas ingressam na empresa ou mudam de departamento.

</br>
</br>

**Prática recomendada**

Atribua pelo menos dois usuários ao nível global de acesso do administrador do sistema.

**Veja o porquê**

Mais de uma pessoa deve entender por que a Workfront foi configurada da maneira que estava, como gerenciá-la/mantê-la e como oferecer suporte aos usuários. Se uma pessoa estiver fora do escritório, sair da organização, estiver ocupada, etc., isso garante que haja outra pessoa que tenha as informações e os conhecimentos para gerenciar com sucesso o sistema.

</br>
</br>

**Prática recomendada**

Restrinja o que os usuários podem fazer com itens do Workfront por meio do compartilhamento, em vez de remover um recurso em um nível de acesso.


**Veja o porquê**

Os níveis de acesso controlam o que os usuários podem fazer com itens específicos em um nível global. As permissões de compartilhamento em cada projeto, tarefa, portfólio, documento etc. controlam o que um usuário individual pode fazer com esse item específico. Em vez de remover um recurso para todos com um nível de acesso específico, ajuste as permissões de compartilhamento em itens específicos para que os usuários tenham controles limitados.
