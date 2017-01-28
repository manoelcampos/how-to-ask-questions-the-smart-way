# Como Fazer Perguntas de Maneira Inteligente

Tradução baseada na [revisão 3.10 da versão original em inglês de 21 Maio de 2014](http://www.catb.org/~esr/faqs/smart-questions.html). 
A fork from the original English version can be found [here](README.en.md).

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
	- [Fórums Web e IRC](#4.3)
	- [Como um segundo passo, use listas de e-mail de projeto](#4.4)
	- [Use cabeçalhos de assunto significativos e específicos](#4.5) 
	- [Torne fácil para responder](#4.6)
	- [Escreva em linguagem clara, gramatica e ortograficamente correta](#4.7) 
	- [Envie questões em formatos acessíveis e padrões](#4.8)
	- [Seja preciso e informativo sobre o seu problema](#4.9)
	- [Volume não é precisão](#4.10)
	- [Não corra para declarar que você encontrou um bug](#4.11)
	- [Bajulação não substitui você de fazer seu trabalho de casa](#4.12)
	- [Descreva os sintomas do problema, não suas suposições](#4.13)
	- [Descreva os sintomas do seu problema em uma ordem cronológica](#4.14)
	- [Descreva o objetivo não o passo](#4.15)
	- [Não peça às pessoas para responderem por e-mail privado](#4.16)
	- [Seja explícito sobre sua questão](#4.17)
	- [Quando estiver perguntando sobre código](#4.18)
	- [Não poste perguntas sobre trabalho de casa](#4.19)
	- [Elimine perguntas sem sentido](#4.20)
	- [Não marque sua questão como “Urgente”, até mesmo se ela é pra você](#4.21)
	- [Cortesia nunca machuca, e algumas vezes ajuda](#4.22)
	- [Prossiga com uma breve nota sobre a solução](#4.23)
- [Como interpretar respostas](#5)
	- [RTFM e STFW: Como saber que você está seriamente ferrado](#5.1)
	- [Se você não entendeu...](#5.2)
	- [Lidando com grosseria](#5.3)
- [Não reagindo como um perdedor](#6)
- [Perguntas que não devem ser feitas](#7)
- [Perguntas boas e ruins](#8)
- [Se você não consegue obter uma resposta](#9)
- [Como responder perguntas de uma forma útil](#10)
- [Recursos relacionados](#11)
- [Agradecimentos](#12)

<a name="1"></a>

# Aviso Legal

Muitos websites de projetos incluem links para este documento em suas seções de como obter ajuda. Isto é bom, é o uso que pretendemos - mas se você é um webmaster criando tal link para sua página de projeto, por favor mostre, perto do link, um aviso proeminente que nós não somos help desk para o seu projeto!

Nós temos aprendido da maneira difícil que, sem tal aviso, nós repetidamente iremos ser importunados por idiotas que acham que por nós termos publicado este documento, é nosso trabalho resolver todos os problemas técnicos do mundo.

Se você está lendo este documento porque precisa de ajuda, e tiver a impressão de que a obterá diretamente dos autores deste documento, você é um dos idiotas que estamos falando a respeito.

Não nos faça perguntas. Nós iremos apenas ignorá-lo. Nós estamos aqui para mostrá-lo como obter ajuda que de fato conhecem o software ou hardware com o qual você está lidando, mas 99.9% das vezes não seremos nós. A menos que você saiba com certeza que um dos autores deste documento é um expert naquilo com o qual você está lidando, deixe nos em paz e todos ficarão felizes. 

<a name="2"></a>

# Introdução

Em um mundo de [hackers](http://www.catb.org/~esr/faqs/hacker-howto.html), o tipo de resposta que você obtém para suas perguntas técnicas depende muito da forma que você faz as perguntas como da dificuldade de desenvolver a resposta. Este guia irá ensiná-lo como fazer perguntas de uma forma que seja mais provável de obter uma resposta satisfatória.

Agora que projetos de open source (código aberto) se difundiram, você frequentemente pode obter boas respostas de usuários mais experientes do que de hackers. Isto é uma Coisa Boa; usuários tendem a ser apenas um pouco mais tolerantes ao tipo de falhas que iniciantes frequentemente cometem. Ainda, tratar usuários experientes como hackers, das formas que recomendamos aqui, irá geralmente ser mais eficiente para obter respostas úteis deles, também.  

A primeira coisa a entender é que hackers realmente gostam de problemas difíceis e perguntas boas e instigantes sobre eles. Se não gostassemos, não estaríamos aqui. Se você nos fornece uma questão interessante para mastigar, seremos gratos a você; boas perguntas são um estímulo e uma dádiva. Boas perguntas nos ajudam a desenvolver nosso entendimento, e frequentemente revelam problemas que podemos não ter notado ou pensado a respeito de outra maneira. Entre hackers, "Boa pergunta!" é um cumprimento forte e sincero.

Apesar disto, hackers tem uma reputação de responder questões simples de uma maneira que parece hostil e arrogante. Algumas vezes parece que somos automaticamente rudes com iniciantes e ignorantes. Mas isto não é realmente verdade. 

O que somos, indescupavelmente, é hostis com pessoas que parecem não querer pensar ou fazer seu próprio trabalho de casa antes de fazer perguntas. Pessoas como estas são sugadoras de tempo - elas tomam sem dar nada de volta, e disperdiçam o tempo que poderíamos ter gasto em outras questões mais interessantes ou outra pessoa que mais valha uma resposta. Nós chamamos pessoas assim de "losers (perdedores)" (e por razões históricas, algumas vezes soletramos "lusers"). 

Nós percebemos que existem muitas pessoas que apenas querem usar o software que desenvolvemos, e que não tem qualquer interesse em aprender detalhes técnicos. Para estes pessoas, um computador é meramente uma ferramenta, um emio para um fim; elas tem coisas mais importantes a fazer e vidas para viver. Nós reconhecemos isto, e não esperamos que cada um se interesse pelas questões técnicas que nos fascinam. No entanto, nosso estilo de responder perguntas é adaptado para pessoas que tem tal interesse e desejam ser participantes ativos na resolução de problemas. Isto não vai mudar. Nem deveria; se mudar, poderíamos nos tornar menos efetivos nas coisas que fazemos de melhor. 

Nó somos (amplamente) voluntários. Nós tiramos tempo de nossas vidas ocupadas para responder perguntas, e as vezes nós somos sobrecarregados com elas. Então, nós fazemos um filtro impiedoso. Em particular, nós descartamos questões de pessoas que parecem ser perdedores, a fim de gastar nosso tempo de responder perguntas mais eficientemente, com vencedores.

Se você acha esta atidude desagradável, condescendente, ou arrogante, verifique nossas premissas. Não estamos pedindo para você se ajoelhar perante nós - de fato, a maioria de nós não poderia amar nada mais do que lidar com você como um igual e dar lhe boas vindas à nossa cultura, se você dedicar o esforço necessário para tornar isto possível. Mas é simplesmente ineficiente para nós tentar ajudar pessoas que não ajudam a si mesmas. Não há problema em ser ignorante; mas não vale bancar o estúpido.

Então, enquanto não é necessário já ser tecnicamente competente para obter nossa atenção, é necessário demonstrar o tipo de atitude que leva à competência - estar alerta, pensativo, observador, desejando ser um parceiro ativo no desenvolvimento de uma solução. Se você não pode viver com este tipo de discriminação, sugerimos que pague alguém por um contrato de suporte comercial, ao invés de pedir a hackers que pessoalmente lhe doem ajuda.  

Se você decide recorrer a nós por ajuda, você não quer ser um dos perdedores. Você não quer ao menos parecer como um. A melhor forma de obter uma resposta rápida e adequada é perguntar como uma pessoa inteligente, confiante e que tenha pistas sobre a questão, precisando apenas de ajuda em um problema particular.

(Melhorias para este guia são bem vindas. Você pode enviar sugestões para <esr@thyrsus.com> ou <respond-auto@linuxmafia.com>. Observe, no entanto, que este documento não tem a intenção de ser um guia geral para [netiqueta](http://www.ietf.org/rfc/rfc1855.txt), e geralmente iremos rejeitar sugestões que não sejam especificamente relacionadas a elicitar respostas úteis em um fórum técnico.)

<a name="3"></a>

# Antes de perguntar

Antes de fazer uma pergunta técnica por e-mail, em um grupo ou em um website de chat, faça o seguinte:

Tente encontrar a resposta pesquisando no arquivo do forum ou lista de e-mail que você paneja postar a pergunta.

- Tente encontrar uma resposta pesquisando na Web.
- Tente encontrar uma resposta lendo o manual do produto com o qual está tendo problemas.
- Tente encontrar uma resposta lendo uma lista de FAQs (Frequent Asked Questions - Lista de Perguntas Frequentes)
- Tente encontrar uma resposta por inspeção e experimentação.
- Tente encontrar uma resposta perguntando um amigo qualificado.

Se você é um programador, tente encontrar uma resposta lendo o código fonte.

Quando você fizer sua pergunta, mostre que de fato você tentou estas opções antes; isto ajudará a estabelecer que você não é uma esponja preguiçosa
disperdiçando o tempo das pessoas. Melhor ainda, mostre que você tem aprendido por meio de tais tentativas. 
Nós gostamos de responder questões de pessoas que demonstram poderem aprender a partir das respostas.

Use táticas como efetuar uma busca no Google com o texto de qualquer que seja a mensagem de erro que você está obtendo (procure tanto no [Google groups](http://groups.google.com) quanto em páginas Web). Isto pode levá-lo diretamente para a documentação de como corrigir o problema ou para um tópico em uma lista de e-mail com a resposta para a sua questão. Mesmo que você não tenha obtido uma resposta com isto, apenas dizendo "Eu procurei no Google pela seguinta frase mas não obtive nada que se mostrasse promissor" é algo aconselhável a fazer ao postar em uma lista de e-mail ou grupo solicitando ajuda, apenas para registrar que buscas não irão ajudar. Também irá ajudar se você direcionar outras pessoas com problemas similares para o seu tópico, incluindo link para a busca com os termos que esperançosamente apontarão para o tópico com o seu problema e possível solução. 

Leve seu tempo. Não espere ser capaz de resolver um problema complicado com alguns segundos de busca no Google. Leia e entenda as FAQs, sente, relaxe e refleta a respeito do problema antes de abordar especialistas. Confie em nós, eles serão capazes de deduzir a partir das suas perguntas, quanta leitura e raciocínio você exerceu, e irão estar mais dispostos a ajudar se você for preparado. Não dispare instantaneamente seu arsenal de perguntas apenas porque você sua primeira busca resultou em nenhuma resposta (ou respostas demais).

Prepare sua pergunta. Pense sobre ela. Respostas que pareçam precipitadas obtêm respostas precipitadas, ou nenhuma sequer. Quanto mais você demonstra que raciocinou e se esforçou em resolver seu problema antes de procurar ajuda, mais probabilidade você tem de obter ajuda de fato.

Tenha cuidado para não fazer a pergunta errada. Se você fizer uma pergunta baseada em suposições equivocadas, é bastante provável que um [hacker aleatório qualquer](https://en.wikipedia.org/wiki/J._Random_Hacker) responda com uma resposta literal inútil enquanto pensa "Que pergunta estúpida...", e esperando que a experiência de obter o que você pediu e não o que você precisa vai ensiná-lo uma lição.

Nunca assuma que você é elegível para obter uma resposta. Você não é; você não está, no fim das contas, pagando pelo serviço. Você irá ganhar uma resposta, se ganhar, fazendo uma pergunta substancial, interessante e instigante - uma que implicitamente contribua para a experiência da comunidade no lugar de mera e passivamente demandar conhecimento de outros.  

De outra lado, deixando claro que é capaz e deseja ajudar no processo de desenvolvimento da solução é um bom início. Perguntas como "Poderia alguém apontar um caminho?", "O que está faltando no meu exemplo?", e "Qual site eu deveria ter verificado?" são mais prováveis de obterem uma resposta do que "Por favor poste o procedimento exato que eu devo usar.", isto porque você está deixando claro que verdadeiramente deseja completar o processo somente se alguém colocá-lo na direção correta.

<a name="4"></a>

# Quando você perguntar

<a name="4.1"></a>

## Escolha seu fórum cuidadosamente

Tenha atenção ao escolher onde fazer sua pergunta. Você provavelmente será ignorado, ou rotulado como perdedor, se você:

- postar sua questão em um fórum onde ela não se enquada nos tópicos abordados
- postar uma pergunta muito elementar em um fórum onde questões técnicas avançadas são esperadas, ou vice-versa
- espalhar a mesma pergunta por muitos fórums diferentes
- enviar um e-mail pessoal para alguém que não é nem um conhecido seu nem pessoalmente responsável por resolver seu problema

Hackers se livram de perguntas que sejam inapropriadamente direcionadas, a fim de tentar proteger seus canais de comunicação 
de serem afogados por irrelevância. Você não quer que isto lhe aconteça.

O primeiro passo, portanto, é procurar o fórum correto. Novamente, [Google e outros métodos de busca na Web são seus amigos](http://www.giyf.com). 
Use-os para encontrar a página web do projeto mais proximamente relacionado com o hardware ou software com o qual você está tendo dificuldades. Normalmente a página terá links para FAQs (Frequent Asked Questions - Lista de Perguntas Frequentes), e para a lista de e-mail do projeto e seus arquivos. Estas listas de e-mail são o destino final para procurar ajuda, se seus próprios esforços (incluindo a leitura das FAQs que você encontrou) não foram suficientes para chegar a uma solução. A página do projeto pode também descrever os procedimentos de como relatar erros (bugs), ou ter um link para tal documentação; se sim, siga tal procedimento.

Disparar um e-mail para uma pessoa ou fórum que você não é familiarizado é arriscado, para dizer o melhor. Por exemplo, não assuma que o autor de uma página informativa deseja ser seu consultor gratuitamente. Não faça suposições otimistas sobre se sua pergunta será bem vinda - se você não está certo, poste a em outro lugar, ou abstenha-se totalmente de postá-la.

Ao selecionar um fórum Web, um newsgroup ou uma lista de e-mail, não confie apenas no nome de tais grupos; 
procure por uma FAQ ou declaração para verificar se sua questão se enquadra nos tópicos do grupo.
Leia algumas das mensagens anteriores antes de postar, de modo que você sinta como as coisas são feitas lá.
De fato, antes de postar, é uma excelente ideia fazer uma busca no arquivo do fórum, newsgroup ou lista de e-mail 
por palavras-chave relacionadas ao seu problema. Você pode encontrar uma resposta, e se não, isto lhe ajudará
a formular melhor a pergunta.

Não dé um tiro de espingarda em todos os canais de ajuda disponíveis de uma vez só, isto é como gritar e irritar as pessoas. 
Avance por eles suavemente. 

Saiba o que o seu tópico é! Um dos erros clássicos é fazer perguntas sobre interfaces de programação do Unix ou Windows em um fórum 
voltado para uma linguagem, biblioteca ou ferramenta portável para ambos sistemas. Se você não entende porque isto é uma
mancada, é melhor você não fazer pergunta alguma até você entender isto.

Em geral, perguntas postadas em um fórum público bem selecionado tem mais possibilidades de obter respostas úteis do que
perguntas equivalentes em um fórum privado. Existem múltiplas rasões para isto. Uma é simplesmente a quantidade de possíveis
respondentes. Outra é o tamanho da audiência; hackers são mais prováveis de responder questões que ajudam muitas pessoas
no lugar de questões que sirvam a apenas algumas. 

Compreensivamente, hackers habilidosos e autores de softwares populares já recebem mensagens mal direcionadas além da conta. Contribuir para esta enchente, em casos extremos, pode ser a gota d'água - algumas vezes, contribuidores de projetos populares tem retirado o suporte devido a danos colaterais insuportáveis na forma de tráfego inútil de e-mails para suas contas pessoais.

<a name="4.2"></a>

## [Stack Overflow](http://stackoverflow.com)

Procure, então pergunta no Stack Exchange.

Em anos recentes, a comunidade de sites Stack Exchange tem emergido como o maior recurso para responder questões técnicas ou não e é até mesmo o fórum preferido para muitos projetos open-source.

Inicia com uma busca no Google antes de procurar no Stack Exchange; o Google indexa o site em tempo real. Há uma chance muito boa de alguém
já ter feito uma pergunta similar, e os sites Stack Exchange estão frequentemente próximos dos topo dos resultados de busca. 
Se você não encontrou nada por meio do Google, procure novamente no site específico mais relevante para sua questão (veja abaixo). 
Procurar usando tags providas pelo site, pode ajudar a reduzir os resultados.

Se você ainda não encontrou nada, poste sua pergunta no site onde ela seja mais relacionada com os tópicos abordados.
Use as ferramentas de formatação, especialmente para código, e adicione tags que sejam relacionadas ao assunto da sua pergunta
(particularmente o nome da linguagem de programação, sistema operacional ou biblioteca com o a qual você está tendo problemas).
Se alguém lhe pede mais informações, edite seu post principal para incluí-la. Se qualquer resposta é útil, 
clique na seta pra cima para adicionar um voto à resposta; se a resposta provê uma solução para seu problema,
clique na imagem de "check" abaixo das setas de votação para aceitá-las como correta.

Stack Exchange tem crescido para [mais de 100 sites](http://stackexchange.com/sites), mas aqui estão os candidatos mais prováveis:

- [Super User](http://superuser.com) é para questões computação de propósito geral. Se sua questão não é sobre código ou programas com os quais você interage apenas por meio de uma conexão de rede, ela provavelmente vai aqui.
- [Stack Overflow](http://stackoverflow.com) é para questão sobre programação.
- [Server Fault](http://serverfault.com) é para questões sobre servidores e administração de redes.
- Muitos projetos tem seus próprios sites específicos, incluindo [Android](http://android.stackexchange.com), [Ubuntu](http://askubuntu.com), [TeX/LaTeX](http://tex.stackexchange.com), and [Microsoft SharePoint](http://sharepoint.stackexchange.com). Acesse o [Stack Exchange](http://stackexchange.com) para obter uma lista atualizada.

<a name="4.3"></a>

## Fórums Web e IRC

Seu grupo de usuários local, ou sua distribuição Linux, podem fazer propaganda em um fórum Web ou canal IRC onde iniciantes podem obter ajuda
(em países que não falam lingua inglesa, fóruns de iniciantes são ainda mais prováveis de serem listas de e-mail). Estes são primeiros lugares bons para perguntar, especialmente se você pensa possa ter tropeçado em um problema comum e relativamente simples. Um canal IRC promovido por propaganda é um convite aberto a fazer perguntas e frequentemente obter respostas em tempo real.

De fato, se você obteve o programa que está lhe causando problema a partir de uma distribuição Linux (como é comum atualmente), é melhor perguntar no(a)fórum/lista da distribuição antes de tentar o(a) fórum/lista do projeto do programa. Os hackers do projeto podem apenas dizer "use nossa versão". 

Antes de postar em qualquer fórum Web, verifique se ele tem um recurso de busca. Se tem, tente algumas buscas por palavras-chave relacionadas ao seu problema; isto pode realmente ajudar. Se você fez uma busca geral na Web antes (como deveria ter feito), busca no fórum de qualquer forma; o motor de busca Web que usou pode não ter indexado todo o conteúdo do fórum recentemente.  

Existe uma tendência crescente de projetos proverem suporte a usuários por meio de um fórum Web ou canal IRC, com e-mail reservado mais para tráfego de desenvolvimento. Então, olhe estes canais primeiros quando estiver procurando ajuda para projetos específicos. 

Em IRC, é provavelmente melhor não iniciar jogando uma longa descrição de um problema no canal; algumas pessoas interpretam isto como "inundação do canal". É melhor proferir uma descrição de uma linha para o problema, como uma forma de puxar conversa.

<a name="4.4"></a>

## Como um segundo passo, use listas de e-mail de projeto

Quando um projeto tem uma lista de e-mail para desenvolvedores, escreve para tal lista, não pra desenvolvedores individuais, mesmo se você acredita que você sabe quem pode melhor responder sua pergunta. Procure na documentação do projeto e em sua homepage pelo endereço da lista de e-mail, e use-a. Existem muitas boas rasões para este política:

Qualquer pergunta boa o suficiente para ser feita a um desenvolvedor específico também será válida para todo o grupo. Contrariamente, se você suspeita que sua pergunta é muito tola para uma lista de e-mail, isto não é desculpa para molestar desenvolvedores individualmente.

Fazendo perguntas na lista distribui a carga entre os desenvolvedores. Um determinado desenvolvedor (especialmente se ele é o líder do projeto) pode estar muito ocupado para responder suas perguntas.

A maioria das listas de e-mail são arquivadas e os arquivos são indexados pelos motores de busca. Se você fizer sua pergunta na lista e ela for respondida, outra pessoa pode encontrar sua pergunta e a resposta na Web, em vez de perguntar novamente.

Se certas perguntas parecem ser feitas frequentemente, desenvolvedores podem use esta informação para melhorar a documentação ou o próprio software para que ele se torne menos confuso. Mas se estas questões são levantadas de modo privado, ninguém tem uma visão completa de quais perguntas são feitas com mais frequência.

Se o projeto tem tanto uma lista de "usuários" e uma de "desenvolvedores" (ou "hackers") ou um fórum Web e você você não está hackiando o código, pergunte na lista/fórum de "usuários". Não assuma que você irá ser bem vindo na lista de desenvolvedores, onde eles provavelmente vão considerar sua pergunta como ruído quebrando o tráfego de desenvolvimento.

No entanto, se você está certo que sua pergunta não é trivial, e você não obteve respostas na lista/fórum de "usuários" após vários dias, tente a lista de "desenvolvedores". É aconselhável você espreitar lá por alguns dias ou pelo menos verificar os últimos dias de mensagens arquivadas, para se familiarizar com os costumes dos integrantes antes de postar (de fato este é um bom conselho em qualquer lista privada ou semi-privada).

Se você não encontrou uma lista de e-mail do projeto, mas encontrou apenas o endereço do mantenedor do projeto, vá em frente e escreve para ele. Mas mesmo neste caso, não assuma que a lista de e-mail não existe. Mencione no seu e-mail que você procurou e não encontrou uma lista de e-mail. Também mencione que você não não se impõe em sua mensagem ser encaminhada para outras pessoas. (Muitas pessoas acreditam que e-mail privado deveria se manter privado, mesmo que não exista nada secreto nele. Permitindo que sua mensagem seja encaminhada, você dá ao seu correspondente uma escolha sobre como lidar com ela.)

<a name="4.5"></a>

## Use cabeçalhos de assunto significativos e específicos
Em listas de e-mail, newgroups ou fóruns Web, o cabeçalho do assunto é sua oportunidade de ouro para atrair a atenção de especialistas qualificados em cerca de 50 caracteres ou menos. Não desperdice-a balbuciando coisas como "Por favor me ajude" (esqueça "POR FAVOR ME AJUDE!!!"; mensagens com assuntos como este são descartadas por reflexo). Não tente nos impressionar com a profundidade da sua angústia; em vez disso, use o espaço para uma descrição super concisa do problema.

Uma boa conveção para cabeçalhos de assunto, usada por muitas empresas de suporte técnico, é "objeto - desvio". A parte "objeto" especifica que coisa ou grupo de coisas está tendo problema, e a parte "desvio" descreve o desvio do comportamento esperado.

- Estúpido: 
	- AJUDA! Vídeo não funciona corretamente no meu laptop!
- Inteligente: 
	- X.org 6.8.1 deforma o cursor do mouse, chipset de vídeo Fooware MV1005
- Smarter:
	- Cursor do mouse no X.org 6.8.1 sobre chipset de vídeo Fooware MV1005 fica deformado

O processo de escrever uma descrião "objeto-desvio" irá ajudá-lo a organizar seu pensamento sobre o problem em mais detailhes. O que é afetado? Apenas o cursor do mouse ou outros gráficos também? É um problema específico da versão do X.org usada pelo servidor X? Ocorre somente na versão 6.8.1? É um problema específico do chipset de vídeo Fooware? Ocorre somente com o modelo MV1005? Um hacker que vê tal mensagem pode imediatamente entender porque você está problema e qual o problema em si, em um piscar de olhos.

De um modo geral, imagine procurando no índice de um arquivo de perguntas, sendo exibidas apenas as linhas do assunto. Faça o seu cabeçalho de assunto refletir sua pergunta suficientemente bem, de modo que a próxima pessoa, pesquisando o arquivo com uma questão similar à sua, será capaz de seguir a trilha para uma resposta, no lugar de postar a pergunta novamente.

Se você faz uma pergunta em uma resposta, tenha certeza de alterar o cabeçalho do assunto para indicar que você está fazendo uma pergunta. O título do assunto que parece com "Re: teste" ou "Re: novo bug" é menos provável de atrair quantidade útil de atenção. Também, elimine citações de mensagens anteriores para o mínimo necessário para informar leitores posteriores.

Não simplesmente pressione "Responder" em uma mensagem em uma lista de e-mails para iniciar um tópico completamente novo. Isto irá limitar sua audiência. Alguns softwares de leitura de e-mail, como *mutt*, permitem ao usuário ordenar mensagens por tópico e então esconder mensagens dentro de tópicos (normalmente usando um botão + para expandir e - para recolher uma mensagem). Pessoas que fazem isso nunca verão sua mensagem.

Mudar o assunto não é suficiente. O *Mutt*, e provavelmente outros leitores de e-mail, procuram por outras informações nos cabeçalhos do e-mail para atribuí-lo a um tópico, não o título do assunto. Nestes casos portanto, você deve iniciar um e-mail completamente novo.

Em fóruns da Web, as regras de boas práticas são levemente diferentes, devido ao fato de as mensagens serem usualmente muito mais fortemente vinculadas a tópicos de discussão específicos e frequentemente invisíveis fora destes tópicos. Mudar o assunto ao fazer uma pergunta em resposta a outra não é essencial. Nem todos os fóruns permitem assuntos diferentes em respostas, e quase ninguém os lê quando são diferentes. No entanto, fazer uma pergunta em uma resposta é uma prática dúbia por ela mesma, porque a pergunta apenas será vista pelas pessoas que estão observando o tópico. Assim, ao menos que você tenha certeza que deseja questionar apenas as pessoas que atualmente estão ativas no tópico, inicie um novo.

<a name="4.6"></a>

## Torne fácil para responder

Finishing your query with “Please send your reply to... ” makes it quite unlikely you will get an answer. If you can't be bothered to take even the few seconds required to set up a correct Reply-To header in your mail agent, we can't be bothered to take even a few seconds to think about your problem. If your mail program doesn't permit this, [get a better mail program](http://linuxmafia.com/faq/Mail/muas.html). If your operating system doesn't support any e-mail programs that permit this, get a better operating system.

In Web forums, asking for a reply by e-mail is outright rude, unless you believe the information may be sensitive (and somebody will, for some unknown reason, let you but not the whole forum know it). If you want an e-mail copy when somebody replies in the thread, request that the Web forum send it; this feature is supported almost everywhere under options like “watch this thread”, “send e-mail on answers”, etc.

<a name="4.7"></a>

## Escreva em linguagem clara, gramatica e ortograficamente correta

We've found by experience that people who are careless and sloppy writers are usually also careless and sloppy at thinking and coding (often enough to bet on, anyway). Answering questions for careless and sloppy thinkers is not rewarding; we'd rather spend our time elsewhere.

So expressing your question clearly and well is important. If you can't be bothered to do that, we can't be bothered to pay attention. Spend the extra effort to polish your language. It doesn't have to be stiff or formal — in fact, hacker culture values informal, slangy and humorous language used with precision. But it has to be precise; there has to be some indication that you're thinking and paying attention.

Spell, punctuate, and capitalize correctly. Don't confuse “its” with “it's”, “loose” with “lose”, or “discrete” with “discreet”. Don't TYPE IN ALL CAPS; this is read as shouting and considered rude. (All-smalls is only slightly less annoying, as it's difficult to read. Alan Cox can get away with it, but you can't.)

More generally, if you write like a semi-literate boob you will very likely be ignored. So don't use instant-messaging shortcuts. Spelling "you" as "u" makes you look like a semi-literate boob to save two entire keystrokes. Worse: writing like a l33t script kiddie hax0r is the absolute kiss of death and guarantees you will receive nothing but stony silence (or, at best, a heaping helping of scorn and sarcasm) in return.

If you are asking questions in a forum that does not use your native language, you will get a limited amount of slack for spelling and grammar errors — but no extra slack at all for laziness (and yes, we can usually spot that difference). Also, unless you know what your respondent's languages are, write in English. Busy hackers tend to simply flush questions in languages they don't understand, and English is the working language of the Internet. By writing in English you minimize your chances that your question will be discarded unread.

If you are writing in English but it is a second language for you, it is good form to alert potential respondents to potential language difficulties and options for getting around them. Examples:

English is not my native language; please excuse typing errors.

If you speak $LANGUAGE, please e-mail/PM me; I may need assistance translating my question.

I am familiar with the technical terms, but some slang expressions and idioms are difficult for me.

I've posted my question in $LANGUAGE and English. I'll be glad to translate responses, if you only use one or the other.

<a name="4.8"></a>

## Envie questões em formatos acessíveis e padrões

If you make your question artificially hard to read, it is more likely to be passed over in favor of one that isn't. So:

Send plain text mail, not HTML. (It's not hard to [turn off HTML](http://www.birdhouse.org/etc/evilmail.html).)

MIME attachments are usually OK, but only if they are real content (such as an attached source file or patch), and not merely boilerplate generated by your mail client (such as another copy of your message).

Don't send e-mail in which entire paragraphs are single multiply-wrapped lines. (This makes it too difficult to reply to just part of the message.) Assume that your respondents will be reading mail on 80-character-wide text displays and set your line wrap accordingly, to something less than 80.

However, do not wrap data (such as log file dumps or session transcripts) at any fixed column width. Data should be included as-is, so respondents can have confidence that they are seeing what you saw.

Don't send MIME Quoted-Printable encoding to an English-language forum. This encoding can be necessary when you're posting in a language ASCII doesn't cover, but many e-mail agents don't support it. When they break, all those =20 glyphs scattered through the text are ugly and distracting — or may actively sabotage the semantics of your text.

Never, ever expect hackers to be able to read closed proprietary document formats like Microsoft Word or Excel. Most hackers react to these about as well as you would to having a pile of steaming pig manure dumped on your doorstep. Even when they can cope, they resent having to do so.

If you're sending e-mail from a Windows machine, turn off Microsoft's problematic “Smart Quotes” feature (From Tools > AutoCorrect Options, clear the smart quotes checkbox under AutoFormat As You Type.). This is so you'll avoid sprinkling garbage characters through your mail.

In Web forums, do not abuse “smiley” and “HTML” features (when they are present). A smiley or two is usually OK, but colored fancy text tends to make people think you are lame. Seriously overusing smileys and color and fonts will make you come off like a giggly teenage girl, which is not generally a good idea unless you are more interested in sex than answers.

If you're using a graphical-user-interface mail client such as Netscape Messenger, MS Outlook, or their ilk, beware that it may violate these rules when used with its default settings. Most such clients have a menu-based “View Source” command. Use this on something in your sent-mail folder, verifying sending of plain text without unnecessary attached crud.

<a name="4.9"></a>

## Seja preciso e informativo sobre o seu problema

Describe the symptoms of your problem or bug carefully and clearly.

Describe the environment in which it occurs (machine, OS, application, whatever). Provide your vendor's distribution and release level (e.g.: “Fedora Core 7”, “Slackware 9.1”, etc.).

Describe the research you did to try and understand the problem before you asked the question.

Describe the diagnostic steps you took to try and pin down the problem yourself before you asked the question.

Describe any possibly relevant recent changes in your computer or software configuration.

If at all possible, provide a way to reproduce the problem in a controlled environment.

Do the best you can to anticipate the questions a hacker will ask, and answer them in advance in your request for help.

Giving hackers the ability to reproduce the problem in a controlled environment is especially important if you are reporting something you think is a bug in code. When you do this, your odds of getting a useful answer and the speed with which you are likely to get that answer both improve tremendously.

Simon Tatham has written an excellent essay entitled [How to Report Bugs Effectively](http://www.chiark.greenend.org.uk/~sgtatham/bugs.html). I strongly recommend that you read it.

<a name="4.10"></a>

## Volume não é precisão

You need to be precise and informative. This end is not served by simply dumping huge volumes of code or data into a help request. If you have a large, complicated test case that is breaking a program, try to trim it and make it as small as possible.

This is useful for at least three reasons. One: being seen to invest effort in simplifying the question makes it more likely you'll get an answer, Two: simplifying the question makes it more likely you'll get a useful answer. Three: In the process of refining your bug report, you may develop a fix or workaround yourself.

<a name="4.11"></a>

## Não corra para declarar que você encontrou um bug

When you are having problems with a piece of software, don't claim you have found a bug unless you are very, very sure of your ground. Hint: unless you can provide a source-code patch that fixes the problem, or a regression test against a previous version that demonstrates incorrect behavior, you are probably not sure enough. This applies to webpages and documentation, too; if you have found a documentation “bug”, you should supply replacement text and which pages it should go on.

Remember, there are many other users that are not experiencing your problem. Otherwise you would have learned about it while reading the documentation and searching the Web (you did do that before complaining, [didn't you](#3)?). This means that very probably it is you who are doing something wrong, not the software.

The people who wrote the software work very hard to make it work as well as possible. If you claim you have found a bug, you'll be impugning their competence, which may offend some of them even if you are correct. It's especially undiplomatic to yell “bug” in the Subject line.

When asking your question, it is best to write as though you assume you are doing something wrong, even if you are privately pretty sure you have found an actual bug. If there really is a bug, you will hear about it in the answer. Play it so the maintainers will want to apologize to you if the bug is real, rather than so that you will owe them an apology if you have messed up.

<a name="4.12"></a>

## Bajulação não substitui você de fazer seu trabalho de casa

Some people who get that they shouldn't behave rudely or arrogantly, demanding an answer, retreat to the opposite extreme of grovelling. “I know I'm just a pathetic newbie loser, but...”. This is distracting and unhelpful. It's especially annoying when it's coupled with vagueness about the actual problem.

Don't waste your time, or ours, on crude primate politics. Instead, present the background facts and your question as clearly as you can. That is a better way to position yourself than by grovelling.

Sometimes Web forums have separate places for newbie questions. If you feel you do have a newbie question, just go there. But don't grovel there either.

<a name="4.13"></a>

## Descreva os sintomas do problema, não suas suposições

It's not useful to tell hackers what you think is causing your problem. (If your diagnostic theories were such hot stuff, would you be consulting others for help?) So, make sure you're telling them the raw symptoms of what goes wrong, rather than your interpretations and theories. Let them do the interpretation and diagnosis. If you feel it's important to state your guess, clearly label it as such and describe why that answer isn't working for you.

- Stupid:
	I'm getting back-to-back SIG11 errors on kernel compiles, and suspect a hairline crack on one of the motherboard traces. What's the best way to check for those?

- Smart:
	My home-built K6/233 on an FIC-PA2007 motherboard (VIA Apollo VP2 chipset) with 256MB Corsair PC133 SDRAM starts getting frequent SIG11 errors about 20 minutes after power-on during the course of kernel compiles, but never in the first 20 minutes. Rebooting doesn't restart the clock, but powering down overnight does. Swapping out all RAM didn't help. The relevant part of a typical compile session log follows.

Since the preceding point seems to be a tough one for many people to grasp, here's a phrase to remind you: "All diagnosticians are from Missouri." That US state's official motto is "Show me" (earned in 1899, when Congressman Willard D. Vandiver said "I come from a country that raises corn and cotton and cockleburs and Democrats, and frothy eloquence neither convinces nor satisfies me. I'm from Missouri. You've got to show me.") In diagnosticians' case, it's not a matter of skepticism, but rather a literal, functional need to see whatever is as close as possible to the same raw evidence that you see, rather than your surmises and summaries. Show us.

<a name="4.14"></a>

## Descreva os sintomas do seu problema em uma ordem cronológica

The clues most useful in figuring out something that went wrong often lie in the events immediately prior. So, your account should describe precisely what you did, and what the machine and software did, leading up to the blowup. In the case of command-line processes, having a session log (e.g., using the script utility) and quoting the relevant twenty or so lines is very useful.

If the program that blew up on you has diagnostic options (such as -v for verbose), try to select options that will add useful debugging information to the transcript. Remember that more is not necessarily better; try to choose a debug level that will inform rather than drowning the reader in junk.

If your account ends up being long (more than about four paragraphs), it might be useful to succinctly state the problem up top, then follow with the chronological tale. That way, hackers will know what to watch for in reading your account.

<a name="4.15"></a>

## Descreva o objetivo não o passo

If you are trying to find out how to do something (as opposed to reporting a bug), begin by describing the goal. Only then describe the particular step towards it that you are blocked on.

Often, people who need technical help have a high-level goal in mind and get stuck on what they think is one particular path towards the goal. They come for help with the step, but don't realize that the path is wrong. It can take substantial effort to get past this.

- Stupid:
	How do I get the color-picker on the FooDraw program to take a hexadecimal RGB value?

- Smart:
	I'm trying to replace the color table on an image with values of my choosing. Right now the only way I can see to do this is by editing each table slot, but I can't get FooDraw's color picker to take a hexadecimal RGB value.

The second version of the question is smart. It allows an answer that suggests a tool better suited to the task.

<a name="4.16"></a>

## Não peça às pessoas para responderem por e-mail privado

Hackers believe solving problems should be a public, transparent process during which a first try at an answer can and should be corrected if someone more knowledgeable notices that it is incomplete or incorrect. Also, helpers get some of their reward for being respondents from being seen to be competent and knowledgeable by their peers.

When you ask for a private reply, you are disrupting both the process and the reward. Don't do this. It's the respondent's choice whether to reply privately — and if he or she does, it's usually because he or she thinks the question is too ill-formed or obvious to be interesting to others.

There is one limited exception to this rule. If you think the question is such that you are likely to get many answers that are all closely similar, then the magic words are “e-mail me and I'll summarize the answers for the group”. It is courteous to try and save the mailing list or newsgroup a flood of substantially identical postings — but you have to keep the promise to summarize.

<a name="4.17" ></a>

## Seja explícito sobre sua questão

Open-ended questions tend to be perceived as open-ended time sinks. Those people most likely to be able to give you a useful answer are also the busiest people (if only because they take on the most work themselves). People like that are allergic to open-ended time sinks, thus they tend to be allergic to open-ended questions.

You are more likely to get a useful response if you are explicit about what you want respondents to do (provide pointers, send code, check your patch, whatever). This will focus their effort and implicitly put an upper bound on the time and energy a respondent must allocate to helping you. This is good.

To understand the world the experts live in, think of expertise as an abundant resource and time to respond as a scarce one. The less of a time commitment you implicitly ask for, the more likely you are to get an answer from someone really good and really busy.

So it is useful to frame your question to minimize the time commitment required for an expert to field it — but this is often not the same thing as simplifying the question. Thus, for example, “Would you give me a pointer to a good explanation of X?” is usually a smarter question than “Would you explain X, please?”. If you have some malfunctioning code, it is usually smarter to ask for someone to explain what's wrong with it than it is to ask someone to fix it.

<a name="4.18"></a>

## Quando estiver perguntando sobre código

Don't ask others to debug your broken code without giving a hint what sort of problem they should be searching for. Posting a few hundred lines of code, saying "it doesn't work", will get you ignored. Posting a dozen lines of code, saying "after line 7 I was expecting to see <x>, but <y> occurred instead" is much more likely to get you a response.

The most effective way to be precise about a code problem is to provide a minimal bug-demonstrating test case. What's a minimal test case? It's an illustration of the problem; just enough code to exhibit the undesirable behavior and no more. How do you make a minimal test case? If you know what line or section of code is producing the problematic behavior, make a copy of it and add just enough supporting code to produce a complete example (i.e. enough that the source is acceptable to the compiler/interpreter/whatever application processes it). If you can't narrow it down to a particular section, make a copy of the source and start removing chunks that don't affect the problematic behavior. The smaller your minimal test case is, the better (see [the section called “Volume is not precision”](#4.10)).

Generating a really small minimal test case will not always be possible, but trying to is good discipline. It may help you learn what you need to solve the problem on your own — and even when it doesn't, hackers like to see that you have tried. It will make them more cooperative.

If you simply want a code review, say as much up front, and be sure to mention what areas you think might particularly need review and why.

<a name="4.19"></a>

## Não poste perguntas sobre trabalho de casa

Hackers are good at spotting homework questions; most of us have done them ourselves. Those questions are for you to work out, so that you will learn from the experience. It is OK to ask for hints, but not for entire solutions.

If you suspect you have been passed a homework question, but can't solve it anyway, try asking in a user group forum or (as a last resort) in a “user” list/forum of a project. While the hackers will spot it, some of the advanced users may at least give you a hint.

<a name="4.20"></a>

## Elimine perguntas sem sentido

Resist the temptation to close your request for help with semantically-null questions like “Can anyone help me?” or “Is there an answer?” First: if you've written your problem description halfway competently, such tacked-on questions are at best superfluous. Second: because they are superfluous, hackers find them annoying — and are likely to return logically impeccable but dismissive answers like “Yes, you can be helped” and “No, there is no help for you.”

In general, asking yes-or-no questions is a good thing to avoid unless you want a [yes-or-no answer](http://homepage.ntlworld.com./jonathan.deboynepollard/FGA/questions-with-yes-or-no-answers.html).

<a name="4.21"></a>

## Não marque sua questão como “Urgente”, até mesmo se ela é pra você

That's your problem, not ours. Claiming urgency is very likely to be counter-productive: most hackers will simply delete such messages as rude and selfish attempts to elicit immediate and special attention. Furthermore, the word 'Urgent' (and other similar attempts to grab attention in the subject line) often triggers spam filters - your intended recipients might never see it at all!

There is one semi-exception. It can be worth mentioning if you're using the program in some high-profile place, one that the hackers will get excited about; in such a case, if you're under time pressure, and you say so politely, people may get interested enough to answer faster.

This is a very risky thing to do, however, because the hackers' metric for what is exciting probably differs from yours. Posting from the International Space Station would qualify, for example, but posting on behalf of a feel-good charitable or political cause would almost certainly not. In fact, posting “Urgent: Help me save the fuzzy baby seals!” will reliably get you shunned or flamed even by hackers who think fuzzy baby seals are important.

If you find this mysterious, re-read the rest of this how-to repeatedly until you understand it before posting anything at all.

<a name="4.22"></a>

## Cortesia nunca machuca, e algumas vezes ajuda

Be courteous. Use “Please” and “Thanks for your attention” or “Thanks for your consideration”. Make it clear you appreciate the time people spend helping you for free.

To be honest, this isn't as important as (and cannot substitute for) being grammatical, clear, precise and descriptive, avoiding proprietary formats etc.; hackers in general would rather get somewhat brusque but technically sharp bug reports than polite vagueness. (If this puzzles you, remember that we value a question by what it teaches us.)

However, if you've got your technical ducks in a row, politeness does increase your chances of getting a useful answer.

(We must note that the only serious objection we've received from veteran hackers to this HOWTO is with respect to our previous recommendation to use “Thanks in advance”. Some hackers feel this connotes an intention not to thank anybody afterwards. Our recommendation is to either say “Thanks in advance” first and thank respondents afterwards, or express courtesy in a different way, such as by saying “Thanks for your attention” or “Thanks for your consideration”.)

<a name="4.23"></a>

## Prossiga com uma breve nota sobre a solução

Send a note after the problem has been solved to all who helped you; let them know how it came out and thank them again for their help. If the problem attracted general interest in a mailing list or newsgroup, it's appropriate to post the followup there.

Optimally, the reply should be to the thread started by the original question posting, and should have ‘FIXED’, ‘RESOLVED’ or an equally obvious tag in the subject line. On mailing lists with fast turnaround, a potential respondent who sees a thread about “Problem X” ending with “Problem X - FIXED” knows not to waste his/her time even reading the thread (unless (s)he personally finds Problem X interesting) and can therefore use that time solving a different problem.

Your followup doesn't have to be long and involved; a simple “Howdy — it was a failed network cable! Thanks, everyone. - Bill” would be better than nothing. In fact, a short and sweet summary is better than a long dissertation unless the solution has real technical depth. Say what action solved the problem, but you need not replay the whole troubleshooting sequence.

For problems with some depth, it is appropriate to post a summary of the troubleshooting history. Describe your final problem statement. Describe what worked as a solution, and indicate avoidable blind alleys after that. The blind alleys should come after the correct solution and other summary material, rather than turning the follow-up into a detective story. Name the names of people who helped you; you'll make friends that way.

Besides being courteous and informative, this sort of followup will help others searching the archive of the mailing-list/newsgroup/forum to know exactly which solution helped you and thus may also help them.

Last, and not least, this sort of followup helps everybody who assisted feel a satisfying sense of closure about the problem. If you are not a techie or hacker yourself, trust us that this feeling is very important to the gurus and experts you tapped for help. Problem narratives that trail off into unresolved nothingness are frustrating things; hackers itch to see them resolved. The goodwill that scratching that itch earns you will be very, very helpful to you next time you need to pose a question.

Consider how you might be able to prevent others from having the same problem in the future. Ask yourself if a documentation or FAQ patch would help, and if the answer is yes send that patch to the maintainer.

Among hackers, this sort of good followup behavior is actually more important than conventional politeness. It's how you get a reputation for playing well with others, which can be a very valuable asset.

<a name="5"></a>

# Como interpretar respostas

<a name="5.1"></a>

## RTFM e STFW: Como saber que você está seriamente ferrado

There is an ancient and hallowed tradition: if you get a reply that reads “RTFM”, the person who sent it thinks you should have Read The Fucking Manual. He or she is almost certainly right. Go read it.

RTFM has a younger relative. If you get a reply that reads “STFW”, the person who sent it thinks you should have Searched The Fucking Web. He or she is almost certainly right. Go search it. (The milder version of this is when you are told “Google is your friend!”)

In Web forums, you may also be told to search the forum archives. In fact, someone may even be so kind as to provide a pointer to the previous thread where this problem was solved. But do not rely on this consideration; do your archive-searching before asking.

Often, the person telling you to do a search has the manual or the web page with the information you need open, and is looking at it as he or she types. These replies mean that the responder thinks (a) the information you need is easy to find, and (b) you will learn more if you seek out the information than if you have it spoon-fed to you.

You shouldn't be offended by this; by hacker standards, your respondent is showing you a rough kind of respect simply by not ignoring you. You should instead be thankful for this grandmotherly kindness.

<a name="5.2"></a>

## Se você não entendeu...

If you don't understand the answer, do not immediately bounce back a demand for clarification. Use the same tools that you used to try and answer your original question (manuals, FAQs, the Web, skilled friends) to understand the answer. Then, if you still need to ask for clarification, exhibit what you have learned.

For example, suppose I tell you: “It sounds like you've got a stuck zentry; you'll need to clear it.” Then: here's a bad followup question: “What's a zentry?” Here's a good followup question: “OK, I read the man page and zentries are only mentioned under the -z and -p switches. Neither of them says anything about clearing zentries. Is it one of these or am I missing something here?”

<a name="5.3"></a>

## Lidando com grosseria

Much of what looks like rudeness in hacker circles is not intended to give offense. Rather, it's the product of the direct, cut-through-the-bullshit communications style that is natural to people who are more concerned about solving problems than making others feel warm and fuzzy.

When you perceive rudeness, try to react calmly. If someone is really acting out, it is very likely a senior person on the list or newsgroup or forum will call him or her on it. If that doesn't happen and you lose your temper, it is likely that the person you lose it at was behaving within the hacker community's norms and you will be considered at fault. This will hurt your chances of getting the information or help you want.

On the other hand, you will occasionally run across rudeness and posturing that is quite gratuitous. The flip-side of the above is that it is acceptable form to slam real offenders quite hard, dissecting their misbehavior with a sharp verbal scalpel. Be very, very sure of your ground before you try this, however. The line between correcting an incivility and starting a pointless flamewar is thin enough that hackers themselves not infrequently blunder across it; if you are a newbie or an outsider, your chances of avoiding such a blunder are low. If you're after information rather than entertainment, it's better to keep your fingers off the keyboard than to risk this.

(Some people assert that many hackers have a mild form of autism or Asperger's Syndrome, and are actually missing some of the brain circuitry that lubricates “normal” human social interaction. This may or may not be true. If you are not a hacker yourself, it may help you cope with our eccentricities if you think of us as being brain-damaged. Go right ahead. We won't care; we like being whatever it is we are, and generally have a healthy skepticism about clinical labels.)

Jeff Bigler's observations about [tact filters](http://www.mit.edu/~jcb/tact.html) are also relevant and worth reading.

In the next section, we'll talk about a different issue; the kind of “rudeness” you'll see when you misbehave.

<a name="6"></a>

# Não reagindo como um perdedor

Odds are you'll screw up a few times on hacker community forums — in ways detailed in this article, or similar. And you'll be told exactly how you screwed up, possibly with colourful asides. In public.

When this happens, the worst thing you can do is whine about the experience, claim to have been verbally assaulted, demand apologies, scream, hold your breath, threaten lawsuits, complain to people's employers, leave the toilet seat up, etc. Instead, here's what you do:

Get over it. It's normal. In fact, it's healthy and appropriate.

Community standards do not maintain themselves: They're maintained by people actively applying them, visibly, in public. Don't whine that all criticism should have been conveyed via private e-mail: That's not how it works. Nor is it useful to insist you've been personally insulted when someone comments that one of your claims was wrong, or that his views differ. Those are loser attitudes.

There have been hacker forums where, out of some misguided sense of hyper-courtesy, participants are banned from posting any fault-finding with another's posts, and told “Don't say anything if you're unwilling to help the user.” The resulting departure of clueful participants to elsewhere causes them to descend into meaningless babble and become useless as technical forums.

Exaggeratedly “friendly” (in that fashion) or useful: Pick one.

Remember: When that hacker tells you that you've screwed up, and (no matter how gruffly) tells you not to do it again, he's acting out of concern for (1) you and (2) his community. It would be much easier for him to ignore you and filter you out of his life. If you can't manage to be grateful, at least have a little dignity, don't whine, and don't expect to be treated like a fragile doll just because you're a newcomer with a theatrically hypersensitive soul and delusions of entitlement.

Sometimes people will attack you personally, flame without an apparent reason, etc., even if you don't screw up (or have only screwed up in their imagination). In this case, complaining is the way to really screw up.

These flamers are either lamers who don't have a clue but believe themselves to be experts, or would-be psychologists testing whether you'll screw up. The other readers either ignore them, or find ways to deal with them on their own. The flamers' behavior creates problems for themselves, which don't have to concern you.

Don't let yourself be drawn into a flamewar, either. Most flames are best ignored — after you've checked whether they are really flames, not pointers to the ways in which you have screwed up, and not cleverly ciphered answers to your real question (this happens as well).

<a name="7"></a>

# Perguntas que não devem ser feitas

Here are some classic stupid questions, and what hackers are thinking when they don't answer them.

- Q: Where can I find program or resource X?
	- A: The same place I'd find it, fool — at the other end of a web search. Ghod, doesn't everybody know how to use [Google](http://www.google.com) yet?

- Q: How can I use X to do Y?
	- A: If what you want is to do Y, you should ask that question without pre-supposing the use of a method that may not be appropriate. 
	- Questions of this form often indicate a person who is not merely ignorant about X, but confused about what problem Y they are solving and too fixated on the details of their particular situation. It is generally best to ignore such people until they define their problem better.

- Q: How can I configure my shell prompt?
	- A: If you're smart enough to ask this question, you're smart enough to [RTFM](#5.1) and find out yourself.

- Q: Can I convert an AcmeCorp document into a TeX file using the Bass-o-matic file converter?
	- A: Try it and see. If you did that, you'd (a) learn the answer, and (b) stop wasting my time.

- Q: My {program, configuration, SQL statement} doesn't work
	- A: This is not a question, and I'm not interested in playing Twenty Questions to pry your actual question out of you — I have better things to do. 
	
	- On seeing something like this, my reaction is normally of one of the following:
		- do you have anything else to add to that?
		- oh, that's too bad, I hope you get it fixed.
		- and this has exactly what to do with me?

- Q: I'm having problems with my Windows machine. Can you help?
	- A: Yes. Throw out that Microsoft trash and install an open-source operating system like Linux or BSD.
	- Note: you can ask questions related to Windows machines if they are about a program that does have an official Windows build, or interacts with Windows machines (i.e., Samba). Just don't be surprised by the reply that the problem is with Windows and not the program, because Windows is so broken in general that this is very often the case.

- Q: My program doesn't work. I think system facility X is broken.
	- A: While it is possible that you are the first person to notice an obvious deficiency in system calls and libraries heavily used by hundreds or thousands of people, it is rather more likely that you are utterly clueless. Extraordinary claims require extraordinary evidence; when you make a claim like this one, you must back it up with clear and exhaustive documentation of the failure case.

- Q: I'm having problems installing Linux or X. Can you help?
	- A: No. I'd need hands-on access to your machine to troubleshoot this. Go ask your local Linux user group for hands-on help. (You can find a list of user groups [here](http://www.linux.org/groups/index.html).)
	- Note: questions about installing Linux may be appropriate if you're on a forum or mailing list about a particular distribution, and the problem is with that distro; or on local user groups forums. In this case, be sure to describe the exact details of the failure. But do careful searching first, with "linux" and all suspicious pieces of hardware.

- Q: How can I crack root/steal channel-ops privileges/read someone's e-mail?
	- A: You're a lowlife for wanting to do such things and a moron for asking a hacker to help you.

<a name="8"></a>

# Perguntas boas e ruins

Finally, I'm going to illustrate how to ask questions in a smart way by example; pairs of questions about the same problem, one asked in a stupid way and one in a smart way.

- Example 1
	- Stupid: Where can I find out stuff about the Foonly Flurbamatic?
	This question just begs for ["STFW"](#5.1) as a reply.
	- Smart: I used Google to try to find “Foonly Flurbamatic 2600” on the Web, but I got no useful hits. Can I get a pointer to programming information on this device?
	This one has already STFWed, and sounds like there might be a real problem.

- Example 2
	- Stupid: I can't get the code from project foo to compile. Why is it broken?
	The querent assumes that somebody else screwed up. Arrogant git...
	- Smart: The code from project foo doesn't compile under Nulix version 6.2. I've read the FAQ, but it doesn't have anything in it about Nulix-related problems. Here's a transcript of my compilation attempt; is it something I did?
	The querent has specified the environment, read the FAQ, is showing the error, and is not assuming his problems are someone else's fault. This one might be worth some attention.

- Example 3
	- Stupid: I'm having problems with my motherboard. Can anybody help?
	J. Random Hacker's response to this is likely to be “Right. Do you need burping and diapering, too?” followed by a punch of the delete key.
	- Smart: I tried X, Y, and Z on the S2464 motherboard. When that didn't work, I tried A, B, and C. Note the curious symptom when I tried C. Obviously the florbish is grommicking, but the results aren't what one might expect. What are the usual causes of grommicking on Athlon MP motherboards? Anybody got ideas for more tests I can run to pin down the problem?
	This person, on the other hand, seems worthy of an answer. He/she has exhibited problem-solving intelligence rather than passively waiting for an answer to drop from on high.

In the last question, notice the subtle but important difference between demanding “Give me an answer” and “Please help me figure out what additional diagnostics I can run to achieve enlightenment.”

In fact, the form of that last question is closely based on a real incident that happened in August 2001 on the linux-kernel mailing list (lkml). I (Eric) was the one asking the question that time. I was seeing mysterious lockups on a Tyan S2462 motherboard. The list members supplied the critical information I needed to solve them.

By asking the question in the way I did, I gave people something to chew on; I made it easy and attractive for them to get involved. I demonstrated respect for my peers' ability and invited them to consult with me as a peer. I also demonstrated respect for the value of their time by telling them the blind alleys I had already run down.

Afterwards, when I thanked everyone and remarked how well the process had worked, an lkml member observed that he thought it had worked not because I'm a “name” on that list, but because I asked the question in the proper form.

Hackers are in some ways a very ruthless meritocracy; I'm certain he was right, and that if I had behaved like a sponge I would have been flamed or ignored no matter who I was. His suggestion that I write up the whole incident as instruction to others led directly to the composition of this guide.

<a name="9"></a>

# Se você não consegue obter uma resposta

If you can't get an answer, please don't take it personally that we don't feel we can help you. Sometimes the members of the asked group may simply not know the answer. No response is not the same as being ignored, though admittedly it's hard to spot the difference from outside.

In general, simply re-posting your question is a bad idea. This will be seen as pointlessly annoying. Have patience: the person with your answer may be in a different time-zone and asleep. Or it may be that your question wasn't well-formed to begin with.

There are other sources of help you can go to, often sources better adapted to a novice's needs.

There are many online and local user groups who are enthusiasts about the software, even though they may never have written any software themselves. These groups often form so that people can help each other and help new users.

There are also plenty of commercial companies you can contract with for help, both large and small. Don't be dismayed at the idea of having to pay for a bit of help! After all, if your car engine blows a head gasket, chances are you would take it to a repair shop and pay to get it fixed. Even if the software didn't cost you anything, you can't expect that support to always come for free.

For popular software like Linux, there are at least 10,000 users per developer. It's just not possible for one person to handle the support calls from over 10,000 users. Remember that even if you have to pay for support, you are still paying much less than if you had to buy the software as well (and support for closed-source software is usually more expensive and less competent than support for open-source software).

<a name="10"></a>

# Como responder perguntas de uma forma útil

Be gentle. Problem-related stress can make people seem rude or stupid even when they're not.

Reply to a first offender off-line. There is no need of public humiliation for someone who may have made an honest mistake. A real newbie may not know how to search archives or where the FAQ is stored or posted.

If you don't know for sure, say so! A wrong but authoritative-sounding answer is worse than none at all. Don't point anyone down a wrong path simply because it's fun to sound like an expert. Be humble and honest; set a good example for both the querent and your peers.

If you can't help, don't hinder. Don't make jokes about procedures that could trash the user's setup — the poor sap might interpret these as instructions.

Ask probing questions to elicit more details. If you're good at this, the querent will learn something — and so might you. Try to turn the bad question into a good one; remember we were all newbies once.

While muttering RTFM is sometimes justified when replying to someone who is just a lazy slob, a pointer to documentation (even if it's just a suggestion to google for a key phrase) is better.

If you're going to answer the question at all, give good value. Don't suggest kludgy workarounds when somebody is using the wrong tool or approach. Suggest good tools. Reframe the question.

Answer the actual question! If the querent has been so thorough as to do his or her research and has included in the query that X, Y, Z, A, B, and C have already been tried without good result, it is supremely unhelpful to respond with “Try A or B,” or with a link to something that only says, “Try X, Y, Z, A, B, or C.”.

Help your community learn from the question. When you field a good question, ask yourself “How would the relevant documentation or FAQ have to change so that nobody has to answer this again?” Then send a patch to the document maintainer.

If you did research to answer the question, demonstrate your skills rather than writing as though you pulled the answer out of your butt. Answering one good question is like feeding a hungry person one meal, but teaching them research skills by example is showing them how to grow food for a lifetime.

<a name="11"></a>

# Recursos relacionados

If you need instruction in the basics of how personal computers, Unix, and the Internet work, see [The Unix and Internet Fundamentals HOWTO](http://en.tldp.org/HOWTO/Unix-and-Internet-Fundamentals-HOWTO/).

When you release software or write patches for software, try to follow the guidelines in the [Software Release Practice HOWTO](http://en.tldp.org/HOWTO/Software-Release-Practice-HOWTO/index.html).

<a name="12"></a>

# Agradecimentos

Evelyn Mitchell contributed some example stupid questions and inspired the “How To Give A Good Answer” section. Mikhail Ramendik contributed some particularly valuable suggestions for improvements.