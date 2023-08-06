# Documentação e Apresentação das Melhores Práticas de User Story

[Texto retirado e traduzido de awkale.me](http://awkale.me/user-story-best-practice/)

## Versão vs User Story vs Tarefa

O desenvolvimento ágil utiliza quatro métodos claros de entrega para trazer estrutura a qualquer projeto: **versões**, **sprints** e **user stories**.
  * Uma **versão** é um conjunto de recursos e correções lançados juntos como uma única atualização para o seu produto. Atribuir problemas a versões ajuda a planejar a ordem em que novos recursos (stories) para o seu produto serão lançados para os clientes. Uma versão pode ser composta de múltiplas sprints.
  * Uma **sprint** é um período de tempo específico durante o qual um trabalho específico deve ser concluído e preparado para revisão.
  * Uma **user story** (representada como um problema no Jira) captura uma descrição de um recurso do ponto de vista do usuário final. A user story descreve o tipo de usuário, o que eles querem e por quê. Uma user story ajuda a criar uma descrição simplificada de um requisito. As user stories são divididas em tarefas individuais que compõem a história (representadas como sub-tarefas no Jira).

## Por que usar user stories?
* Mantenha o foco na entrega de valor para o negócio.
* Evite introduzir detalhes muito cedo que possam impedir opções de design e prender os desenvolvedores em uma solução inadequada.
* Evite a aparência de completude e clareza falsas.
* Divida em partes pequenas o suficiente para permitir negociação e movimentação no backlog.
* Deixe as funções técnicas para o arquiteto, desenvolvedores, testadores e assim por diante.

## Criando uma user story
* O objetivo é delinear um valor específico para o cliente que uma equipe pode entregar em uma iteração usando algumas frases curtas, preferencialmente em linguagem não técnica. Enquanto os requisitos tradicionais (como casos de uso) tentam ser o mais detalhados possível, uma user story é definida incrementalmente, em três estágios:
  * A descrição breve da necessidade.
  * As conversas que ocorrem durante o refinamento do backlog e o planejamento da iteração para solidificar os detalhes.
  * Os testes que confirmam a conclusão satisfatória da história.

## O que torna uma ótima user story
  * Elas não entram em detalhes específicos.
  * As user stories devem ser escritas usando o seguinte modelo:
  > Como um [tipo de usuário], eu quero [meta] para que eu [receba benefício].
  > **Meta do usuário final:** _______________________________
  > **Meta do negócio final:** _____________________________
  > **Critérios de aceitação:**
    * O produto define quaisquer requisitos iniciais de funcionalidade que possam ser pensados.
    * Este é um esboço básico que será finalizado por meio de wireframes, fluxos e discussões.
    * Os critérios de aceitação devem ser finalizados antes do início do desenvolvimento.
  > **Medição do sucesso:** ___________________________
     * A medição do sucesso é a maneira pela qual provaremos que a história teve sucesso em atingir o usuário e a meta de negócios definidos acima. Isso inicialmente ficará em branco e será determinado por meio de conversas com pesquisa, experiência do usuário e produto. Isso deve ser finalizado antes do início do desenvolvimento.

## Exemplo de user story
  > Como um comprador no site, quero ter a capacidade de pagar com um cartão de crédito, para que eu possa confirmar imediatamente minha compra.
  > **Meta do usuário final:** Comprar itens com um cartão de crédito
  > **Meta do negócio final:** Aumentar as compras
  > **Critérios de aceitação:**
    * Aceitar Discover, Visa, MC
    * Validar o número do cartão de crédito
    * Validar a data de validade e o CVV
    * Validar o endereço de cobrança
    * Gerar mensagens de sucesso/falha após o processamento
  > **Medição do sucesso:** ___________________________

> "As histórias não são detalhadas até estarem prontas para serem desenvolvidas. Você só precisa entender o suficiente para permitir a priorização com outras histórias." - Kent Beck

* Uma user story bem elaborada seguirá o mnemônico INVEST.
  * I - Independente
    * As histórias são mais fáceis de trabalhar se forem independentes. Ou seja, elas não devem se sobrepor em conceito, e devemos ser capazes de agendar e implementá-las em qualquer ordem.
  * N - Negociável
    * Uma boa história é negociável. Não é um contrato explícito para recursos; em vez disso, os detalhes serão co-criados pelo cliente e pelo programador durante o desenvolvimento. Uma boa história captura a essência, não os detalhes. Com o tempo, o cartão pode adquirir anotações, ideias de teste e assim por diante, mas não precisamos dessas informações para priorizar ou agendar histórias.
  * V - Valioso
    * Uma história precisa ser valiosa. Não nos importamos com o valor para qualquer pessoa; precisa ser valiosa para o cliente. Os desenvolvedores podem ter preocupações (legítimas), mas elas devem ser apresentadas de forma que o cliente as perceba como importantes. Isso é especialmente importante ao dividir histórias.
    * Pense em uma história completa como um bolo de várias camadas, por exemplo, uma camada de rede, uma camada de persistência, uma camada lógica e uma camada de apresentação. Ao dividir uma história, estamos servindo apenas parte desse bolo. Queremos dar ao cliente a essência do bolo inteiro, e a melhor maneira é cortá-lo verticalmente através das camadas. Os desenvolvedores frequentemente têm a inclinação de trabalhar em apenas uma camada por vez (e acertá-la), mas uma camada completa do banco de dados (por exemplo) tem pouco valor para o cliente se não houver uma camada de apresentação.
  * E - Estimável
    *Uma boa história pode ser estimada. Não precisamos de uma estimativa exata, mas apenas o suficiente para ajudar o cliente a classificar e agendar a implementação da história. Ser estimável é em parte uma função de ser negociável, já que é difícil estimar uma história que não entendemos. É também uma função do tamanho: histórias maiores são mais difíceis de estimar.
    * Por fim, é uma função da equipe: o que é fácil de estimar pode variar dependendo da experiência da equipe. (Às vezes, a equipe pode ter que dividir uma história em um "spike" (limitado no tempo) que fornecerá informações suficientes para fazer uma estimativa decente e o restante da história que realmente implementará o recurso desejado.)
  * S - Pequena
    * Boas histórias tendem a ser pequenas. As histórias geralmente representam no máximo algumas semanas de trabalho para uma pessoa. (Algumas equipes as limitam a alguns dias de trabalho.) Acima desse tamanho, torna-se muito difícil saber o que está incluído no escopo da história. Dizer "levaria mais de um mês" frequentemente adiciona implicitamente "porque eu não entendo tudo o que estaria envolvido". Histórias menores tendem a ter estimativas mais precisas.
  * T - Testável
    * Uma boa história é testável. Escrever um cartão de história carrega uma promessa implícita: "Entendo o que quero o suficiente para poder escrever um teste para isso." Várias equipes relataram que, ao exigir testes do cliente antes de implementar uma história, a equipe é mais produtiva.
    * "Testabilidade" sempre foi uma característica de bons requisitos; escrever os testes cedo nos ajuda a saber se esse objetivo está sendo atendido. Se o cliente não souber como testar algo, isso pode indicar que a história não está clara o suficiente ou que não reflete algo valioso para eles, ou que o cliente precisa de ajuda no teste. A equipe pode tratar os requisitos não funcionais (como desempenho e usabilidade) como coisas que precisam ser testadas. Descobrir como operacionalizar esses testes ajudará a equipe a entender as verdadeiras necessidades.

## Esboço da user story
  * User Story
  * Meta do usuário final
  * Meta do negócio final
  * Critérios de Aceitação (isso não é finalizado até que a história esteja pronta para o desenvolvimento)
  * Medição do Sucesso (isso é adicionado após conversas com o produto, experiência do usuário e pesquisa)

## O que fazer e o que não fazer criando user stories
* FAÇA foco em um usuário específico
  * Evite o papel genérico de "Usuário" ao escrever user stories. As user stories se referem a todos os papéis que interagem com o sistema ou que percebem algum valor ou benefício do sistema.
* FAÇA fornecer critérios de aceitação
  * O proprietário do produto deve listar o máximo de critérios de aceitação possível para esclarecer a intenção da história. Os critérios de aceitação se tornarão casos de teste de garantia de qualidade.
* FAÇA ter conversas
  * Atualize os critérios de aceitação e os detalhes da user story com base em suas conversas.
* NÃO entre em detalhes específicos
* NÃO forneça a solução
  * As user stories devem se concentrar na necessidade e no benefício do usuário, não na solução.