## Postagem 6: Padrões GRASP

Logo após a programação estruturada, a próxima transformação de grande impacto na área de software foi o surgimento do conjunto de princípios conhecidos como Orientação a Objetos. Dentre os fatores que contribuíram para popularizar as linguagens baseadas em OO, um trabalho importante foi a documentação feita por diversos especialistas de software de soluções que ficaram conhecidas como padrões de projetos. Uma das mais famosas foi a publicação de 23 patterns, em 1994, aos quais se convencionou chamar de GoF, sigla em inglês para *Gang of Four*.

Além deles, vários outros patterns foram desenvolvidos ao longo do tempo. Um exemplo disto são os padrões SOLID, um acrônimo onde cada letra representa um princípio de design de orientação a objetos. De forma análoga, existe também os padrões GRASP, os quais contemplam um conjunto de princípios baseados na noção de responsabilidade e que podem servir de guia no desenvolvimento de soluções OO. Este post aborda um pouco sobre o GRASP, utilizando os conhecimentos das aulas do professor Luiz Borba, postadas [aqui](https://www.youtube.com/watch?v=IdQjsAcgtNM).

Para começo de conversa, a sigla GRASP significa *General Responsability Assignment Software Patterns* ou Padrões Gerais para Atribuição de Responsabilidade. Consiste em diretrizes para atribuir responsabilidade a classes e objetos em um projeto OO. Mas antes de entendermos a definição, devemos entender o real significado da palavra responsabilidade. Neste contexto, a responsabilidade é definida como as obrigações que um objeto possui quando se leva em conta o seu papel dentro de um determinado contexto. Para definir a responsabilidade de um objeto, então, leva-se em conta o que este elemento irá "fazer" e/ou "saber". 

Ao todo, são nove os padrões GRASP, resumidos na tabela a seguir:

| **Padrão** | **Descrição** |
|--------|-----------|
|*Information Expert*| Onde delegar responsabilidades?|
| *Creator*| Quem deve ser o responsável por criar uma nova instância da classe? |
|*Low Coupling*| Quão fortemente um elemento está conectado? Como reduzir o impacto de mudanças?|
|*High Cohesion*| Como obter os objetos focados, fáceis de entender, gerenciáveis e ainda pouco acopláveis?|
|*Controller*| Quem deve responder aos eventos do sistema?|
|*Polymorphism*| Como criar componentes de softwares conectáveis com base no tipo?|
|*Pure Fabrication*|Que objeto deve ter a responsabilidade quando você não quer violar *High Cohesion* e *Low Coupling*, mas as soluções oferecidas pelo *Information Expert* não são apropriadas?|
|*Indirection*|Onde colocar uma responsabilidade de modo a evitar o acoplamento direto entre duas ou mais classes? Como desacoplar objetos de modo a possibilitar o baixo acoplamento e manter alta a possibilidade de reuso?|
|*Protected Variations*| Como projetar objetos, subsistema e sistemas para que as variações ou instabilidades nesses elementos não tenha um impacto indesejável nos outros elementos?|

<br/>
O GRASP possui inúmeros benefícios, como a reutilização de componentes, utilização de todos os eventos em uma única classe, facilidade de manutenção e uma melhor distribuição de responsabilidades. O post foca mais na parte teórica, mas recomenda-se fortemente assistir aos vídeos para saber um pouco mais sobre a prática e a implementação de cada um dos padrões GRASP!

Espero que você tenha compreendido um pouco mais sobre os padrões. Até a próxima!


________________________________________________________________________________________________________________________________________


## Postagem 4: Modelo de Domínio Rico e Anêmico

Modelos Ricos e Anêmicos estão totalmente ligados ao Desenvimento Orientado a Objetos. Primeiramente, é preciso entender o conceito e a diferença entre eles.

Na Orientação a Objetos, quando a interação entre as classes do sistema não é clara o suficiente, existem diversos problemas como a repetição de código, dificuldade de manutenção e a propagação de bugs. Por conta disso, existe um conceito popular no desenvolvimento de software, que se chama Arquitetura em Camadas. Nela, a ideia é separar as regras de negócio, os atributos da entidade e o acesso aos dados. Isso é feito a fim de facilitar a manutenção do código, porém, quando implementada na prática essa arquitetura dá origem a regras de negócios repetidas e espalhadas. Por esse motivo, a Arquitetura em Camadas é hoje conhecida como Modelo Anêmico. Para ser mais preciso, a palavra *anêmico* significa a falta de alguma coisa. Sendo assim, o Modelo Anêmico é caracterizado como aquele em que as definições de estado e comportamento não ficam na mesma classe e por isso não representam o mundo real. 

Em contrapartida, o Modelo Rico utiliza a Orientação a Objetos e todos os seus conceitos. O modelo de classe deve possuir as classes que representam o mundo real, tendo estado e comportamento. Nesse modelo, é empregado o conceito de Desenvolvimento Orientado a Domínio ou *Domain Driven Design* e não mais o Design Orientado a Dados. Uma das principais vantagens é a facilidade de testes, já que cada classe é responsável por apenas o seu comportamento, o entendimento do domínio, já que representa o mundo real e a facilidade de manutenção. A principal característica do Modeo Rico é utilizar todos os benefícios que a orientação a objetos dá ao desenvolvedor: reutilização de código, polimorfismo, herança, etc.

O seguinte [podcast](http://podcast.dotnetarchitects.net/wp-content/uploads/2010/03/011-Modelo_anemico.mp3) traz uma discussão interessante sobre ambos os lados. Os defensores do Modelo Anêmico pregam que ele não é um antipadrão de projeto, pois consideram que antipadrões, na verdade, são nocivos sempre, o que não seria o caso. Eles enxergam que o maior ganho dessa arquitetura é a produtividade. Em contrapartida, os defensores do Modelo Rico também dizem que com este a produtividade também poderia existir, inclusive maior que no Modelo Anêmico. Além disso, ainda focam na ideia do desenvolvimento voltado a testes, já apresentada acima.

Como tudo nessa vida, a escolha entre qual o modelo será implementado depende de cada situação. Fazendo uma busca simples na internet dá para perceber que há uma certa resistência ao Anêmico, como pode ser visto [aqui](http://www.arquiteturajava.com.br/livro/cuidado-com-o-modelo-anemico.pdf). Entretanto, como abordado no podcast, o mercado atual se caracteriza por desenvolvedores que muitas vezes sabem a teoria da orientação a objetos, porém não colocam em prática, não conseguindo realmente aplicar o Modelo Rico.

Espero que você também tenha aprendido um pouco mais sobre os dois! Até a próxima!

________________________________________________________________________________________________________________________________________


## Postagem 3: Arquitetura de Software

Existem diversas abordagens distintas de Arquitetura de Software. Como comentado um pouco na postagem 1, uma dessas definições é a de que a Arquitetura de Software trata dos componentes do sistema e como eles se interagem. Ela desempenha um papel fundamental para gerenciar a complexidade inerente ao software a ser criado. Uma boa arquitetura possibilita que um sistema satisfaça às exigências principais de um projeto, tais como: desempenho, confiabilidade, portabilidade, manutenibilidade, interoperabilidade e etc. O seguinte [podcast](http://www.grokpodcast.com/2012/01/12/episodio-56-arquitetura-e-design-de-software-parte-1-de-4/) resume a arquitetura como uma maneira de visualizar a implementação do código.

Tendo essas definição em mente, um estilo arquitetural de software pode ser visto como um padrão que oferece um framework abstrato para uma família de sistemas. Dessa forma, ele melhora o particionamento e promove reuso de design, fornecendo soluções para problemas recorrentes. A tabela abaixo oferece diversos estilos arquiteturais utilizados:


| **Estilo de Arquitetura** | **Descrição** |
| --- | --- |
| Client-Server	| Segrega o sistema em duas aplicações, em que o cliente faz uma requisição de serviço ao servidor.
Arquitetura baseada em Componentes | O design de aplicação é decomposto em componentes lógicos e funcionais que são independentes de local e expõe interfaces de comunicação bem definidas.|
Arquitetura em Camadas | Separa as respnsabilidades da aplicação em grupos bem definidos (camadas).|
Message-Bus |	Um sistema de software que pode receber e enviar mensagens baseado em um conjunto de formatos conhecidos, de forma que sistemas possam se comunicar uns com os outros sem necessidade de conhecer o destinatário atual.|
Orientado a Objetos	| Um estilo arquitetural baseado na divisão de tarefas para uma aplicação ou sistema em reutilização individual e objetos autossuficientes, cada um contendo os dados e comportamentos relevantes ao objeto.|
Apresentação Separada |	Separa a lógica para gerenciar a interação do usuário da visualização da interface de usuário (UI) e dos dados com os quais o usuário trabalha.|


<br/>
Além dessas, existe uma outra discutida também no podcast: Service-Oriented Architecture (SOA). É uma arquitetura orientada a serviços, como o nome já diz e baseia-se nos princípios da computação distribuída, utilizando serviços web para estabelecer a comunicação entre os sistemas clientes e os sistemas que implementam os serviços. Para saber mais sobre ela, acesse o [link](http://www.grokpodcast.com/2012/02/02/episodio-59-arquitetura-e-design-de-software-parte-4-de-4/) :)


________________________________________________________________________________________________________________________________________


## Postagem 1: Arquiteto de Software

Pelo que entendi do podcast e pesquisando um pouco na internet, não há uma definição clara sobre o papel do arquiteto de software, sendo um termo abrangente e que aceita uma certa variedade de papeis.

Ao tomarmos como base a ideia de que a arquitetura de software trata dos componentes do sistema, da interação entre eles, e das suas propriedades externas, fica claro que o arquiteto seria a figura responsável por trazer uma diretriz tecnológica, além de alinhar a escolha desses componentes ao negócio.

A partir daí surge a discussão de onde se encaixaria um arquiteto: no lado do desenvolvimento, ou apenas no âmbito mais tático e de direcionamento. Hierarquicamente o arquiteto estaria acima de um engenheiro de software sênior, mas uma das coisas que começou a virar tendência em alguns projetos, principalmente em start-ups, e também foi discutida no podcast é que a responsabilidade da a arquitetura está em toda a equipe.

Um arquiteto não é um profissional que será formado da noite pro dia e deve ser valorizado dentro de uma empresa, por se tratar de alguém que precisa estar em constante estudo, saber gerenciar relacionamentos, tomar decisões tecnológicas e intermediar o nível de negócio com o de desenvolvimento. É uma profissão que está cada vez mais em alta, como podemos ver nos links abaixo:

**1)** [Com média salarial acima de 10 mil, Arquiteto de TI é um dos profissionais desejados no Brasil](http://www.cbsi.net.br/2015/03/com-media-salarial-acima-de-10-mil.html)


**2)** [Média salarial para arquiteto de software](https://www.sine.com.br/media-salarial-para-arquiteto-de-software)
