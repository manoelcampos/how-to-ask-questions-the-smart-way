# Como Fazer Perguntas de Forma Inteligente

Tradução baseada na [revisão 3.10 da versão original em inglês, de 21 de maio de 2014](http://www.catb.org/~esr/faqs/smart-questions.html). 
Um fork da versão original em inglês pode ser encontrado [aqui](README.en.md).

- Eric Steven Raymond
	- [Thyrsus Enterprises](http://www.catb.org/~esr/)
	- <esr@thyrsus.com>
    
- Rick Moen
	- <respond-auto@linuxmafia.com>

[Copyright © 2001,2006,2014 Eric S. Raymond, Rick Moen](COPYRIGHT.md)

# Sumário

- [Aviso Legal](#1)
- [Introdução](#2)
- [Antes de perguntar](#3)
- [Quando você perguntar](#4)
	- [Escolha seu fórum cuidadosamente](#4.1)
	- [Stack Overflow](#4.2)
	- [Fóruns Web e IRC](#4.3)
	- [Como um segundo passo, use listas de e-mail de projeto](#4.4)
	- [Use linhas de assunto significativas e específicas](#4.5) 
	- [Facilite a resposta](#4.6)
	- [Escreva com clareza e correção gramatical e ortográfica](#4.7) 
	- [Envie perguntas em formatos acessíveis e padronizados](#4.8)
	- [Seja preciso e informativo sobre o seu problema](#4.9)
	- [Volume não é precisão](#4.10)
	- [Não se apresse em declarar que você encontrou um bug](#4.11)
	- [Bajulação não substitui o seu dever de casa](#4.12)
	- [Descreva os sintomas do problema, não suas suposições](#4.13)
	- [Descreva os sintomas do seu problema em ordem cronológica](#4.14)
	- [Descreva o objetivo, não o passo](#4.15)
	- [Não peça respostas por e-mail privado](#4.16)
	- [Seja explícito sobre a sua pergunta](#4.17)
	- [Ao perguntar sobre código](#4.18)
	- [Não poste perguntas de dever de casa](#4.19)
	- [Elimine perguntas vazias](#4.20)
	- [Não marque sua pergunta como “Urgente”, mesmo que seja urgente para você](#4.21)
	- [Educação nunca fez mal, e às vezes ajuda](#4.22)
	- [Faça um breve acompanhamento sobre a solução](#4.23)
- [Como interpretar respostas](#5)
	- [RTFM e STFW: Como saber que você pisou feio na bola](#5.1)
	- [Se você não entendeu...](#5.2)
	- [Como lidar com grosseria](#5.3)
- [Não reaja como um perdedor](#6)
- [Perguntas que não devem ser feitas](#7)
- [Perguntas boas e ruins](#8)
- [Se você não consegue obter uma resposta](#9)
- [Como responder perguntas de uma forma útil](#10)
- [Recursos relacionados](#11)
- [Agradecimentos](#12)

<a name="1"></a>

# Aviso Legal

Muitos sites de projetos incluem links para este documento em suas seções de ajuda. Isso é ótimo, é o uso que pretendemos — mas se você é um webmaster criando esse link para a página do seu projeto, por favor exiba, junto ao link, um aviso bem visível de que não somos o help desk do seu projeto!

Aprendemos da maneira difícil que, sem esse aviso, somos importunados repetidamente por idiotas que acham que, só porque publicamos este documento, é nosso trabalho resolver todos os problemas técnicos do mundo.

Se você está lendo este documento porque precisa de ajuda e tem a impressão de que vai obtê-la diretamente dos autores, você é um dos idiotas de quem estamos falando.

Não nos faça perguntas. Vamos simplesmente ignorar você. Estamos aqui para mostrar como obter ajuda de pessoas que de fato conhecem o software ou hardware com o qual você está lidando, e em 99,9% das vezes não somos nós. A menos que você tenha certeza de que um dos autores deste documento é especialista no assunto, deixe-nos em paz e todos ficarão felizes.

<a name="2"></a>

# Introdução

No mundo dos [hackers](http://www.catb.org/~esr/faqs/hacker-howto.html), o tipo de resposta que você recebe para suas perguntas técnicas depende tanto da forma como você pergunta quanto da dificuldade de elaborar a resposta. Este guia vai ensinar você a fazer perguntas de um jeito que aumente as chances de obter uma resposta satisfatória.

Agora que o software de código aberto (open source) se difundiu, você muitas vezes consegue respostas tão boas de usuários experientes quanto de hackers. Isso é uma Coisa Boa; usuários tendem a ser um pouco mais tolerantes com o tipo de erro que iniciantes costumam cometer. Ainda assim, tratar usuários experientes como hackers, do modo que recomendamos aqui, geralmente também é eficaz para obter respostas úteis deles.

A primeira coisa a entender é que hackers adoram problemas difíceis e perguntas boas e instigantes sobre eles. Se não adorássemos, não estaríamos aqui. Se você nos oferece uma questão interessante para mastigar, seremos gratos; boas perguntas são um estímulo e uma dádiva. Elas nos ajudam a aprofundar nosso entendimento e frequentemente revelam problemas que talvez não tivéssemos notado ou considerado de outra maneira. Entre hackers, "Boa pergunta!" é um elogio forte e sincero.

Apesar disso, hackers têm a reputação de responder perguntas simples de um jeito que parece hostil e arrogante. Às vezes parece que somos rudes automaticamente com iniciantes e ignorantes. Mas isso não é bem verdade.

O que somos, sem pedir desculpas, é hostis com quem parece não querer pensar nem fazer o próprio dever de casa antes de perguntar. Pessoas assim são sugadoras de tempo: tomam sem dar nada em troca e desperdiçam tempo que poderíamos gastar com perguntas mais interessantes ou com alguém mais merecedor de uma resposta. Chamamos essas pessoas de "losers" (perdedores) (e, por razões históricas, às vezes escrevemos "lusers").

Sabemos que muitas pessoas só querem usar o software que desenvolvemos e não têm nenhum interesse em aprender detalhes técnicos. Para elas, o computador é apenas uma ferramenta, um meio para atingir um fim; elas têm coisas mais importantes a fazer e vidas para viver. Reconhecemos isso e não esperamos que todo mundo se interesse pelas questões técnicas que nos fascinam. No entanto, nosso estilo de responder perguntas é voltado a quem tem esse interesse e quer participar ativamente da solução dos problemas. Isso não vai mudar. Nem deveria; se mudasse, poderíamos nos tornar menos eficazes naquilo que fazemos de melhor.

Somos (em sua maioria) voluntários. Tiramos tempo de nossas vidas ocupadas para responder perguntas e, às vezes, ficamos sobrecarregados com elas. Por isso, aplicamos um filtro impiedoso. Em particular, descartamos perguntas de quem parece ser perdedor, para gastar nosso tempo de forma mais eficiente com os vencedores.

Se você acha essa atitude antipática, condescendente ou arrogante, reveja suas suposições. Não estamos pedindo que você se ajoelhe diante de nós; na verdade, a maioria de nós adoraria tratar você como um igual e recebê-lo em nossa cultura, se você fizer o esforço necessário para isso. Mas simplesmente não é eficiente tentar ajudar quem não ajuda a si mesmo. Não há problema em ser ignorante; o que não vale é bancar o estúpido.

Então, embora não seja preciso ser tecnicamente competente para chamar nossa atenção, é preciso demonstrar o tipo de atitude que leva à competência: estar alerta, ser reflexivo e observador, e querer ser um parceiro ativo na construção de uma solução. Se você não consegue conviver com esse tipo de discriminação, sugerimos que contrate um suporte comercial em vez de pedir a hackers que lhe doem ajuda pessoalmente.

Se você decidir recorrer a nós, não quer ser um dos perdedores. Não quer nem parecer um. A melhor forma de obter uma resposta rápida e adequada é perguntar como uma pessoa inteligente, confiante e com alguma noção do assunto, que só precisa de ajuda em um ponto específico.

(Melhorias para este guia são bem-vindas. Você pode enviar sugestões para <esr@thyrsus.com> ou <respond-auto@linuxmafia.com>. Note, porém, que este documento não pretende ser um guia geral de [netiqueta](http://www.ietf.org/rfc/rfc1855.txt), e geralmente rejeitaremos sugestões que não estejam especificamente relacionadas a obter respostas úteis em um fórum técnico.)

<a name="3"></a>

# Antes de perguntar

Antes de fazer uma pergunta técnica por e-mail, em um grupo de discussão ou em um site de chat, faça o seguinte:

- Tente encontrar a resposta pesquisando no arquivo do fórum ou da lista de e-mail em que você pretende postar a pergunta.
- Tente encontrar a resposta pesquisando na Web.
- Tente encontrar a resposta lendo o manual do produto com o qual você está tendo problemas.
- Tente encontrar a resposta lendo as FAQs (Frequently Asked Questions - Perguntas Frequentes).
- Tente encontrar a resposta inspecionando e experimentando.
- Tente encontrar a resposta perguntando a um amigo experiente.

Se você é programador, tente encontrar a resposta lendo o código-fonte.

Quando fizer sua pergunta, mostre que você de fato tentou essas opções antes; isso ajuda a deixar claro que você não é um aproveitador preguiçoso desperdiçando o tempo dos outros. Melhor ainda, mostre o que aprendeu com essas tentativas. Gostamos de responder perguntas de quem demonstra ser capaz de aprender com as respostas.

Use táticas como pesquisar no Google o texto da mensagem de erro que você está recebendo (pesquise tanto no [Google Groups](http://groups.google.com) quanto em páginas Web). Isso pode levar você direto à documentação da correção ou a uma thread de lista de e-mail com a resposta para a sua dúvida. Mesmo que não leve, dizer "Pesquisei no Google a seguinte frase, mas não encontrei nada promissor" é uma boa prática ao pedir ajuda por e-mail ou em grupos, nem que seja para registrar quais buscas não ajudam. Isso também ajuda a direcionar outras pessoas com problemas parecidos para a sua thread, desde que você inclua o link da busca com os termos que, com sorte, levarão à thread com o seu problema e a possível solução.

Tome o tempo que precisar. Não espere resolver um problema complicado com alguns segundos de busca no Google. Leia e entenda as FAQs, sente-se, relaxe e reflita sobre o problema antes de recorrer a especialistas. Acredite, eles conseguem perceber, pelas suas perguntas, o quanto você leu e pensou, e ficam mais dispostos a ajudar quando você chega preparado. Não saia disparando todo o seu arsenal de perguntas só porque a primeira busca não deu resposta (ou deu respostas demais).

Prepare sua pergunta. Pense bem nela. Perguntas com cara de afobadas recebem respostas afobadas, ou nenhuma. Quanto mais você demonstrar que pensou e se esforçou para resolver o problema antes de pedir ajuda, maiores as chances de realmente receber ajuda.

Cuidado para não fazer a pergunta errada. Se a sua pergunta se baseia em suposições equivocadas, é bem provável que um [hacker qualquer](https://en.wikipedia.org/wiki/J._Random_Hacker) responda de forma literal e inútil, pensando "Que pergunta idiota...", na esperança de que a experiência de receber o que você pediu, e não o que você precisava, lhe sirva de lição.

Nunca presuma que você tem direito a uma resposta. Não tem; afinal, você não está pagando pelo serviço. Você vai conquistar uma resposta, se conquistar, fazendo uma pergunta substancial, interessante e instigante, que contribua implicitamente para a experiência da comunidade em vez de apenas exigir passivamente o conhecimento dos outros.

Por outro lado, deixar claro que você é capaz e está disposto a ajudar a desenvolver a solução é um bom começo. Perguntas como "Alguém poderia me dar uma pista?", "O que está faltando no meu exemplo?" e "Que site eu deveria ter consultado?" têm mais chances de obter resposta do que "Por favor, poste o procedimento exato que devo seguir.", porque deixam claro que você realmente quer fazer o trabalho e só precisa que alguém aponte a direção certa.

<a name="4"></a>

# Quando você perguntar

<a name="4.1"></a>

## Escolha seu fórum cuidadosamente

Tenha cuidado ao escolher onde fazer sua pergunta. Você provavelmente será ignorado, ou rotulado como perdedor, se você:

- postar sua pergunta em um fórum onde ela foge do assunto
- postar uma pergunta muito elementar em um fórum onde se esperam questões técnicas avançadas, ou vice-versa
- espalhar a mesma pergunta por vários fóruns diferentes
- enviar um e-mail pessoal a alguém que não é seu conhecido nem responsável direto por resolver o seu problema

Hackers descartam perguntas direcionadas ao lugar errado para proteger seus canais de comunicação de serem afogados em irrelevância. Você não quer que isso aconteça com você.

O primeiro passo, portanto, é encontrar o fórum certo. Mais uma vez, [o Google e outros mecanismos de busca são seus amigos](http://www.giyf.com). Use-os para achar o site do projeto mais diretamente ligado ao hardware ou software com o qual você está tendo dificuldade. Normalmente o site terá links para as FAQs, para a lista de e-mail do projeto e para os arquivos dela. Essas listas são o último recurso na busca por ajuda, caso seus próprios esforços (incluindo a leitura das FAQs que você encontrou) não tenham bastado. O site do projeto também pode descrever como relatar erros (bugs), ou ter um link para essa documentação; se tiver, siga o procedimento.

Disparar um e-mail para uma pessoa ou fórum com o qual você não tem familiaridade é arriscado, para dizer o mínimo. Por exemplo, não presuma que o autor de uma página informativa quer ser seu consultor gratuito. Não faça suposições otimistas sobre sua pergunta ser bem-vinda; se você não tem certeza, poste em outro lugar ou nem poste.

Ao escolher um fórum Web, newsgroup ou lista de e-mail, não confie apenas no nome do grupo; procure uma FAQ ou uma descrição para verificar se a sua pergunta se encaixa nos assuntos do grupo. Leia algumas mensagens anteriores antes de postar, para sentir como as coisas funcionam por lá. Aliás, antes de postar, é uma excelente ideia pesquisar no arquivo do fórum, newsgroup ou lista de e-mail por palavras-chave relacionadas ao seu problema. Você pode encontrar a resposta e, se não encontrar, isso ajudará a formular melhor a pergunta.

Não saia atirando para todo lado, em todos os canais de ajuda disponíveis de uma só vez; isso é como gritar e irrita as pessoas. Vá por eles com calma, um de cada vez.

Saiba qual é o seu assunto! Um dos erros clássicos é perguntar sobre interfaces de programação do Unix ou do Windows em um fórum dedicado a uma linguagem, biblioteca ou ferramenta portável para ambos os sistemas. Se você não entende por que isso é uma gafe, é melhor não perguntar nada até entender.

Em geral, perguntas postadas em um fórum público bem escolhido têm mais chances de obter respostas úteis do que perguntas equivalentes em um fórum privado. Há várias razões para isso. Uma é simplesmente o número de possíveis respondentes. Outra é o tamanho da audiência: hackers tendem a responder mais perguntas que ajudam muita gente do que perguntas que servem a poucos.

É compreensível que hackers habilidosos e autores de softwares populares já recebam mensagens mal direcionadas além da conta. Contribuir para essa enxurrada pode, em casos extremos, ser a gota d'água; às vezes, contribuidores de projetos populares deixaram de oferecer suporte por causa do dano colateral insuportável de tanto e-mail inútil em suas contas pessoais.

<a name="4.2"></a>

## [Stack Overflow](http://stackoverflow.com)

Pesquise primeiro, depois pergunte no Stack Exchange.

Nos últimos anos, a rede de sites Stack Exchange surgiu como o maior recurso para responder perguntas técnicas (e não só técnicas), e é até o fórum preferido de muitos projetos de código aberto.

Comece com uma busca no Google antes de pesquisar no Stack Exchange; o Google indexa o site em tempo real. Há uma boa chance de alguém já ter feito uma pergunta parecida, e os sites do Stack Exchange costumam aparecer perto do topo dos resultados. Se você não encontrou nada pelo Google, pesquise de novo no site do Stack Exchange mais relevante para a sua pergunta (veja abaixo). Pesquisar usando as tags do site pode ajudar a reduzir os resultados.

Se ainda não encontrou nada, poste sua pergunta no site cujo assunto mais se relaciona com ela. Use as ferramentas de formatação, especialmente para código, e adicione tags relacionadas ao assunto da pergunta (principalmente o nome da linguagem de programação, do sistema operacional ou da biblioteca com a qual você está tendo problemas). Se alguém pedir mais informações, edite sua postagem original para incluí-las. Se alguma resposta for útil, clique na seta para cima para dar um voto a ela; se a resposta resolver o seu problema, clique no ícone de "check" abaixo das setas de voto para marcá-la como aceita.

O Stack Exchange já cresceu para [mais de 100 sites](http://stackexchange.com/sites), mas estes são os candidatos mais prováveis:

- O [Super User](http://superuser.com) é para perguntas gerais sobre computação. Se a sua pergunta não é sobre código nem sobre programas com os quais você só interage por uma conexão de rede, ela provavelmente cabe aqui.
- O [Stack Overflow](http://stackoverflow.com) é para perguntas sobre programação.
- O [Server Fault](http://serverfault.com) é para perguntas sobre servidores e administração de redes.
- Muitos projetos têm seus próprios sites, incluindo [Android](http://android.stackexchange.com), [Ubuntu](http://askubuntu.com), [TeX/LaTeX](http://tex.stackexchange.com) e [Microsoft SharePoint](http://sharepoint.stackexchange.com). Acesse o [Stack Exchange](http://stackexchange.com) para ver a lista atualizada.

<a name="4.3"></a>

## Fóruns Web e IRC

Seu grupo de usuários local ou sua distribuição Linux podem divulgar um fórum Web ou canal IRC onde iniciantes conseguem ajuda (em países de língua não inglesa, os fóruns para iniciantes têm ainda mais chances de serem listas de e-mail). Esses são bons primeiros lugares para perguntar, especialmente se você acha que esbarrou em um problema comum e relativamente simples. Um canal IRC divulgado é um convite aberto para fazer perguntas e, muitas vezes, receber respostas em tempo real.

Aliás, se você obteve o programa que está dando problema por meio de uma distribuição Linux (o que é comum hoje em dia), é melhor perguntar no fórum/lista da distribuição antes de tentar o fórum/lista do projeto do programa. Os hackers do projeto podem simplesmente responder "use a nossa versão".

Antes de postar em qualquer fórum Web, verifique se ele tem um recurso de busca. Se tiver, tente algumas buscas por palavras-chave relacionadas ao seu problema; isso pode realmente ajudar. Se você já fez uma busca geral na Web (como deveria), pesquise no fórum mesmo assim; o mecanismo de busca que você usou pode não ter indexado o conteúdo recente do fórum.

Há uma tendência crescente de projetos oferecerem suporte aos usuários por meio de um fórum Web ou canal IRC, reservando o e-mail mais para o tráfego de desenvolvimento. Portanto, procure primeiro por esses canais quando buscar ajuda para projetos específicos.

No IRC, provavelmente é melhor não começar despejando uma longa descrição do problema no canal; algumas pessoas consideram isso "flood". É melhor soltar uma descrição de uma linha do problema, para puxar conversa.

<a name="4.4"></a>

## Como um segundo passo, use listas de e-mail de projeto

Quando um projeto tem uma lista de e-mail para desenvolvedores, escreva para a lista, não para desenvolvedores individuais, mesmo que você ache que sabe quem poderia responder melhor. Procure o endereço da lista na documentação e na página inicial do projeto, e use-o. Há várias boas razões para essa política:

Qualquer pergunta boa o bastante para ser feita a um desenvolvedor específico também é válida para todo o grupo. Por outro lado, se você suspeita que sua pergunta é boba demais para uma lista de e-mail, isso não é desculpa para perturbar desenvolvedores individualmente.

Fazer perguntas na lista distribui a carga entre os desenvolvedores. Um desenvolvedor específico (especialmente se for o líder do projeto) pode estar ocupado demais para responder às suas perguntas.

A maioria das listas de e-mail é arquivada, e os arquivos são indexados por mecanismos de busca. Se você fizer sua pergunta na lista e ela for respondida, outra pessoa pode encontrar a pergunta e a resposta na Web, em vez de perguntar de novo.

Se certas perguntas aparecem com frequência, os desenvolvedores podem usar essa informação para melhorar a documentação ou o próprio software, tornando-o menos confuso. Mas, se essas perguntas são feitas em particular, ninguém tem a visão completa das que mais aparecem.

Se o projeto tem tanto uma lista de "usuários" quanto uma de "desenvolvedores" (ou "hackers"), ou um fórum Web, e você não está mexendo no código, pergunte na lista/fórum de "usuários". Não presuma que será bem-vindo na lista de desenvolvedores, onde sua pergunta provavelmente será vista como ruído atrapalhando o tráfego de desenvolvimento.

No entanto, se você tem certeza de que a pergunta não é trivial e não obteve resposta na lista/fórum de "usuários" depois de vários dias, tente a lista de "desenvolvedores". É aconselhável acompanhar a lista em silêncio por alguns dias, ou pelo menos ler as mensagens arquivadas dos últimos dias, para se familiarizar com os costumes dos participantes antes de postar (aliás, esse é um bom conselho para qualquer lista privada ou semiprivada).

Se você não encontrou uma lista de e-mail do projeto, só o endereço do mantenedor, vá em frente e escreva para ele. Mas, mesmo nesse caso, não presuma que a lista não existe. Mencione no e-mail que você procurou e não encontrou uma lista. Mencione também que você não se importa que a sua mensagem seja encaminhada a outras pessoas. (Muita gente acredita que e-mail privado deve permanecer privado, mesmo que não haja nada secreto nele. Ao permitir o encaminhamento, você dá ao destinatário a escolha de como lidar com a mensagem.)

<a name="4.5"></a>

## Use linhas de assunto significativas e específicas

Em listas de e-mail, newsgroups ou fóruns Web, a linha de assunto é a sua chance de ouro de chamar a atenção de especialistas qualificados em 50 caracteres ou menos. Não a desperdice com lamúrias como "Por favor, me ajudem" (e esqueça "POR FAVOR, ME AJUDEM!!!"; mensagens com assuntos assim são descartadas por reflexo). Não tente nos impressionar com a profundidade da sua angústia; use o espaço para uma descrição superconcisa do problema.

Uma boa convenção para linhas de assunto, usada por muitas empresas de suporte técnico, é "objeto - desvio". A parte "objeto" especifica qual coisa ou grupo de coisas está com problema, e a parte "desvio" descreve o desvio em relação ao comportamento esperado.

- Estúpido: 
	- AJUDA! Vídeo não funciona corretamente no meu laptop!
- Inteligente: 
	- X.org 6.8.1 deforma o cursor do mouse, chipset de vídeo Fooware MV1005
- Mais inteligente:
	- Cursor do mouse fica deformado no X.org 6.8.1 com chipset de vídeo Fooware MV1005

O processo de escrever uma descrição "objeto - desvio" ajuda você a organizar melhor o seu raciocínio sobre o problema, com mais detalhes. O que é afetado? Só o cursor do mouse ou outros gráficos também? O problema é específico da versão do X.org usada pelo servidor X? Ocorre só na versão 6.8.1? É específico do chipset de vídeo Fooware? Ocorre só com o modelo MV1005? Um hacker que vê uma mensagem assim entende imediatamente, num piscar de olhos, com o que você está tendo problema e qual é o problema em si.

De modo geral, imagine-se examinando o índice de um arquivo de perguntas em que só aparecem as linhas de assunto. Faça sua linha de assunto refletir bem a pergunta, para que a próxima pessoa, ao pesquisar o arquivo com uma dúvida parecida com a sua, consiga seguir a trilha até a resposta em vez de postar a pergunta de novo.

Se você fizer uma pergunta em uma resposta, não deixe de alterar a linha de assunto para indicar isso. Um assunto como "Re: teste" ou "Re: novo bug" tem menos chances de atrair uma boa dose de atenção. Além disso, reduza as citações de mensagens anteriores ao mínimo necessário para situar os leitores seguintes.

Não simplesmente clique em "Responder" a uma mensagem de uma lista de e-mail para iniciar uma thread completamente nova. Isso limita a sua audiência. Alguns leitores de e-mail, como o *mutt*, permitem organizar as mensagens por thread e então ocultar as threads (normalmente com um + para expandir e um - para recolher). Quem faz isso nunca verá a sua mensagem.

Mudar o assunto não basta. O *mutt*, e provavelmente outros leitores de e-mail, usam outras informações nos cabeçalhos para atribuir a mensagem a uma thread, e não a linha de assunto. Nesses casos, portanto, você deve começar um e-mail completamente novo.

Em fóruns Web, as regras de etiqueta são um pouco diferentes, porque as mensagens costumam estar muito mais ligadas a threads de discussão específicas e, muitas vezes, são invisíveis fora deles. Mudar o assunto ao fazer uma pergunta em resposta a outra não é essencial. Nem todos os fóruns permitem assuntos diferentes nas respostas, e quase ninguém os lê quando são diferentes. Ainda assim, fazer uma pergunta em uma resposta já é uma prática duvidosa por si só, porque a pergunta só será vista por quem está acompanhando a thread. Portanto, a menos que você tenha certeza de que quer perguntar apenas às pessoas ativas na thread, abra uma nova.

<a name="4.6"></a>

## Facilite a resposta

Terminar sua pergunta com “Por favor, envie sua resposta para...” torna bem improvável que você receba uma resposta. Se você não se deu ao trabalho de gastar os poucos segundos necessários para configurar um cabeçalho Reply-To correto no seu programa de e-mail, nós não vamos nos dar ao trabalho de gastar alguns segundos pensando no seu problema. Se o seu programa de e-mail não permite isso, [arrume um programa melhor](http://linuxmafia.com/faq/Mail/muas.html). Se o seu sistema operacional não suporta nenhum programa de e-mail que permita isso, arrume um sistema operacional melhor.

Em fóruns Web, pedir resposta por e-mail é francamente rude, a menos que você ache que a informação possa ser sigilosa (e que alguém, por algum motivo desconhecido, vá contá-la a você, mas não ao fórum inteiro). Se você quer uma cópia por e-mail quando alguém responder na thread, peça ao fórum que a envie; esse recurso é suportado em quase todo lugar, em opções como “acompanhar esta thread”, “enviar e-mail quando houver respostas”, etc.

<a name="4.7"></a>

## Escreva com clareza e correção gramatical e ortográfica

Descobrimos por experiência que quem escreve de forma descuidada e desleixada geralmente também é descuidado e desleixado ao pensar e ao programar (com frequência suficiente para apostar nisso, pelo menos). Responder a perguntas de pessoas descuidadas e desleixadas não é gratificante; preferimos gastar nosso tempo em outro lugar.

Por isso, expressar sua pergunta de forma clara e bem-feita é importante. Se você não se dá ao trabalho de fazer isso, nós não nos damos ao trabalho de prestar atenção. Dedique um esforço extra para polir sua linguagem. Ela não precisa ser rígida nem formal — na verdade, a cultura hacker valoriza a linguagem informal, cheia de gírias e bem-humorada, desde que usada com rigor. Mas tem de haver rigor; é preciso algum sinal de que você está pensando e prestando atenção.

Use ortografia, pontuação e maiúsculas corretas. Não confunda “mas” com “mais”, “há” com “a” ou “a gente” com “agente”. Não ESCREVA TUDO EM MAIÚSCULAS; isso é lido como gritaria e considerado rude. (Escrever tudo em minúsculas é só um pouco menos irritante, porque é difícil de ler. Alan Cox pode se dar a esse luxo, mas você não.)

De modo mais geral, se você escrever como um semianalfabeto, muito provavelmente será ignorado. Portanto, não use abreviações de mensageiros instantâneos. Escrever “vc” em vez de “você” faz você parecer um semianalfabeto só para economizar míseras teclas. Pior: escrever como um script kiddie hax0r l33t é o beijo da morte e garante que você não receberá nada além de um silêncio sepulcral (ou, na melhor das hipóteses, uma bela porção de desprezo e sarcasmo).

Se você está fazendo perguntas em um fórum que não usa o seu idioma nativo, terá uma folga limitada para erros de ortografia e gramática — mas nenhuma folga para a preguiça (e sim, geralmente conseguimos perceber a diferença). Além disso, a menos que você saiba quais idiomas seus respondentes falam, escreva em inglês. Hackers ocupados tendem a simplesmente descartar perguntas em idiomas que não entendem, e o inglês é a língua de trabalho da Internet. Escrevendo em inglês, você minimiza a chance de a sua pergunta ser descartada sem ser lida.

Se você escreve em inglês, mas ele é a sua segunda língua, é de bom tom avisar os possíveis respondentes sobre eventuais dificuldades de idioma e sobre formas de contorná-las. Exemplos:

English is not my native language; please excuse typing errors. (O inglês não é a minha língua nativa; por favor, desculpem os erros de digitação.)

If you speak $LANGUAGE, please e-mail/PM me; I may need assistance translating my question. (Se você fala $IDIOMA, por favor, me envie um e-mail/mensagem privada; posso precisar de ajuda para traduzir minha pergunta.)

I am familiar with the technical terms, but some slang expressions and idioms are difficult for me. (Conheço os termos técnicos, mas algumas gírias e expressões idiomáticas são difíceis para mim.)

I've posted my question in $LANGUAGE and English. I'll be glad to translate responses, if you only use one or the other. (Postei minha pergunta em $IDIOMA e em inglês. Terei prazer em traduzir as respostas, se você usar apenas um dos dois.)

<a name="4.8"></a>

## Envie perguntas em formatos acessíveis e padronizados

Se você tornar sua pergunta artificialmente difícil de ler, ela tem mais chances de ser deixada de lado em favor de outra que não seja. Portanto:

Envie e-mail em texto simples, não em HTML. (Não é difícil [desativar o HTML](http://www.birdhouse.org/etc/evilmail.html).)

Anexos MIME geralmente são aceitáveis, mas somente se forem conteúdo de verdade (como um arquivo-fonte ou um patch anexado), e não apenas texto padrão gerado pelo seu cliente de e-mail (como outra cópia da sua mensagem).

Não envie e-mails em que parágrafos inteiros são uma única linha quebrada várias vezes. (Isso dificulta responder apenas a uma parte da mensagem.) Presuma que seus respondentes lerão e-mails em telas de texto de 80 colunas e configure a quebra de linha para menos de 80.

Entretanto, não quebre dados (como dumps de arquivos de log ou transcrições de sessão) em nenhuma largura fixa de coluna. Os dados devem ser incluídos como estão, para que os respondentes tenham confiança de que estão vendo o que você viu.

Não envie a codificação MIME Quoted-Printable para um fórum em inglês. Essa codificação pode ser necessária ao postar em um idioma que o ASCII não cobre, mas muitos agentes de e-mail não a suportam. Quando ela falha, todos aqueles glifos =20 espalhados pelo texto são feios e distraem — ou podem até sabotar a semântica do seu texto.

Nunca, jamais espere que hackers consigam ler formatos de documento proprietários fechados, como Microsoft Word ou Excel. A maioria dos hackers reage a eles mais ou menos como você reagiria a uma pilha de esterco de porco fumegante despejada na sua porta. Mesmo quando conseguem lidar com eles, ficam ressentidos por terem de fazê-lo.

Se você envia e-mail de uma máquina Windows, desative o problemático recurso “Aspas inteligentes” da Microsoft (em Ferramentas > Opções de AutoCorreção, desmarque a caixa de aspas inteligentes em AutoFormatação ao Digitar). Isso evita que caracteres-lixo sejam espalhados pelo seu e-mail.

Em fóruns Web, não abuse dos recursos de “smileys” e “HTML” (quando existirem). Um smiley ou dois geralmente são aceitáveis, mas texto colorido e floreado tende a fazer as pessoas acharem que você é um bobo. Exagerar seriamente em smileys, cores e fontes fará você parecer uma adolescente dando risadinhas, o que geralmente não é uma boa ideia, a menos que você esteja mais interessado em sexo do que em respostas.

Se você usa um cliente de e-mail com interface gráfica, como Netscape Messenger, MS Outlook ou similares, cuidado: ele pode violar essas regras com as configurações padrão. A maioria desses clientes tem um comando de menu “Exibir código-fonte” (View Source). Use-o em alguma mensagem da sua pasta de enviados para verificar se você está enviando texto simples, sem anexos desnecessários.

<a name="4.9"></a>

## Seja preciso e informativo sobre o seu problema

Descreva com cuidado e clareza os sintomas do seu problema ou bug.

Descreva o ambiente em que ele ocorre (máquina, sistema operacional, aplicação, o que for). Informe a distribuição do seu fornecedor e o nível de versão (por exemplo: “Fedora Core 7”, “Slackware 9.1”, etc.).

Descreva a pesquisa que você fez para tentar entender o problema antes de perguntar.

Descreva os passos de diagnóstico que você executou para tentar identificar o problema por conta própria antes de perguntar.

Descreva quaisquer mudanças recentes, possivelmente relevantes, na configuração do seu computador ou software.

Se possível, forneça uma forma de reproduzir o problema em um ambiente controlado.

Faça o melhor possível para antecipar as perguntas que um hacker fará e responda a elas de antemão no seu pedido de ajuda.

Dar aos hackers a capacidade de reproduzir o problema em um ambiente controlado é especialmente importante se você está relatando algo que acha ser um bug no código. Quando você faz isso, suas chances de obter uma resposta útil, e a rapidez com que provavelmente a obterá, melhoram enormemente.

Simon Tatham escreveu um excelente ensaio intitulado [How to Report Bugs Effectively](http://www.chiark.greenend.org.uk/~sgtatham/bugs.html). Eu recomendo fortemente que você o leia.

<a name="4.10"></a>

## Volume não é precisão

Você precisa ser preciso e informativo. Despejar enormes volumes de código ou dados em um pedido de ajuda não contribui para isso. Se você tem um caso de teste grande e complicado que está quebrando um programa, tente reduzi-lo e deixá-lo o menor possível.

Isso é útil por pelo menos três razões. Um: ser visto investindo esforço em simplificar a pergunta torna mais provável que você receba uma resposta. Dois: simplificar a pergunta torna mais provável que você receba uma resposta útil. Três: no processo de refinar o seu relato de bug, você pode acabar desenvolvendo uma correção ou um contorno (workaround) por conta própria.

<a name="4.11"></a>

## Não se apresse em declarar que você encontrou um bug

Quando você estiver tendo problemas com um software, não afirme ter encontrado um bug a menos que tenha muita, muita certeza. Dica: a menos que você consiga fornecer um patch de código-fonte que corrija o problema, ou um teste de regressão contra uma versão anterior que demonstre comportamento incorreto, provavelmente você não tem certeza suficiente. Isso vale também para páginas Web e documentação; se você encontrou um “bug” na documentação, deve fornecer o texto substituto e dizer em quais páginas ele deve entrar.

Lembre-se: há muitos outros usuários que não estão tendo o seu problema. Caso contrário, você teria ficado sabendo disso ao ler a documentação e pesquisar na Web (você fez isso antes de reclamar, [não fez?](#3)). Isso significa que, muito provavelmente, é você quem está fazendo algo errado, e não o software.

As pessoas que escreveram o software trabalham muito para fazê-lo funcionar o melhor possível. Se você afirma ter encontrado um bug, estará questionando a competência delas, o que pode ofender alguns mesmo que você esteja certo. É especialmente indelicado gritar “bug” na linha de assunto.

Ao fazer sua pergunta, o melhor é escrever como se você presumisse que está fazendo algo errado, mesmo que, no íntimo, tenha bastante certeza de que encontrou um bug de verdade. Se houver mesmo um bug, você ficará sabendo na resposta. Aja de modo que os mantenedores queiram pedir desculpas a você caso o bug seja real, e não de modo que você lhes deva desculpas se tiver feito besteira.

<a name="4.12"></a>

## Bajulação não substitui o seu dever de casa

Algumas pessoas que entendem que não devem se comportar de modo rude ou arrogante, exigindo uma resposta, recuam para o extremo oposto, o de se rastejar. “Sei que sou apenas um novato patético e perdedor, mas...”. Isso distrai e não ajuda. É especialmente irritante quando vem acompanhado de vagueza sobre o problema real.

Não perca seu tempo, nem o nosso, com política de primata tosca. Em vez disso, apresente os fatos de contexto e a sua pergunta da forma mais clara possível. Essa é uma forma melhor de se posicionar do que se rastejar.

Às vezes os fóruns Web têm espaços separados para perguntas de novatos. Se você acha que tem mesmo uma pergunta de novato, vá direto para lá. Mas também não se rasteje lá.

<a name="4.13"></a>

## Descreva os sintomas do problema, não suas suposições

Não adianta dizer aos hackers o que você acha que está causando o seu problema. (Se as suas teorias de diagnóstico fossem tão boas assim, você estaria pedindo ajuda a outras pessoas?) Portanto, certifique-se de relatar os sintomas brutos do que dá errado, e não as suas interpretações e teorias. Deixe que eles façam a interpretação e o diagnóstico. Se achar importante declarar o seu palpite, rotule-o claramente como tal e descreva por que essa resposta não está funcionando para você.

- Estúpido:
	Estou recebendo erros SIG11 consecutivos ao compilar o kernel e suspeito de uma rachadura fina em uma das trilhas da placa-mãe. Qual é a melhor forma de verificar isso?

- Inteligente:
	Meu K6/233 montado em casa, com placa-mãe FIC-PA2007 (chipset VIA Apollo VP2) e 256 MB de SDRAM Corsair PC133, começa a ter erros SIG11 frequentes cerca de 20 minutos depois de ligado durante compilações do kernel, mas nunca nos primeiros 20 minutos. Reiniciar não zera a contagem, mas desligar durante a noite zera. Trocar toda a RAM não ajudou. A parte relevante do log de uma compilação típica segue abaixo.

Como o ponto anterior parece difícil de entender para muita gente, aqui vai uma frase para lembrar: “Todos os diagnosticadores são do Missouri.” O lema oficial desse estado americano é “Show me” (“Mostre-me”) (conquistado em 1899, quando o congressista Willard D. Vandiver disse “Venho de uma terra que produz milho, algodão, carrapichos e democratas, e eloquência espumante nem me convence nem me satisfaz. Sou do Missouri. Vocês têm de me mostrar.”). No caso dos diagnosticadores, não é questão de ceticismo, mas uma necessidade literal e funcional de ver algo o mais próximo possível da mesma evidência bruta que você vê, e não os seus palpites e resumos. Mostre-nos.

<a name="4.14"></a>

## Descreva os sintomas do seu problema em ordem cronológica

As pistas mais úteis para descobrir o que deu errado muitas vezes estão nos eventos imediatamente anteriores. Portanto, o seu relato deve descrever com precisão o que você fez, e o que a máquina e o software fizeram, até o problema estourar. No caso de processos de linha de comando, ter um log da sessão (por exemplo, usando o utilitário script) e citar as vinte linhas mais relevantes é muito útil.

Se o programa que falhou tem opções de diagnóstico (como -v para verbose), tente selecionar opções que acrescentem informação de depuração útil à transcrição. Lembre-se de que mais não é necessariamente melhor; tente escolher um nível de depuração que informe, em vez de afogar o leitor em lixo.

Se o seu relato ficar longo (mais de uns quatro parágrafos), pode ser útil declarar o problema de forma sucinta no começo e depois seguir com a história cronológica. Assim, os hackers saberão o que observar ao ler o seu relato.

<a name="4.15"></a>

## Descreva o objetivo, não o passo

Se você está tentando descobrir como fazer algo (em vez de relatar um bug), comece descrevendo o objetivo. Só depois descreva o passo específico em direção a ele em que você está bloqueado.

Muitas vezes, quem precisa de ajuda técnica tem um objetivo de alto nível em mente e trava naquilo que acha ser um caminho específico até ele. Essas pessoas pedem ajuda com o passo, mas não percebem que o caminho está errado. Pode dar bastante trabalho superar isso.

- Estúpido:
	Como faço o seletor de cores do programa FooDraw aceitar um valor RGB hexadecimal?

- Inteligente:
	Estou tentando substituir a tabela de cores de uma imagem por valores da minha escolha. No momento, a única forma que vejo de fazer isso é editando cada posição da tabela, mas não consigo fazer o seletor de cores do FooDraw aceitar um valor RGB hexadecimal.

A segunda versão da pergunta é a inteligente. Ela permite uma resposta que sugira uma ferramenta mais adequada à tarefa.

<a name="4.16"></a>

## Não peça respostas por e-mail privado

Hackers acreditam que resolver problemas deve ser um processo público e transparente, em que uma primeira tentativa de resposta pode e deve ser corrigida se alguém mais conhecedor perceber que ela está incompleta ou incorreta. Além disso, parte da recompensa de quem ajuda vem de ser visto como competente e conhecedor por seus pares.

Quando você pede uma resposta privada, atrapalha tanto o processo quanto a recompensa. Não faça isso. Cabe ao respondente decidir se responde em particular — e, se o fizer, geralmente é porque acha que a pergunta é mal formulada ou óbvia demais para interessar aos outros.

Há uma exceção limitada a essa regra. Se você acha que a pergunta é do tipo que vai render muitas respostas muito parecidas, as palavras mágicas são “mande um e-mail e eu faço um resumo das respostas para o grupo”. É cortês tentar poupar a lista de e-mail ou o newsgroup de uma enxurrada de postagens substancialmente idênticas — mas você tem de cumprir a promessa de resumir.

<a name="4.17"></a>

## Seja explícito sobre a sua pergunta

Perguntas abertas tendem a ser vistas como sorvedouros de tempo sem fim. As pessoas mais capazes de lhe dar uma resposta útil também são as mais ocupadas (nem que seja porque assumem a maior parte do trabalho). Pessoas assim têm alergia a sorvedouros de tempo sem fim e, por isso, tendem a ter alergia a perguntas abertas.

Você tem mais chances de obter uma resposta útil se for explícito sobre o que quer que os respondentes façam (dar indicações, enviar código, verificar o seu patch, o que for). Isso vai focar o esforço deles e impor, implicitamente, um limite máximo ao tempo e à energia que um respondente precisa dedicar a ajudar você. Isso é bom.

Para entender o mundo em que os especialistas vivem, pense na expertise como um recurso abundante e no tempo para responder como um recurso escasso. Quanto menor o compromisso de tempo que você pede, implicitamente, maiores as chances de obter resposta de alguém realmente bom e realmente ocupado.

Portanto, é útil formular sua pergunta de modo a minimizar o tempo exigido de um especialista para tratá-la — mas isso muitas vezes não é o mesmo que simplificar a pergunta. Assim, por exemplo, “Você poderia me indicar uma boa explicação sobre X?” geralmente é uma pergunta mais inteligente do que “Você poderia me explicar X, por favor?”. Se você tem um código com defeito, geralmente é mais inteligente pedir que alguém explique o que há de errado com ele do que pedir que o conserte.

<a name="4.18"></a>

## Ao perguntar sobre código

Não peça a outros que depurem o seu código quebrado sem dar uma pista do tipo de problema que devem procurar. Postar algumas centenas de linhas de código dizendo “não funciona” fará você ser ignorado. Postar uma dúzia de linhas dizendo “depois da linha 7 eu esperava ver <x>, mas aconteceu <y>” tem muito mais chance de render uma resposta.

A forma mais eficaz de ser preciso sobre um problema de código é fornecer um caso de teste mínimo que demonstre o bug. O que é um caso de teste mínimo? É uma ilustração do problema; apenas código suficiente para exibir o comportamento indesejado e nada mais. Como fazer um caso de teste mínimo? Se você sabe qual linha ou trecho do código produz o comportamento problemático, faça uma cópia dele e acrescente apenas o código de apoio necessário para produzir um exemplo completo (ou seja, o suficiente para que o código-fonte seja aceito pelo compilador/interpretador/seja qual for a aplicação que o processa). Se você não consegue restringir a um trecho específico, faça uma cópia do código-fonte e comece a remover pedaços que não afetam o comportamento problemático. Quanto menor o seu caso de teste mínimo, melhor (veja [a seção “Volume não é precisão”](#4.10)).

Gerar um caso de teste realmente pequeno nem sempre será possível, mas tentar é uma boa disciplina. Isso pode ajudar você a aprender o que precisa para resolver o problema por conta própria — e, mesmo quando não ajuda, os hackers gostam de ver que você tentou. Isso os deixará mais cooperativos.

Se você simplesmente quer uma revisão de código, diga isso logo de início e mencione quais áreas acha que podem precisar de revisão especial e por quê.

<a name="4.19"></a>

## Não poste perguntas de dever de casa

Hackers são bons em identificar perguntas de dever de casa; a maioria de nós já fez muitas. Essas perguntas são para você resolver, para que aprenda com a experiência. Não há problema em pedir dicas, mas não soluções completas.

Se você suspeita que recebeu uma pergunta de dever de casa, mas mesmo assim não consegue resolvê-la, tente perguntar em um fórum de grupo de usuários ou (como último recurso) em uma lista/fórum de “usuários” de um projeto. Embora os hackers vão perceber o que é, alguns dos usuários avançados talvez pelo menos deem uma dica.

<a name="4.20"></a>

## Elimine perguntas vazias

Resista à tentação de encerrar o seu pedido de ajuda com perguntas semanticamente nulas como “Alguém pode me ajudar?” ou “Existe alguma resposta?”. Primeiro: se você escreveu a descrição do problema de forma minimamente competente, essas perguntas acrescentadas são, no máximo, supérfluas. Segundo: justamente por serem supérfluas, os hackers as acham irritantes — e provavelmente responderão de forma logicamente impecável, porém desdenhosa, como “Sim, você pode ser ajudado” e “Não, não há ajuda para você.”

Em geral, evite perguntas de sim ou não, a menos que você queira uma [resposta de sim ou não](http://homepage.ntlworld.com./jonathan.deboynepollard/FGA/questions-with-yes-or-no-answers.html).

<a name="4.21"></a>

## Não marque sua pergunta como “Urgente”, mesmo que seja urgente para você

Esse é problema seu, não nosso. Alegar urgência tem grande chance de ser contraproducente: a maioria dos hackers simplesmente apagará essas mensagens, vendo-as como tentativas rudes e egoístas de obter atenção imediata e especial. Além disso, a palavra “Urgente” (e outras tentativas semelhantes de chamar atenção na linha de assunto) muitas vezes aciona filtros de spam — seus destinatários podem nem chegar a ver a mensagem!

Há uma semiexceção. Pode valer a pena mencionar que você está usando o programa em algum lugar de alto perfil, que deixe os hackers empolgados; nesse caso, se você está sob pressão de tempo e diz isso com educação, as pessoas podem se interessar o bastante para responder mais rápido.

Isso é muito arriscado, porém, porque o critério dos hackers para o que é empolgante provavelmente difere do seu. Postar da Estação Espacial Internacional se qualificaria, por exemplo, mas postar em nome de uma causa beneficente ou política edificante quase certamente não. Na verdade, postar “Urgente: Ajudem a salvar os filhotes de foca!” garante que você será evitado ou atacado (flamed) até por hackers que acham os filhotes de foca importantes.

Se isso lhe parece misterioso, releia este guia inteiro quantas vezes for preciso até entender, antes de postar qualquer coisa.

<a name="4.22"></a>

## Educação nunca fez mal, e às vezes ajuda

Seja cortês. Use “Por favor” e “Obrigado pela atenção” ou “Obrigado pela consideração”. Deixe claro que você agradece o tempo que as pessoas dedicam a ajudar você de graça.

Para ser honesto, isso não é tão importante quanto (nem pode substituir) ser gramatical, claro, preciso e descritivo, evitar formatos proprietários etc.; os hackers em geral preferem relatos de bug um tanto bruscos, mas tecnicamente afiados, a uma polidez vaga. (Se isso o deixa intrigado, lembre-se de que valorizamos uma pergunta pelo que ela nos ensina.)

No entanto, se você tem os seus pontos técnicos em ordem, a educação realmente aumenta as chances de obter uma resposta útil.

(Devemos registrar que a única objeção séria que recebemos de hackers veteranos a este HOWTO diz respeito à nossa recomendação anterior de usar “Obrigado desde já” (“Thanks in advance”). Alguns hackers acham que isso dá a entender a intenção de não agradecer a ninguém depois. Nossa recomendação é dizer “Obrigado desde já” primeiro e agradecer aos respondentes depois, ou expressar cortesia de outra forma, como dizendo “Obrigado pela atenção” ou “Obrigado pela consideração”.)

<a name="4.23"></a>

## Faça um breve acompanhamento sobre a solução

Envie uma nota a todos que o ajudaram depois que o problema for resolvido; conte como terminou e agradeça de novo pela ajuda. Se o problema despertou interesse geral em uma lista de e-mail ou newsgroup, é apropriado postar o acompanhamento lá.

O ideal é que a resposta seja enviada na thread iniciada pela pergunta original e tenha ‘RESOLVIDO’, ‘SOLUCIONADO’ ou uma etiqueta igualmente óbvia na linha de assunto. Em listas de e-mail de resposta rápida, um possível respondente que vê uma thread sobre “Problema X” terminando com “Problema X - RESOLVIDO” sabe que não precisa perder tempo lendo a thread (a menos que ele(a) mesmo(a) ache o Problema X interessante) e pode usar esse tempo para resolver outro problema.

Seu acompanhamento não precisa ser longo nem complicado; um simples “Olá — era um cabo de rede com defeito! Obrigado a todos. - Bill” já seria melhor que nada. Na verdade, um resumo curto e simpático é melhor que uma longa dissertação, a menos que a solução tenha profundidade técnica real. Diga qual ação resolveu o problema, mas não precisa reproduzir toda a sequência de investigação.

Para problemas com mais profundidade, é apropriado postar um resumo do histórico de investigação. Descreva o enunciado final do problema. Descreva o que funcionou como solução e indique depois os becos sem saída evitáveis. Os becos sem saída devem vir depois da solução correta e do restante do resumo, em vez de transformar o acompanhamento em uma história de detetive. Cite o nome das pessoas que ajudaram você; assim você fará amigos.

Além de cortês e informativo, esse tipo de acompanhamento ajudará outras pessoas que pesquisarem no arquivo da lista/newsgroup/fórum a saber exatamente qual solução funcionou para você e, portanto, também pode ajudá-las.

Por último, mas não menos importante, esse tipo de acompanhamento dá a todos que ajudaram uma satisfatória sensação de fechamento sobre o problema. Se você não é técnico nem hacker, acredite: essa sensação é muito importante para os gurus e especialistas a quem você recorreu. Narrativas de problemas que se perdem em um nada sem solução são frustrantes; hackers têm coceira para vê-las resolvidas. A boa vontade que você ganha ao aliviar essa coceira será muito, muito útil na próxima vez que você precisar fazer uma pergunta.

Pense em como você poderia evitar que outras pessoas tenham o mesmo problema no futuro. Pergunte-se se um patch na documentação ou na FAQ ajudaria e, se a resposta for sim, envie esse patch ao mantenedor.

Entre hackers, esse tipo de bom acompanhamento é, na verdade, mais importante que a educação convencional. É assim que você ganha a reputação de quem trabalha bem com os outros, o que pode ser um patrimônio muito valioso.

<a name="5"></a>

# Como interpretar respostas

<a name="5.1"></a>

## RTFM e STFW: Como saber que você pisou feio na bola

Existe uma tradição antiga e venerada: se você receber uma resposta que diz “RTFM”, a pessoa que a enviou acha que você deveria ter lido o Maldito Manual (*Read The Fucking Manual*). Ela quase certamente tem razão. Vá ler.

O RTFM tem um parente mais novo. Se você receber uma resposta que diz “STFW”, a pessoa que a enviou acha que você deveria ter pesquisado na Maldita Web (*Searched The Fucking Web*). Ela quase certamente tem razão. Vá pesquisar. (A versão mais branda é quando lhe dizem “O Google é seu amigo!”)

Em fóruns Web, também podem lhe dizer para pesquisar nos arquivos do fórum. Aliás, alguém pode até ser gentil o bastante para indicar a thread anterior em que o problema foi resolvido. Mas não conte com essa gentileza; faça a sua pesquisa nos arquivos antes de perguntar.

Muitas vezes, quem manda você pesquisar está com o manual ou a página Web que contém a informação de que você precisa aberto, olhando para ele enquanto digita. Essas respostas significam que o respondente acha que (a) a informação de que você precisa é fácil de achar e (b) você aprenderá mais se for atrás dela do que se a receber de mão beijada.

Você não deve se ofender com isso; pelos padrões hackers, seu respondente está lhe mostrando uma espécie de respeito rude simplesmente por não ignorá-lo. Em vez disso, deve ser grato por essa gentileza de avó.

<a name="5.2"></a>

## Se você não entendeu...

Se você não entender a resposta, não devolva imediatamente um pedido de esclarecimento. Use as mesmas ferramentas que usou para tentar responder à pergunta original (manuais, FAQs, a Web, amigos experientes) para entender a resposta. Depois, se ainda precisar pedir esclarecimento, mostre o que você aprendeu.

Por exemplo, suponha que eu diga: “Parece que você tem um zentry travado; você vai precisar limpá-lo.” Uma pergunta de acompanhamento ruim seria: “O que é um zentry?” Uma boa pergunta de acompanhamento seria: “OK, li a man page e os zentries só são mencionados nas opções -z e -p. Nenhuma delas diz nada sobre limpar zentries. É uma dessas ou estou deixando passar alguma coisa?”

<a name="5.3"></a>

## Como lidar com grosseria

Muito do que parece grosseria nos círculos hackers não tem a intenção de ofender. É, antes, o produto do estilo de comunicação direto, que corta a enrolação, natural em quem se preocupa mais em resolver problemas do que em deixar os outros com a sensação de estarem sendo acarinhados.

Quando perceber grosseria, tente reagir com calma. Se alguém estiver realmente passando dos limites, é muito provável que uma pessoa sênior da lista, do newsgroup ou do fórum chame a atenção dela. Se isso não acontecer e você perder a calma, é provável que a pessoa com quem você perdeu a calma estivesse se comportando dentro das normas da comunidade hacker e que você seja considerado o culpado. Isso prejudicará as suas chances de obter a informação ou a ajuda que você quer.

Por outro lado, de vez em quando você se deparará com grosseria e pose totalmente gratuitas. O reverso do que foi dito acima é que é aceitável criticar com bastante dureza os verdadeiros infratores, dissecando seu mau comportamento com um bisturi verbal afiado. Tenha muita, muita certeza do seu terreno antes de tentar isso, porém. A linha entre corrigir uma incivilidade e iniciar uma flamewar inútil é tão tênue que os próprios hackers não raramente a cruzam sem querer; se você é novato ou de fora, suas chances de evitar esse deslize são baixas. Se você busca informação, e não entretenimento, é melhor manter os dedos longe do teclado do que arriscar.

(Algumas pessoas afirmam que muitos hackers têm uma forma leve de autismo ou síndrome de Asperger e na verdade carecem de parte dos circuitos cerebrais que lubrificam a interação social “normal”. Isso pode ou não ser verdade. Se você não é hacker, pode ajudar a lidar com as nossas excentricidades pensar em nós como pessoas com lesão cerebral. Fique à vontade. Não nos importamos; gostamos de ser o que quer que sejamos e, em geral, temos um saudável ceticismo em relação a rótulos clínicos.)

As observações de Jeff Bigler sobre [filtros de tato](http://www.mit.edu/~jcb/tact.html) também são relevantes e valem a leitura.

Na próxima seção, falaremos de uma questão diferente: o tipo de “grosseria” que você verá quando se comportar mal.

<a name="6"></a>

# Não reaja como um perdedor

É provável que você erre algumas vezes em fóruns da comunidade hacker — das formas detalhadas neste artigo, ou semelhantes. E lhe dirão exatamente como você errou, possivelmente com comentários coloridos. Em público.

Quando isso acontecer, a pior coisa que você pode fazer é reclamar da experiência, alegar ter sofrido agressão verbal, exigir desculpas, gritar, prender a respiração, ameaçar com processos, reclamar aos empregadores das pessoas, deixar a tampa do vaso levantada, etc. Em vez disso, faça o seguinte:

Supere. É normal. Na verdade, é saudável e apropriado.

Os padrões da comunidade não se mantêm sozinhos: são mantidos por pessoas que os aplicam ativamente, de forma visível, em público. Não reclame que toda crítica deveria ter sido feita por e-mail privado: não é assim que funciona. Também não adianta insistir que você foi insultado pessoalmente quando alguém comenta que uma de suas afirmações estava errada ou que a opinião dele difere. Essas são atitudes de perdedor.

Já houve fóruns hackers em que, por um senso equivocado de hipercortesia, os participantes eram proibidos de apontar falhas nas postagens dos outros e ouviam “Não diga nada se não estiver disposto a ajudar o usuário.” A consequente saída dos participantes bem informados para outros lugares fez esses fóruns descerem a um falatório sem sentido e se tornarem inúteis como fóruns técnicos.

Exageradamente “amigável” (desse jeito) ou útil: escolha um.

Lembre-se: quando aquele hacker diz que você errou e (por mais ríspido que seja) diz para não repetir, ele está agindo por preocupação com (1) você e (2) a comunidade dele. Seria muito mais fácil para ele ignorar você e filtrá-lo da vida dele. Se você não consegue ser grato, tenha pelo menos um pouco de dignidade, não reclame e não espere ser tratado como uma boneca de porcelana só porque é um recém-chegado com uma alma teatralmente hipersensível e delírios de merecimento.

Às vezes as pessoas vão atacar você pessoalmente, soltar flames sem motivo aparente, etc., mesmo que você não tenha errado (ou só tenha errado na imaginação delas). Nesse caso, reclamar é a forma de realmente errar.

Esses flamers são ou lamers que não têm noção mas se acham especialistas, ou aspirantes a psicólogo testando se você vai errar. Os outros leitores ou os ignoram ou dão um jeito de lidar com eles por conta própria. O comportamento dos flamers cria problemas para eles mesmos, que não precisam preocupar você.

Também não se deixe arrastar para uma flamewar. A maioria dos flames é melhor ignorada — depois de você verificar se são mesmo flames, e não indicações de como você errou, nem respostas habilmente cifradas para a sua pergunta real (isso também acontece).

<a name="7"></a>

# Perguntas que não devem ser feitas

Aqui estão algumas perguntas estúpidas clássicas e o que os hackers pensam quando não as respondem.

- P: Onde posso encontrar o programa ou recurso X?
	- R: No mesmo lugar em que eu o encontraria, seu tolo — na outra ponta de uma busca na Web. Meu Deus do céu, será que ainda não é todo mundo que sabe usar o [Google](http://www.google.com)?

- P: Como posso usar X para fazer Y?
	- R: Se o que você quer é fazer Y, deveria fazer essa pergunta sem pressupor o uso de um método que pode não ser apropriado.
	- Perguntas desse tipo costumam indicar uma pessoa que não é apenas ignorante sobre X, mas também confusa sobre qual problema Y está resolvendo e fixada demais nos detalhes da sua situação particular. Geralmente é melhor ignorar essas pessoas até que definam melhor o problema.

- P: Como posso configurar o prompt do meu shell?
	- R: Se você é esperto o bastante para fazer essa pergunta, é esperto o bastante para dar um [RTFM](#5.1) e descobrir sozinho.

- P: Posso converter um documento da AcmeCorp em um arquivo TeX usando o conversor de arquivos Bass-o-matic?
	- R: Tente e veja. Se tivesse feito isso, você (a) aprenderia a resposta e (b) pararia de me fazer perder tempo.

- P: Meu {programa, configuração, instrução SQL} não funciona
	- R: Isso não é uma pergunta, e não estou interessado em jogar Vinte Perguntas para arrancar de você a sua pergunta de verdade — tenho coisas melhores a fazer.
	
	- Ao ver algo assim, minha reação normalmente é uma destas:
		- você tem mais alguma coisa a acrescentar?
		- ah, que pena, espero que você consiga consertar.
		- e o que exatamente isso tem a ver comigo?

- P: Estou tendo problemas com a minha máquina Windows. Podem ajudar?
	- R: Sim. Jogue fora esse lixo da Microsoft e instale um sistema operacional de código aberto como Linux ou BSD.
	- Nota: você pode fazer perguntas relacionadas a máquinas Windows se elas forem sobre um programa que tenha build oficial para Windows ou que interaja com máquinas Windows (por exemplo, o Samba). Só não se surpreenda com a resposta de que o problema é do Windows e não do programa, porque o Windows é tão problemático em geral que isso acontece com muita frequência.

- P: Meu programa não funciona. Acho que o recurso X do sistema está quebrado.
	- R: Embora seja possível que você seja a primeira pessoa a notar uma deficiência óbvia em chamadas de sistema e bibliotecas muito usadas por centenas ou milhares de pessoas, é bem mais provável que você seja totalmente leigo. Afirmações extraordinárias exigem evidências extraordinárias; quando fizer uma afirmação como essa, você deve sustentá-la com documentação clara e exaustiva do caso de falha.

- P: Estou com problemas para instalar o Linux ou o X. Podem ajudar?
	- R: Não. Eu precisaria de acesso direto à sua máquina para resolver isso. Procure o grupo de usuários Linux da sua região para obter ajuda presencial. (Há uma lista de grupos de usuários [aqui](http://www.linux.org/groups/index.html).)
	- Nota: perguntas sobre instalar o Linux podem ser apropriadas se você está em um fórum ou lista sobre uma distribuição específica e o problema é com essa distro; ou em fóruns de grupos de usuários locais. Nesse caso, descreva os detalhes exatos da falha. Mas antes faça uma pesquisa cuidadosa, com “linux” e todas as peças de hardware suspeitas.

- P: Como posso quebrar a senha de root / roubar privilégios de operador de canal / ler o e-mail de alguém?
	- R: Você é um canalha por querer fazer essas coisas e um tolo por pedir a um hacker que o ajude.

<a name="8"></a>

# Perguntas boas e ruins

Por fim, vou ilustrar com exemplos como fazer perguntas de forma inteligente; pares de perguntas sobre o mesmo problema, uma feita de forma estúpida e outra de forma inteligente.

- Exemplo 1
	- Estúpida: Onde posso descobrir coisas sobre o Foonly Flurbamatic?
	Essa pergunta está pedindo um [“STFW”](#5.1) como resposta.
	- Inteligente: Usei o Google para tentar encontrar “Foonly Flurbamatic 2600” na Web, mas não obtive resultados úteis. Posso receber uma indicação de informações de programação sobre esse dispositivo?
	Esta pessoa já fez o STFW e parece que pode haver um problema de verdade.

- Exemplo 2
	- Estúpida: Não consigo compilar o código do projeto foo. Por que ele está quebrado?
	Quem pergunta presume que outra pessoa errou. Que sujeito arrogante...
	- Inteligente: O código do projeto foo não compila no Nulix versão 6.2. Li a FAQ, mas ela não traz nada sobre problemas relacionados ao Nulix. Aqui está uma transcrição da minha tentativa de compilação; será que é algo que eu fiz?
	Quem pergunta especificou o ambiente, leu a FAQ, está mostrando o erro e não presume que os seus problemas sejam culpa de outra pessoa. Esta pergunta pode merecer alguma atenção.

- Exemplo 3
	- Estúpida: Estou com problemas na minha placa-mãe. Alguém pode ajudar?
	A resposta de um hacker qualquer a isso provavelmente será “Certo. Quer que eu também faça você arrotar e troque suas fraldas?”, seguida de um soco na tecla delete.
	- Inteligente: Tentei X, Y e Z na placa-mãe S2464. Como não funcionou, tentei A, B e C. Note o sintoma curioso quando tentei C. Obviamente o florbish está grommicking, mas os resultados não são o que se esperaria. Quais são as causas usuais de grommicking em placas-mãe Athlon MP? Alguém tem ideias de mais testes que eu possa rodar para delimitar o problema?
	Esta pessoa, por outro lado, parece merecer uma resposta. Ela demonstrou inteligência na resolução de problemas em vez de esperar passivamente que uma resposta caísse do alto.

Na última pergunta, note a diferença sutil, mas importante, entre exigir “Dê-me uma resposta” e pedir “Por favor, ajude-me a descobrir que diagnósticos adicionais posso rodar para chegar à iluminação.”

Na verdade, a forma dessa última pergunta é baseada de perto em um incidente real ocorrido em agosto de 2001 na lista de e-mail linux-kernel (lkml). Eu (Eric) fui quem fez a pergunta daquela vez. Eu estava tendo travamentos misteriosos em uma placa-mãe Tyan S2462. Os membros da lista forneceram as informações críticas de que eu precisava para resolvê-los.

Ao fazer a pergunta do jeito que fiz, dei às pessoas algo para mastigar; tornei fácil e atraente para elas se envolverem. Demonstrei respeito pela capacidade dos meus pares e os convidei a me consultar como um igual. Também demonstrei respeito pelo valor do tempo deles ao contar os becos sem saída pelos quais eu já havia passado.

Depois, quando agradeci a todos e comentei como o processo havia funcionado bem, um membro da lkml observou que achava que ele havia funcionado não porque eu sou um “nome” naquela lista, mas porque fiz a pergunta da forma correta.

Hackers são, em certos aspectos, uma meritocracia muito implacável; tenho certeza de que ele estava certo e de que, se eu tivesse me comportado como um aproveitador, teria sido atacado ou ignorado, não importa quem eu fosse. A sugestão dele de que eu escrevesse todo o incidente como instrução para outros levou diretamente à composição deste guia.

<a name="9"></a>

# Se você não consegue obter uma resposta

Se você não conseguir uma resposta, por favor não leve para o lado pessoal o fato de acharmos que não podemos ajudá-lo. Às vezes os membros do grupo consultado simplesmente não sabem a resposta. Não obter resposta não é o mesmo que ser ignorado, embora seja verdade que é difícil perceber a diferença de fora.

Em geral, simplesmente repostar a sua pergunta é uma má ideia. Isso será visto como um incômodo gratuito. Tenha paciência: a pessoa que tem a sua resposta pode estar em outro fuso horário e dormindo. Ou pode ser que a sua pergunta não estivesse bem formulada desde o início.

Existem outras fontes de ajuda a que você pode recorrer, muitas vezes mais adequadas às necessidades de um iniciante.

Existem muitos grupos de usuários, online e locais, formados por entusiastas do software, mesmo que eles nunca tenham escrito software. Esses grupos frequentemente se formam para que as pessoas se ajudem e ajudem novos usuários.

Há também muitas empresas comerciais, grandes e pequenas, que você pode contratar para obter ajuda. Não se desanime com a ideia de ter de pagar por um pouco de ajuda! Afinal, se o motor do seu carro queimar a junta do cabeçote, é provável que você o leve a uma oficina e pague para consertá-lo. Mesmo que o software não tenha custado nada, você não pode esperar que o suporte seja sempre de graça.

Para softwares populares como o Linux, há pelo menos 10.000 usuários por desenvolvedor. Simplesmente não é possível que uma pessoa atenda aos chamados de suporte de mais de 10.000 usuários. Lembre-se de que, mesmo que você tenha de pagar por suporte, ainda estará pagando muito menos do que se tivesse de comprar o software também (e o suporte para software de código fechado costuma ser mais caro e menos competente do que o de software de código aberto).

<a name="10"></a>

# Como responder perguntas de uma forma útil

Seja gentil. O estresse causado por problemas pode fazer as pessoas parecerem rudes ou estúpidas mesmo quando não são.

Responda a quem errou pela primeira vez em particular. Não há necessidade de humilhação pública para alguém que pode ter cometido um erro honesto. Um novato de verdade pode não saber como pesquisar nos arquivos nem onde a FAQ é armazenada ou publicada.

Se você não sabe com certeza, diga! Uma resposta errada, mas com ar de autoridade, é pior do que nenhuma. Não leve ninguém por um caminho errado só porque é divertido soar como especialista. Seja humilde e honesto; dê um bom exemplo tanto a quem perguntou quanto aos seus pares.

Se você não pode ajudar, não atrapalhe. Não faça piadas sobre procedimentos que poderiam destruir a configuração do usuário — o coitado pode interpretá-las como instruções.

Faça perguntas investigativas para obter mais detalhes. Se você for bom nisso, quem perguntou aprenderá algo — e você também. Tente transformar a pergunta ruim em uma boa; lembre-se de que todos já fomos novatos.

Embora murmurar RTFM às vezes se justifique ao responder a alguém que é só um preguiçoso desleixado, uma indicação da documentação (mesmo que seja só a sugestão de pesquisar uma frase-chave no Google) é melhor.

Se você vai responder à pergunta, ofereça uma resposta de qualidade. Não sugira gambiarras quando alguém está usando a ferramenta ou a abordagem errada. Sugira boas ferramentas. Reformule a pergunta.

Responda à pergunta de verdade! Se quem perguntou foi tão minucioso a ponto de pesquisar e de incluir na consulta que X, Y, Z, A, B e C já foram tentados sem bom resultado, é supremamente inútil responder “Tente A ou B”, ou com um link para algo que só diz “Tente X, Y, Z, A, B ou C.”.

Ajude a sua comunidade a aprender com a pergunta. Quando receber uma boa pergunta, pergunte-se: “Como a documentação ou a FAQ relevante teria de mudar para que ninguém precise responder a isso de novo?” Depois envie um patch ao mantenedor do documento.

Se você pesquisou para responder à pergunta, demonstre suas habilidades em vez de escrever como se tivesse tirado a resposta da cartola. Responder a uma boa pergunta é como dar uma refeição a uma pessoa faminta, mas ensinar habilidades de pesquisa pelo exemplo é mostrar a ela como cultivar alimento pela vida inteira.

<a name="11"></a>

# Recursos relacionados

Se você precisa de instrução sobre os fundamentos de como funcionam computadores pessoais, Unix e a Internet, veja o [The Unix and Internet Fundamentals HOWTO](http://en.tldp.org/HOWTO/Unix-and-Internet-Fundamentals-HOWTO/).

Quando você lançar software ou escrever patches para software, procure seguir as diretrizes do [Software Release Practice HOWTO](http://en.tldp.org/HOWTO/Software-Release-Practice-HOWTO/index.html).

<a name="12"></a>

# Agradecimentos

Evelyn Mitchell contribuiu com alguns exemplos de perguntas estúpidas e inspirou a seção “Como responder perguntas de uma forma útil”. Mikhail Ramendik contribuiu com sugestões de melhoria particularmente valiosas.