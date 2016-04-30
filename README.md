# Como Fazer Perguntas de Maneira Inteligente
---------------------------------------------

[Tradução baseada na revisão 3.10 da versão original em inglês de 21 Maio de 2014](http://www.catb.org/~esr/faqs/smart-questions.html)
--------------------------------------------------------------------------------------------------------------------------------------

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
	- [Web e fórums IRC](#4.3)
	- [Como um segundo passo, use listas de email de projeto](#4.4)
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

Tente encontrar a resposta pesquisando no arquivo do forum ou lista de email que você paneja postar a pergunta.

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

Tenha cuidado para não fazer a pergunta errada. Se você fizer uma pergunta baseada em suposições equivocadas, é bastante provável que um ["J. Random Hacker"](https://en.wikipedia.org/wiki/J._Random_Hacker) responda com uma resposta literal inútil enquanto pensa "Que pergunta estúpida...", e esperando que a experiência de obter o que você pediu e não o que você precisa vai ensiná-lo uma lição.

Nunca assuma que você é elegível para obter uma resposta. Você não é; você não está, no fim das contas, pagando pelo serviço. Você irá ganhar uma resposta, se ganhar, fazendo uma pergunta substancial, interessante e instigante - uma que implicitamente contribua para a experiência da comunidade no lugar de mera e passivamente demandar conhecimento de outros.  

De outra lado, deixando claro que é capaz e deseja ajudar no processo de desenvolvimento da solução é um bom início. Perguntas como "Poderia alguém apontar um caminho?", "O que está faltando no meu exemplo?", e "Qual site eu deveria ter verificado?" são mais prováveis de obterem uma resposta do que "Por favor poste o procedimento exato que eu devo usar.", isto porque você está deixando claro que verdadeiramente deseja completar o processo somente se alguém colocá-lo na direção correta.

<a name="4"></a>
# Quando você perguntar

<a name="4.1"></a>
## Escolha seu fórum cuidadosamente

Be sensitive in choosing where you ask your question. You are likely to be ignored, or written off as a loser, if you:

post your question to a forum where it's off topic

post a very elementary question to a forum where advanced technical questions are expected, or vice-versa

cross-post to too many different newsgroups

post a personal e-mail to somebody who is neither an acquaintance of yours nor personally responsible for solving your problem

Hackers blow off questions that are inappropriately targeted in order to try to protect their communications channels from being drowned in irrelevance. You don't want this to happen to you.

The first step, therefore, is to find the right forum. Again, Google and other Web-searching methods are your friend. Use them to find the project webpage most closely associated with the hardware or software giving you difficulties. Usually it will have links to a FAQ (Frequently Asked Questions) list, and to project mailing lists and their archives. These mailing lists are the final places to go for help, if your own efforts (including reading those FAQs you found) do not find you a solution. The project page may also describe a bug-reporting procedure, or have a link to one; if so, follow it.

Shooting off an e-mail to a person or forum which you are not familiar with is risky at best. For example, do not assume that the author of an informative webpage wants to be your free consultant. Do not make optimistic guesses about whether your question will be welcome — if you're unsure, send it elsewhere, or refrain from sending it at all.

When selecting a Web forum, newsgroup or mailing list, don't trust the name by itself too far; look for a FAQ or charter to verify your question is on-topic. Read some of the back traffic before posting so you'll get a feel for how things are done there. In fact, it's a very good idea to do a keyword search for words relating to your problem on the newsgroup or mailing list archives before you post. It may find you an answer, and if not it will help you formulate a better question.

Don't shotgun-blast all the available help channels at once, that's like yelling and irritates people. Step through them softly.

Know what your topic is! One of the classic mistakes is asking questions about the Unix or Windows programming interface in a forum devoted to a language or library or tool portable across both. If you don't understand why this is a blunder, you'd be best off not asking any questions at all until you get it.

In general, questions to a well-selected public forum are more likely to get useful answers than equivalent questions to a private one. There are multiple reasons for this. One is simply the size of the pool of potential respondents. Another is the size of the audience; hackers would rather answer questions that educate many people than questions serving only a few.

Understandably, skilled hackers and authors of popular software are already receiving more than their fair share of mis-targeted messages. By adding to the flood, you could in extreme cases even be the straw that breaks the camel's back — quite a few times, contributors to popular projects have withdrawn their support because collateral damage in the form of useless e-mail traffic to their personal accounts became unbearable.

<a name="4.2"></a>
## [Stack Overflow](http://stackoverflow.com)

Search, then ask on Stack Exchange

In recent years, the Stack Exchange community of sites has emerged as a major resource for answering technical and other questions and is even the preferred forum for many open-source projects.

Start with a Google search before looking at Stack Exchange; Google indexes it in real time. There's a very good chance someone has already asked a similar question, and the Stack Exchange sites are often near the top of the search results. If you didn't find anything through Google, search again on the specific site most relevant to your question (see below). Searching with tags can help narrow down the results.

If you still didn't find anything, post your question on the one site where it's most on-topic. Use the formatting tools, especially for code, and add tags that are related to the substance of your question (particularly the name of the programming language, operating system, or library you're having trouble with). If a commenter asks you for more information, edit your main post to include it. If any answer is helpful, click the up arrow to upvote it; if an answer gives a solution to your problem, click the check under the voting arrows to accept it as correct.

Stack Exchange has grown to [over 100 sites](http://stackexchange.com/sites), but here are the most likely candidates:

Super User is for questions about general-purpose computing. If your question isn't about code or programs that you talk to only over a network connection, it probably goes here.

Stack Overflow is for questions about programming.

Server Fault is for questions about server and network administration.

Several projects have their own specific sites, including Android, Ubuntu, TeX/LaTeX, and SharePoint. Check the Stack Exchange site for an up-to-date list.

<a name="4.3"></a>
## Web e fórums IRC

Your local user group, or your Linux distribution, may advertise a Web forum or IRC channel where newbies can get help. (In non-English-speaking countries newbie forums are still more likely to be mailing lists.) These are good first places to ask, especially if you think you may have tripped over a relatively simple or common problem. An advertised IRC channel is an open invitation to ask questions there and often get answers in real time.

In fact, if you got the program that is giving you problems from a Linux distribution (as is common today), it may be better to ask in the distro's forum/list before trying the program's project forum/list. The project's hackers may just say, “use our build”.

Before posting to any Web forum, check if it has a Search feature. If it does, try a couple of keyword searches for something like your problem; it just might help. If you did a general Web search before (as you should have), search the forum anyway; your Web-wide search engine might not have all of this forum indexed recently.

There is an increasing tendency for projects to do user support over a Web forum or IRC channel, with e-mail reserved more for development traffic. So look for those channels first when seeking project-specific help.

In IRC, it's probably best not to dump a long problem description on the channel first thing; some people interpret this as channel-flooding. Best to utter a one-line problem description in a way pitched to start a conversation on the channel.

<a name="4.4"></a>
## Como um segundo passo, use listas de email de projeto

When a project has a development mailing list, write to the mailing list, not to individual developers, even if you believe you know who can best answer your question. Check the documentation of the project and its homepage for the address of a project mailing list, and use it. There are several good reasons for this policy:

Any question good enough to be asked of one developer will also be of value to the whole group. Contrariwise, if you suspect your question is too dumb for a mailing list, it's not an excuse to harass individual developers.

Asking questions on the list distributes load among developers. The individual developer (especially if he's the project leader) may be too busy to answer your questions.

Most mailing lists are archived and the archives are indexed by search engines. If you ask your question on-list and it is answered, a future querent could find your question and the answer on the Web instead of asking it again.

If certain questions are seen to be asked often, developers can use that information to improve the documentation or the software itself to be less confusing. But if those questions are asked in private, nobody has the complete picture of what questions are asked most often.

If a project has both a “user” and a “developer” (or “hacker”) mailing list or Web forum, and you are not hacking on the code, ask in the “user” list/forum. Do not assume that you will be welcome on the developer list, where they're likely to experience your question as noise disrupting their developer traffic.

However, if you are sure your question is non-trivial, and you get no answer in the “user” list/forum for several days, try the “developer” one. You would be well advised to lurk there for a few daysor at least review the last few days of archived messages, to learn the local folkways before posting (actually this is good advice on any private or semi-private list).

If you cannot find a project's mailing list address, but only see the address of the maintainer of the project, go ahead and write to the maintainer. But even in that case, don't assume that the mailing list doesn't exist. Mention in your e-mail that you tried and could not find the appropriate mailing list. Also mention that you don't object to having your message forwarded to other people. (Many people believe that private e-mail should remain private, even if there is nothing secret in it. By allowing your message to be forwarded you give your correspondent a choice about how to handle your e-mail.)

<a name="4.5"></a>
## Use cabeçalhos de assunto significativos e específicos

On mailing lists, newsgroups or Web forums, the subject header is your golden opportunity to attract qualified experts' attention in around 50 characters or fewer. Don't waste it on babble like “Please help me” (let alone “PLEASE HELP ME!!!!”; messages with subjects like that get discarded by reflex). Don't try to impress us with the depth of your anguish; use the space for a super-concise problem description instead.

One good convention for subject headers, used by many tech support organizations, is “object - deviation”. The “object” part specifies what thing or group of things is having a problem, and the “deviation” part describes the deviation from expected behavior.

- Stupid: 
	- HELP! Video doesn't work properly on my laptop!
- Smart: 
	- X.org 6.8.1 misshapen mouse cursor, Fooware MV1005 vid. chipset
- Smarter:
	- X.org 6.8.1 mouse cursor on Fooware MV1005 vid. chipset - is misshapen

The process of writing an “object-deviation” description will help you organize your thinking about the problem in more detail. What is affected? Just the mouse cursor or other graphics too? Is this specific to the X.org version of X? To version 6.8.1? Is this specific to Fooware video chipsets? To model MV1005? A hacker who sees the result can immediately understand what it is that you are having a problem with and the problem you are having, at a glance.

More generally, imagine looking at the index of an archive of questions, with just the subject lines showing. Make your subject line reflect your question well enough that the next person searching the archive with a question similar to yours will be able to follow the thread to an answer rather than posting the question again.

If you ask a question in a reply, be sure to change the subject line to indicate that you're asking a question. A Subject line that looks like “Re: test” or “Re: new bug” is less likely to attract useful amounts of attention. Also, pare quotation of previous messages to the minimum consistent with cluing in new readers.

Do not simply hit reply to a list message in order to start an entirely new thread. This will limit your audience. Some mail readers, like mutt, allow the user to sort by thread and then hide messages in a thread by folding the thread. Folks who do that will never see your message.

Changing the subject is not sufficient. Mutt, and probably other mail readers, looks at other information in the e-mail's headers to assign it to a thread, not the subject line. Instead start an entirely new e-mail.

On Web forums the rules of good practice are slightly different, because messages are usually much more tightly bound to specific discussion threads and often invisible outside those threads. Changing the subject when asking a question in reply is not essential. Not all forums even allow separate subject lines on replies, and nearly nobody reads them when they do. However, asking a question in a reply is a dubious practice in itself, because it will only be seen by those who are watching this thread. So, unless you are sure you want to ask only the people currently active in the thread, start a new one.

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

If you speak $LANGUAGE, please email/PM me; I may need assistance translating my question.

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
	
	Questions of this form often indicate a person who is not merely ignorant about X, but confused about what problem Y they are solving and too fixated on the details of their particular situation. It is generally best to ignore such people until they define their problem better.

- Q: How can I configure my shell prompt?
	- A: If you're smart enough to ask this question, you're smart enough to [RTFM](#5.1) and find out yourself.

- Q: Can I convert an AcmeCorp document into a TeX file using the Bass-o-matic file converter?
	- A: Try it and see. If you did that, you'd (a) learn the answer, and (b) stop wasting my time.

- Q: My {program, configuration, SQL statement} doesn't work
	- A: This is not a question, and I'm not interested in playing Twenty Questions to pry your actual question out of you — I have better things to do. 
	
	On seeing something like this, my reaction is normally of one of the following:
		- do you have anything else to add to that?
		- oh, that's too bad, I hope you get it fixed.
		- and this has exactly what to do with me?

- Q: I'm having problems with my Windows machine. Can you help?
	- A: Yes. Throw out that Microsoft trash and install an open-source operating system like Linux or BSD.
	
	Note: you can ask questions related to Windows machines if they are about a program that does have an official Windows build, or interacts with Windows machines (i.e., Samba). Just don't be surprised by the reply that the problem is with Windows and not the program, because Windows is so broken in general that this is very often the case.


- Q: My program doesn't work. I think system facility X is broken.
	- A: While it is possible that you are the first person to notice an obvious deficiency in system calls and libraries heavily used by hundreds or thousands of people, it is rather more likely that you are utterly clueless. Extraordinary claims require extraordinary evidence; when you make a claim like this one, you must back it up with clear and exhaustive documentation of the failure case.

- Q: I'm having problems installing Linux or X. Can you help?
	- A: No. I'd need hands-on access to your machine to troubleshoot this. Go ask your local Linux user group for hands-on help. (You can find a list of user groups [here](http://www.linux.org/groups/index.html).)

	Note: questions about installing Linux may be appropriate if you're on a forum or mailing list about a particular distribution, and the problem is with that distro; or on local user groups forums. In this case, be sure to describe the exact details of the failure. But do careful searching first, with "linux" and all suspicious pieces of hardware.

- Q: How can I crack root/steal channel-ops privileges/read someone's e-mail?
	- A: You're a lowlife for wanting to do such things and a moron for asking a hacker to help you.

<a name="8"></a>
# Perguntas boas e ruins

Finally, I'm going to illustrate how to ask questions in a smart way by example; pairs of questions about the same problem, one asked in a stupid way and one in a smart way.

- Stupid: Where can I find out stuff about the Foonly Flurbamatic?
This question just begs for ["STFW"](#5.1) as a reply.

- Smart: I used Google to try to find “Foonly Flurbamatic 2600” on the Web, but I got no useful hits. Can I get a pointer to programming information on this device?
This one has already STFWed, and sounds like there might be a real problem.


- Stupid: I can't get the code from project foo to compile. Why is it broken?
The querent assumes that somebody else screwed up. Arrogant git...

- Smart: The code from project foo doesn't compile under Nulix version 6.2. I've read the FAQ, but it doesn't have anything in it about Nulix-related problems. Here's a transcript of my compilation attempt; is it something I did?
The querent has specified the environment, read the FAQ, is showing the error, and is not assuming his problems are someone else's fault. This one might be worth some attention.


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