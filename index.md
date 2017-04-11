## Postagem 4: Modelo de Domínio Rico e Anêmico

Modelos Ricos e Anêmicos estão totalmente ligados ao Desenvimento Orientado a Objetos. Primeiramente, é preciso entender o conceito e a diferença entre eles.

Na Orientação a Objetos, quando a interação entre as classes do sistema não é clara o suficiente, existem diversos problemas como a repetição de código, dificuldade de manutenção e a propagação de bugs. Por conta disso, existe um conceito popular no desenvolvimento de software, que se chama Arquitetura em Camadas. Nela, a ideia é separar as regras de negócio, os atributos da entidade e o acesso aos dados. Isso é feito a fim de facilitar a manutenção do código, porém, quando implementada na prática essa arquitetura dá origem a regras de negócios repetidas e espalhadas. Por esse motivo, a Arquitetura em Camadas é hoje conhecida como Modelo Anêmico. Para ser mais preciso, a palavra *anêmico* significa a falta de alguma coisa. Sendo assim, o Modelo Anêmico é caracterizado como aquele em que as definições de estado e comportamento não ficam na mesma classe e por isso não representam o mundo real. 

Em contrapartida, o Modelo Rico utiliza a Orientação a Objetos e todos os seus conceitos. O modelo de classe deve possuir as classes que representam o mundo real, tendo estado e comportamento. Nesse modelo, é empregado o conceito de Desenvolvimento Orientado a Domínio ou *Domain Driven Design* e não mais o Design Orientado a Dados. Uma das principais vantagens é a facilidade de testes, já que cada classe é responsável por apenas o seu comportamento, o entendimento do domínio, já que representa o mundo real e a facilidade de manutenção. A principal característica do Modeo Rico é utilizar todos os benefícios que a orientação a objetos dá ao desenvolvedor: reutilização de código, polimorfismo, herança, etc.

O seguinte [podcast](http://podcast.dotnetarchitects.net/wp-content/uploads/2010/03/011-Modelo_anemico.mp3) traz uma discussão interessante sobre ambos os lados. Os defensores do Modelo Anêmico pregam que ele não é um antipadrão de projeto, pois consideram que antipadrões, na verdade, são nocivos sempre, o que não seria o caso. Eles enxergam que o maior ganho dessa arquitetura é a produtividade. Em contrapartida, os defensores do Modelo Rico também dizem que com este a produtividade também poderia existir, inclusive maior que no Modelo Anêmico. Além disso, ainda focam na ideia do desenvolvimento voltado a testes, já apresentada acima.

Como tudo nessa vida, a escolha entre qual o modelo será implementado depende de cada situação. Fazendo uma busca simples na internet dá para perceber que há uma certa resistência ao Anêmico, como pode ser visto [aqui](http://www.arquiteturajava.com.br/livro/cuidado-com-o-modelo-anemico.pdf). Entretanto, como abordado no podcast, o mercado atual se caracteriza por desenvolvedores que muitas vezes sabem a teoria da orientação a objetos, porém não colocam em prática, não conseguindo realmente aplicar o Modelo Rico.

Espero que você também tenha aprendido um pouco mais sobre os dois! Até a próxima!

________________________________________________________________________________________________________________________________________


## Postagem 1: Arquiteto de Software

Pelo que entendi do podcast e pesquisando um pouco na internet, não há uma definição clara sobre o papel do arquiteto de software, sendo um termo abrangente e que aceita uma certa variedade de papeis.

Ao tomarmos como base a ideia de que a arquitetura de software trata dos componentes do sistema, da interação entre eles, e das suas propriedades externas, fica claro que o arquiteto seria a figura responsável por trazer uma diretriz tecnológica, além de alinhar a escolha desses componentes ao negócio.

A partir daí surge a discussão de onde se encaixaria um arquiteto: no lado do desenvolvimento, ou apenas no âmbito mais tático e de direcionamento. Hierarquicamente o arquiteto estaria acima de um engenheiro de software sênior, mas uma das coisas que começou a virar tendência em alguns projetos, principalmente em start-ups, e também foi discutida no podcast é que a responsabilidade da a arquitetura está em toda a equipe.

Um arquiteto não é um profissional que será formado da noite pro dia e deve ser valorizado dentro de uma empresa, por se tratar de alguém que precisa estar em constante estudo, saber gerenciar relacionamentos, tomar decisões tecnológicas e intermediar o nível de negócio com o de desenvolvimento. É uma profissão que está cada vez mais em alta, como podemos ver nos links abaixo:

**1)** [Com média salarial acima de 10 mil, Arquiteto de TI é um dos profissionais desejados no Brasil](http://www.cbsi.net.br/2015/03/com-media-salarial-acima-de-10-mil.html)


**2)** [Média salarial para arquiteto de software](https://www.sine.com.br/media-salarial-para-arquiteto-de-software)
