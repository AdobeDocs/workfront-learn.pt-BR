---
title: Prática recomendada - Licenças e níveis de acesso
description: Explore as recomendações de práticas recomendadas dos especialistas da Adobe Workfront sobre a configuração, o gerenciamento e o uso das licenças e dos níveis de acesso da Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 0%

---

# Prática recomendada - Licenças e níveis de acesso

## O que é uma &quot;prática recomendada&quot; do Adobe Workfront?

As práticas recomendadas são diretrizes que representam um curso de ação eficaz e eficiente; são facilmente adotadas por você e pelos usuários em sua empresa; e podem ser replicadas com sucesso em toda a organização.

Ao revisar essas recomendações, lembre-se de que algumas práticas recomendadas do Workfront são universais, enquanto outras podem ser mais específicas ao tópico. Use essas práticas recomendadas como uma estrutura para ajudar a orientar as configurações e o uso do sistema Workfront.

## Navegando nesta página

Ao percorrer essa página, primeiro você encontrará uma lista de alto nível de todas as práticas recomendadas para o tópico. Isso permite analisar as recomendações sem mergulhar nos detalhes do &quot;por quê&quot;.

O &quot;Por que essas práticas recomendadas?&quot; A área, localizada após a lista de alto nível, fornece mais detalhes sobre algumas das práticas recomendadas e por que elas são consideradas um processo, ferramenta, etc. Você deve considerar a implementação com sua instância do Workfront.

</br>
</br>

## Práticas recomendadas para licenças e níveis de acesso

* Comece com menos acesso para usuários ao configurar níveis de acesso.

* Ao atribuir licenças de Revisão e Solicitação, normalmente o padrão é Revisar, pois fornece ao usuário mais permissões no Adobe Workfront.

* Desmarque a caixa de seleção &quot;Compartilhar em todo o sistema&quot; em cada objeto em todos os níveis de acesso, a menos que você deseje especificamente que esses usuários possam fazer isso.

* Considere ativar a configuração &quot;Nunca permitir que os usuários excluam comentários&quot; em Definir restrições adicionais em um nível de acesso.

* Limitar o número de administradores do sistema a favor de administradores de grupo.

* Copie um nível de acesso existente e faça modificações, em vez de criar um novo nível do zero.

* Documente o que cada nível de acesso pode fazer na caixa Descrição.

* Limite-se apenas aos níveis de acesso necessários para atingir suas metas de trabalho, idealmente quatro ou cinco, que atendam às necessidades da maioria dos usuários do sistema.

* Atribua pelo menos dois usuários ao nível de acesso de administrador de sistema global.

* Restrinja o que os usuários podem fazer com itens do Workfront por meio do compartilhamento, em vez de remover um recurso em um nível de acesso.

</br>
</br>


## Por que essas práticas recomendadas?

**Prática recomendada**

Comece com menos acesso para usuários ao configurar níveis de acesso.



**Veja o porquê**

Inicie os usuários com o acesso mínimo de que precisarão para fazer seu trabalho. Se não puderem realizar suas tarefas devido a direitos de acesso insuficientes, geralmente solicitarão acesso adicional. Conceder aos usuários acesso excessivo imediatamente pode levar a problemas de segurança. Além disso, é sempre melhor fornecer aos usuários mais acesso do que remover o acesso.

</br>
</br>



**Prática recomendada**

Ao atribuir licenças de Revisão e Solicitação, normalmente o padrão é Revisar, pois fornece ao usuário mais permissões no Adobe Workfront.



**Veja o porquê**

Embora as licenças de Revisão e Solicitação possam ser atribuídas a um número ilimitado de usuários no Workfront, as licenças de Solicitação estão limitadas apenas a fazer e atualizar solicitações. Uma licença de revisão tem mais acesso a projetos e tarefas do que uma licença de solicitação, bem como a possibilidade de visualizar portfólios e programas, editar documentos e acessar ferramentas de gerenciamento de recursos.

</br>
</br>

**Prática recomendada**

Desmarque a caixa de seleção &quot;Compartilhar em todo o sistema&quot; em cada objeto em todos os níveis de acesso, a menos que haja um motivo específico para que os usuários precisem compartilhar em todo o sistema.



**Veja o porquê**

O compartilhamento de um objeto em todo o sistema geralmente é usado como uma muleta para permitir que determinados usuários vejam itens no Workfront. Isso acontece quando a estrutura do grupo Workfront está ausente ou quando as permissões de compartilhamento não são totalmente compreendidas. Quando os itens são compartilhados em todo o sistema, significa que todos podem ver o item compartilhado. Dependendo do tipo de informação que está sendo mantida no sistema, isso pode levar a problemas de privacidade.



Por exemplo, você pode estar trabalhando com vários fornecedores dentro do Workfront para verificar o progresso, fornecer aprovações etc. Se a caixa de seleção &quot;Compartilhar em todo o sistema&quot; for uma opção, ela poderá ser selecionada ou definida como padrão, disponibilizando informações para todos os fornecedores.



Ao desmarcar a opção completamente, você a torna um usuário, com permissão para compartilhar, deve determinar a pessoa ou pessoas específicas - por meio de uma empresa, grupo ou equipe - com as quais deseja compartilhar o objeto.

</br>
</br>

**Prática recomendada**

Considere ativar a configuração &quot;Nunca permitir que os usuários excluam comentários&quot; em Definir restrições adicionais em um nível de acesso.



**Veja o porquê**

Ativar essa opção garante que as comunicações anteriores não sejam removidas do Workfront. Algumas organizações exigem que o histórico completo de comentários seja mantido para fins de auditoria.

</br>
</br>

**Prática recomendada**

Limitar o número de administradores do sistema a favor de administradores de grupo.



**Veja o porquê**

Os administradores do sistema têm acesso a tudo no Workfront, incluindo configurações globais do sistema. As configurações que os administradores de grupos podem acessar são controladas pelo administrador do sistema e se aplicam somente a esse grupo específico.



Ter administradores de grupo permite que os administradores do sistema deleguem muitas responsabilidades, permitindo que eles se concentrem em itens de imagem maiores, em vez da manutenção diária do Workfront. Os administradores de grupo podem manter-se em contato com as necessidades de seus grupos com mais facilidade, o que oferece um melhor serviço aos usuários.

</br>
</br>


**Prática recomendada**

Copie um nível de acesso existente e faça modificações, em vez de criar um novo nível do zero.



**Veja o porquê**

A cópia de um nível de acesso existente fornece uma base consistente para novos níveis de acesso, garantindo que as configurações iniciais sejam idênticas. Isso também economiza tempo, pois os administradores do sistema não precisarão configurar um nível de acesso totalmente do zero.

</br>
</br>

**Prática recomendada**

Documente o que cada nível de acesso pode fazer na caixa Descrição.



**Veja o porquê**

Seja detalhado com a descrição, listando quais são as configurações para cada tipo de objeto. Isso ajuda os administradores de sistemas, presentes e futuros, a saber exatamente o que cada nível de acesso faz sem precisar mergulhar no próprio nível de acesso para analisar as configurações.



Isso também pode facilitar a comparação dos níveis de acesso ao analisá-los em um relatório. O campo de descrição pode ser adicionado rapidamente à visualização para ver rapidamente como eles diferem e, possivelmente, por que um nível de acesso diferente foi criado.

</br>
</br>

**Prática recomendada**

Limite-se apenas aos níveis de acesso necessários para atingir suas metas de trabalho, idealmente quatro ou cinco, que atendam às necessidades da maioria dos usuários do sistema.


**Veja o porquê**

O nível de acesso garante que, quando um objeto do Workfront for compartilhado com um usuário, ele tenha os direitos necessários para editá-lo, excluí-lo etc. Você pode tornar os níveis de acesso mais gerais, pois o compartilhamento em itens individuais pode ser configurado para ser mais específico.


Além disso, ter menos níveis de acesso pode facilitar a manutenção de um sistema organizado e a implementação de uma estratégia, o que também pode resultar em uma integração mais rápida quando as pessoas ingressam na empresa ou trocam de departamento.

</br>
</br>

**Prática recomendada**

Atribua pelo menos dois usuários ao nível de acesso de administrador de sistema global.

**Veja o porquê**

Mais de uma pessoa deve entender por que o Workfront foi configurado da maneira como era, como gerenciá-lo/mantê-lo e como oferecer suporte aos usuários. Se uma pessoa estiver fora do escritório, sair da organização, estiver ocupada, etc., isso garante que haja outra pessoa com as informações e o conhecimento necessários para gerenciar o sistema com êxito.

</br>
</br>

**Prática recomendada**

Restrinja o que os usuários podem fazer com itens do Workfront por meio do compartilhamento, em vez de remover um recurso em um nível de acesso.


**Veja o porquê**

Os níveis de acesso controlam o que os usuários podem fazer com itens específicos em nível global. As permissões de compartilhamento em cada projeto, tarefa, portfólio, documento, etc. controlam o que um usuário individual pode fazer com esse item específico. Em vez de remover um recurso para todos com um nível de acesso específico, ajuste as permissões de compartilhamento em itens específicos para que os usuários tenham controles limitados.
