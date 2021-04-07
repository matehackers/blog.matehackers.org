---
layout: post
title: Git social?
date: 2015-04-15
tags: ["git","internet","noticias","social","software livre"]
---

Originalmente (seria) publicado na [Igreja Universal do Reino do IURI](http://iuri.tem.blog.br)

> Edição: foi publicado! [iuri.tem.blog.br/posts/git_social](http://iuri.tem.blog.br/posts/git_social)
Mas como a [minha ikiwiki](http://ninguem.tem.blog.br) está com algum erro de configuração, e o assunto vai perder a validade antes que eu consiga computador e internet para arrumar, então vou publicar aqui.

Note que a sintaxe do wordpress é diferente, eu alterei todas as formatações pra dar certo neste blog mas como são muitos links eu não alterei nenhum. Este post foi originalmente foi escrito para ikiwiki em iuri.tem.blog.br e não tem nenhum script que eu possa usar pra converter pro formato do wordpress, ou eu é que sou burro.

É o [Wordpress](http://wordpress.org) (ou o [administrador](https://matehackers.org/quem_somos?rev=1424727431#lucas_fialho_zawacki) do [Mate Blog](http://blog.matehackers.org)) que está errado em não ter [markdown](http://daringfireball.net/projects/markdown/) habilitado, não sou [eu](http://blog.matehackers.org/author/iuri) nem a [Ikiwiki](http://ikiwiki.info).

Eu sei que o [Aaron Swartz](https://pt.wikipedia.org/wiki/Aaron_Swartz) escreveu um [script pra converter markdown pra html](https://github.com/aaronsw/html2text), mas o wordpress não segue regras e padrões, então alguém teria que escrever um script pra converter qualquer coisa pra wordpress. Mas como o wordpress vai mudando em todas as versões sem respeito com outras ferramentas para blogueiros, o que acontece na prática é que todo mundo cria ferramentas para tirar publicações do wordpress e publicar em outros lugares.

Mas hoje eu não vou atacar o wordpress, vou atacar o github e o gitlab. Segue o texto original:

<!--more-->

* * *

# Gitorious morreu!

Com a [morte][a] do [Gitorious][b], agora todo mundo precisa encontrar uma alternativa para hospedar publicamente seus repositórios [git][_c].

> Edição: [Rolf Bjaanes anunciou que os repositórios permanecerão somente leitura][br] graças aos esforços dele e do pessoal do [Archive Team][bs].>
> [br]: http://archiveteam.org/index.php?title=Gitorious>
> [bs]: http://archiveteam.org

# Por que?

Alguém muito bem intencionado vai me perguntar: "-Por quê? Por que é que tu não aproveita a migração *gratuíta* do [Gitorious][b] para o [GitLab][d]? Por que é que tu não usa o [GitHub][e]? Ou a alternativa, que é o [BitBucket][f]? Porquê?"

Não sei se eu usei os porquês direito, mas eu não vou perder tempo respondendo estas perguntas. Os desenvolvedores do [libreboot][g] encarecidamente explicam [porquê não usar Github][h] de forma detalhada e suficiente pra convencer qualquer teimoso que defende serviços comerciais. Quem não está disposto a ser convencida(o) tem a mente fechada e não merece a minha dedicação.

Os mesmos desenvolvedores também explicam [porquê não usar Gitorious][i]. Escreveram isto recentemente, depois do [incidente de março][a]. Palmas pra eles e quem ainda acha que opções comerciais são soluções que leia e se aprofunde.

# Mas e a tua opinião?

## Liberdade é um conceito filosófico e político

A primeira coisa que tem que ficar clara é que se o teu conceito de liberdade presume que um código escrito tenha que permanecer "livre" para que outras pessoas possam fazer o **que quiserem** com ele, então nosso conceito de liberdade é diferente.

Eu sou *[[!wikipedia pt:Esquerda_pol%C3%ADtica desc="de esquerda"]]*. Eu sou *[[!wikipedia pt:copyleft desc="copyleft"]]*. Eu sou *[GNU][l]*. Eu sou *[FSF][m]*. Alias, corrigindo em tempo, eu não sou de *[[!wikipedia pt:Esquerda_pol%C3%ADtica desc="esquerda"]]*. Eu sou de _**[[!wikipedia pt:Extrema-esquerda desc="extrema-esquerda"]]**_.

Se tu entende que "liberdade" significa, entre outras coisas, dar "liberdade" para as pessoas usarem trabalhos, construções para monopolizar o controle dos meios de produção, então tu é [[!wikipedia pt:Liberalismo desc="neo liberal"]]. Eu sou [[!wikipedia pt:Socialismo_libertário desc="libertário de esquerda"]] [[!wikipedia pt:Anticapitalismo desc="anticapitalista"]].

[_copyleft segundo a Free Software Foundation][n] é mais que uma licença, é uma consolidação filosófica e uma subversão do conceito de direito autoral para boicotar a propriedade intelectual privada. É um ato de resistência que promoveu a inversão dos papéis pelo menos dentro do escopo da tecnologia da informação. Hoje quem decide fechar código e tornar as coisas proprietárias, e investir em valor de mercado dos softwares são mau vistos, marginalizados e tido como pessoas/organizações que prejudicam a comunidade que usa e desenvolve software, e a sociedade de forma geral.

Há quem critique a [filosofia GNU][o] argumentando que as [licenças da GNU][p] não são "realmente livres". Mas estas pessoas simplesmente têm [outra visão sobre liberdade][q], embora normalmente não admitam que têm posições políticas divergentes. Mas é o que a galera da [[!wikipedia pt:Direita_pol%C3%ADtica desc="direita"]] e do [[!wikipedia pt:Mercado_livre desc="livre mercado"]] sempre diz, que não têm opiniões políticas, quando em verdade o que eles têm é intolerância ao diálogo com gente da [[!wikipedia pt:Esquerda_pol%C3%ADtica desc="esquerda"]] que nem eu, por acharem que suas opiniões representam a elucidação do óbvio, e não o "lado do muro" que eles escolhem.

## Liberdade de expressão não é anarco capitalismo

A menos que o [_código fonte do Gitorious][r] - o [software][r], não a [empresa][s] - siga sendo mantido pela comunidade e utilizado de forma livre (segundo o [_conceito pragmático do Stallman][t]), então apoiar o [Gitorious][b] hoje significa apoiar o [GitLab][d] e suas [soluções empresariais de código fechado][u]. E não era isto que o [Gitorious][b] vinha fazendo, a começar pela licença copyleft [Affero GPL][v], que com esta confusão eu tive a oportunidade de [estudar mais minunciosamente][w] e pretendo utilizá-la mais daqui pra frente, já que para o tipo de coisa que eu faço esta licença é mais indicada que a [GPL normal][x].

Outra coisa é que quem historicamente promoveu o uso do [Gitorious][b] acabou no fim das contas incentivando as pessoas a usarem um [serviço comercial de código fechado][u], em decorrência da tática comercial que foi parte do [acordo entre Gitorious e GitLab][y]: eles botam um aviso no [site][b] dando a entender que o caminho mais fácil, rápido e seguro é migrar "automaticamente" os repositórios que agora estão no Gitorious para o GitLab. "*Sem custos*". Ao invés de fazer o **certo**, que é [promover a crítica construtiva][z], como faz a galera do [Peers Community][aa] e [apresentar possíveis alternativas][ab], como fez [Jason Self][ac].

## "*Sem custos*" é o caralho.

A quantidade de softwares livre que atendem às regras rigorosoas do [projeto GNU][ad] e que terão que mover seus repositórios para serviços de hospedagem git públicos livres é grande. E isto nem é um problema. O problema real é a enorme quantidade de instâncias, ou "clones" dos respositórios que se beneficiam da centralização do código no [site do Gitorious][b].

## **PS:** Centalização?

Sim, a centralização sempre é ruim, mas uma aplicação prática da centralização é ter um [[!wikipedia pt:URL desc="URL"]] que possa ser usado como [remote][ae] "oficial" do código de algum sofware, com a intenção de garantir que o esforço de todo mundo que contribui com o código seja consolidado. Este é um dos objetivos de se usar um sistema como o [git][_c].

Se não fossem estes métodos de organização, então cada pessoa teria que desenvolver sozinha seu próprio software, e aí não haveria justificativa para empreender esforços com colaboratividade em primeiro lugar, e eu não estaria escrevendo nada disto.

A própria tecnologia do [git][_c] permite manter o código fonte de um software descentralizado e adicionar mais de um remote no código, mas esta prática não é comum. Talvez com o [incidente com o Gitorious][a] que motivou esta publicação as(os) desenvolvedoras(es) de software livre comecem a adotar práticas melhores de programação.

## Exemplos?

Vejamos o exemplo da [Lorea][af], que é uma rede social descentralizada baseada no conceito de sementes. A maioria das sementes, como as que eu administro que são a [Rede dxs de Baixo][ag] e a [Lorea Independência][ah], a primeira semente, [N-1][ai], a semente principal [Anillosur][aj], e ainda as sementes [Ecoxarxes][ak], [_coolmeia][al], entre outras, usam o [repositório principal][am] do [Lorea][af].

A semente que eu sou moderador, a [Saravea][an] usa seu [próprio repositório][ao], o que é o mais seguro possível e satisfaz todas as premissas de um software totalmente livre. Isto só traz um único problema, toda vez que [_cai o site][ap] do [Saravá][aq], cai o [Saravea][an] e o [repositório][ao] junto. Contanto que pelo menos uma pessoa tenha clonado, já é o suficiente pra botar o serviço de volta no ar novamente.

Mas no caso das sementes que se atualizam a partir do único [remote][ae] que é no [Gitorious][b], só avisando todos os administradores **antes** da data limite para o [site do gitorious.org][b] sair do ar.

# O que fazer então?

Se o software que tu hospeda no teu servidor tem uma única linha contendo algo com *gitorious.org* quando tu digita isto no diretório base:

git remote --v

Então tu tem que tomar uma atitude. Tem que descobrir pra onde vai o código do software que tu usa, e se a organização que botou o código no [gitorious.org][b] está preocupada com isto.

Além da [Lorea Independência][ah], outro sistema do [Hacklab Independência][ar] que será afetado é a [instância][as] [Mediagoblin][at] da [Mídia Capoeira][au]. Porque o [_código do Mediagoblin][av] está no [gitorious.org][b].

# E agora, vamos pra onde?

Sim, temos que ser sociais. E usar o [Github][e] ou qualquer alternativa comercial é inaceitável não só ponto de vista ideológico, mas do ponto de vista da existência de projetos de software livre. Como é que um serviço que [se declara facilitador do compartilhamento de código][aw] fica [_confabulando sobre abrir ou não abrir o código][q]?

Então é necessário sim pensar em alternativas. Se todo mundo fosse hospedar "em casa" os seus repositórios, precisaríamos de outros serviços importantes como *[wikis][ax]*, *[bug trackers][ay]*, *[issue trackers][ay]* e outras coisas que a maioria que ta lendo isto e conhece os termos deve saber só como funciona no [Github][e] e em lugar nenhum além disto.

Não é todo mundo que consegue colaboração e comprometimento de muita gente desta forma. É mais fácil morrer sozinho com um projeto "puro" do que conseguir participação com comprometimento desta forma.

É importante fazer um "paênteses" aqui pra dizer que eu não sou a favor de participação a qualquer custo. Participação sem comprometimento é nociva. A qualidade do teu projeto não é diretamente proporcional ao seu número de "watches", "forks", "likes" ou qualquer outro método de quantificação que os ególatras gostam de ver. Talvez na maioria das vezes o número de commits pode estar relacionado com a qualidade do teu código, mas isto não deve ser tomado como regra porque há quem estabeleça a política de poucos commits "grandes" ou muitos commits "pequenos".

## Ta, e vamos pra onde afinal? Até agora só enrolação!

Sim, eu sei que quem fica lendo muito acaba perdendo a paciência e quer logo uma solução. Mas a solução imediata já foi dada no próprio [site do gitorious][b]. Migra pro [Gitlab][d] que está comprando a [Gitorious][s]. Simples assim. Se tu não tem tempo pra ler, se informar, avaliar, tu tem que ser refém de quem tem recursos, dinheiro e expertise pra te obrigar a fazer as coisas de uma forma que lhes dê lucro ou outro tipo de benefício. É assim que funciona. Ou tu usa o teu cérebro ou vão te usar.

Dito isto, as duas iniciativas promissoras que eu consegui encontrar são o [GitBull][az] e o [Not a Bug][ba].

### GitBull

[Aparentemente][bb] esta é uma iniciativa *libre*, ou seja, comprometida com a [filosofia GNU][o]. O software que eles utilizam é o [Kallithea][bc], que também é *libre* e parece minimalista e bonito. Entretanto, aparentemente ainda não tem as coisas bonitas e convenientes que tem nos serviços comerciais, como *[issue tracker][ay]*, por exemplo.

Preliminarmente analisando me parece tão bom ou melhor que o [Gitorious][b], e mesmo que o serviço [GitBull][az] não permaneça *libre* e siga o caminho do [Gitorious][b], o software que o [GitBull][az] usa, o [Kallithea][bc], permanecerá *libre* e a [Software Freedom Conservancy][bd] vai continuar mantendo o código.

### Not a Bug

[Not a Bug][ba] é muito mais parecido com o famigerado [Github][e], e o motivo disto é que o software utilizado é uma [versão modificada][be] do [Gogs][bf].

[Gogs][bf] é um software livre com licença permissiva ([MIT][bg], do jeito que os marketeiros do [Github][e] e [Gitlab][d] gostam), de código aberto, e seu desenvolvimento é bem comercial. Inclusive o [_código fonte][bh] dele está no [Github][e], e eles usam os serviços comerciais paralelos do [Github][e], como por exemplo o [Gitter][bi]. Isto beneficia todo mundo, inclusive é possível fazer um *[fork][bj]* deste código e licenciar o software sob alguma licença [_copyleft][n]. É possível inclusive fechar o código e fazer um *[fork][bj]* alterado para um serviço comercial com código proprietário.

No caso do [Not a Bug][ba], eles estão usando o [Gogs][bf] com a mesma licença. O resultado é um site pronto pra uso com uma aparência semelhante à do [Github][e].

Este é um projeto da [Peers Community][bk], que [diz que é uma iniciativa livre][aa].

### Hacklab Independência?

Claro, provavalmente [eu][bl] que tenho mania de instalar tudo o que eu acho legal nos [servidores][bm] do [Hacklab Independência][ar], vou tentar um destes dois softwares ([Kallithea][bc] e [Gogs][bf]) provavelmente em *git.hi.ato.br*.

Também vou sugerir para o administrador do site do [Matehackers][bn] que instale o [Gogs][bf] em um subdomínio tipo *git.matehackers.org* para incentivar o maior uso do site próprio e menor uso do [repositório][bo] do [Matehackers][bn] no [Github][e].

Porque pra quem não sabe, este que está escrevendo usa o [Github][e] junto com o [Matehackers][bo] e mesmo junto com o [Hacklab Independência][bp]. Eu tenho [perfil][bq] no [Github][e] e tudo. Então eu também tenho que tomar vergonha na cara e seguir o meu conselho.

[a]: https://about.gitlab.com/2015/03/03/gitlab-acquires-gitorious/
[b]: https://gitorious.org
[_c]: http://git-scm.com
[d]: https://gitlab.com
[e]: https://github.com
[f]: https://bitbucket.com
[g]: http://libreboot.org
[h]: http://www.libreboot.org/github/
[i]: http://www.libreboot.org/gitorious/
[j]: http://jxself.org/goodbye-gitorious.shtml
[k]: https://pt.wikipedia.org/wiki/Esquerda_pol%C3%ADtica
[l]: http://gnu.org
[m]: http://fsf.org
[n]: https://www.gnu.org/copyleft/copyleft.html
[o]: https://www.gnu.org/philosophy/philosophy.html
[p]: https://www.gnu.org/licenses/licenses.html
[q]: http://tom.preston-werner.com/2011/11/22/open-source-everything.html
[r]: https://gitorious.org/gitorious
[s]: http://www.gitorious.com/about
[t]: http://www.gnu.org/philosophy/pragmatic.html
[u]: https://about.gitlab.com/pricing/
[v]: http://www.gnu.org/licenses/agpl.html
[w]: http://www.gnu.org/licenses/why-affero-gpl.html
[x]: http://www.gnu.org/licenses/gpl.html
[y]: http://thenextweb.com/insider/2015/03/03/gitlab-acquires-rival-gitorious-will-shut-june-1/
[z]: http://freepo.st/community/NotABug.org
[aa]: http://peers.community/#about
[ab]: http://jxself.org/goodbye-gitorious.shtml
[ac]: http://jxself.org/about.shtml
[ad]: http://www.gnu.org/gnu/manifesto.html
[ae]: http://git-scm.com/book/en/v2/Git-Branching-Remote-Branches
[af]: https://lorea.org
[ag]: https://baixo.de/
[ah]: https://lorea.hi.ato.br/
[ai]: https://n-1.cc/
[aj]: https://red.anillosur.net/
[ak]: https://cooperativa.ecoxarxes.cat/
[al]: https://net.coolmeia.org/
[am]: https://gitorious.org/lorea
[an]: https://saravea.org
[ao]: https://git.sarava.org/?a=project_list;pf=lorea
[ap]: https://www.sarava.org/pt-br/content/servidor-do-sarav%C3%A1-tem-seus-discos-r%C3%ADgidos-apreendidos-para-investiga%C3%A7%C3%A3o-por-representante-d
[aq]: https://www.sarava.org
[ar]: https://hi.ato.br
[as]: https://capoeira.li/midia
[at]: https://mediagoblin.org
[au]: https://capoeira.li
[av]: https://gitorious.org/mediagoblin
[aw]: https://github.com/about
[ax]: https://hi.ato.br/wiki
[ay]: https://trac.hi.ato.br
[az]: https://gitbull.org/
[ba]: https://notabug.org
[bb]: https://gitbull.org/#about
[bc]: https://kallithea-scm.org/
[bd]: https://sfconservancy.org/
[be]: https://notabug.org/hp/gogs/
[bf]: http://gogs.io/
[bg]: http://opensource.org/licenses/MIT
[bh]: https://github.com/gogits/gogs/
[bi]: https://gitter.im/gogits/gogs
[bj]: https://help.github.com/articles/fork-a-repo/
[bk]: http://peers.community
[bl]: /autor/iuri/
[bm]: https://hi.ato.br/servidores
[bn]: http://matehackers.org
[bo]: https://github.com/matehackers
[bq]: https://github.com/hiatobr
