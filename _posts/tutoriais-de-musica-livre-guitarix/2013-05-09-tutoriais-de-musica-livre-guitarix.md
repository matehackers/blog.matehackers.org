---
layout: post
title: Tutoriais de Música Livre – Guitarix
date: 2013-05-09
tags: ["guitarix","guitarra","jack","linux","livre","musica","software livre","software-musica"]
---

No artigo [Linux e o Guitarrista Pobre](http://blog.lfzawacki.com/linux-guitarrista-pobre/) eu introduzi as tecnologias Jack e Rakkarack e mostrei como o segundo é uma ótima opção para tirar timbres diferentes da sua guitarra e fazer um som esperto. Recomendo ler aquele artigo antes para se familiarizar com o que falarei aqui.

Neste artigo eu vou apresentar mais uma excelente opção para guitarristas, o simulador de amplificadores valvulados [Guitarix](http://guitarix.sourceforge.net/index.php).

## Instalação

Você vai precisar do Guitarix e do Jack instalados para acompanhar este artigo. Para conseguir mais resultados interessantes eu recomendo também o Jack Control, o Audacity e o gxtuner.

## Interface

Eu gosto bastante da carinha que este programa tem, aqui vai uma foto e uma explicação básica dela. Esta versão que eu estou usando é a _0.22.4_ e pode ser que a sua tenha uma aparência um pouco diferente, mas provavelmente nem tanto. Se estiver perdido peça ajuda nos comentários.

![](guitarix.png)

Em #1 vemos a parte principal do programa, o rack com o cabeçote do amplificador e os efeitos. É aqui que você vai passar a maior parte do tempo mexendo, mais especificamente em #2 onde ficam os controles do amp.

Para adicionar mais efeitos no rack dê uma olhada em #3 e uma lista de timbres pré-prontos (presets) está em #4.

Em #5 você pode ler algumas informações sobre o timbre que você está usando, desabilitar todos os efeitos (ouvir apenas o sinal de entrada) ou desconectar o programa do Jack. Finalmente em #6 você pode mostrar e esconder diferentes partes da interface.

## Conexões no Jack

O Guitarix modifica o sinal em dois passos: primeiro ligamos o nosso sinal de guitarra (geralmente o `system`) no cabeçote do amplificador (`gx_head_amp`) e depois ele passa pelos efeitos (`gx_head_fx`). Quando o Guitarix é iniciado ele já configura este esquema, como pode ser visto na figura abaixo:

![](jack.png)

Você pode ser criativo com as entradas e saídas e usar outros programas no meio, ou no sinal de saída ou até mesmo ligar coisas como sintetizadores, microfones e mais no sinal de entrada. Essa é a graça do Jack :)

## Afinando a Guitarra

Antes começar a tocar você pode usar a sessão do afinador. Infelizmente na última versão que eu instalei na minha máquina esse recurso parece que não está funcionando muito bem. Para resolver eu ando utilizando um programa chamado `gxtuner`, que é derivado do próprio código do Guitarix, mas funciona separadamente. Você pode instalar ele também pelos pacotes da sua distribuição e usar para afinar rapidamente sua guitarra. A foto abaixo mostra como ele funciona:

![](gxtuner.png)

## Usando os presets

Para começar em grande estilo você pode dar uma olhada nos `presets`, caso eles não estejam visíveis é possível acessá-los com o menu Presets -> Preset Selection. É possível achar desde sons de distorção bem forte, para rock e metal, até alguns sons limpos e outros pesadamente com efeitos, embora para brincar de [Tom Morello](https://en.wikipedia.org/wiki/Tom_morello) eu recomende o Rakarrack mesmo.

Tome cuidado que algumas distorções podem ficar bem cheias de ruído e diminuir isso envolve entre outras coisas melhorar a qualidade de: cabos, captadores da guitarra ou sua placa de áudio. Para resultados mais profissionais talvez seja necessário empregar o uso de pré-amplificadores reais ou interfaces de áudio com maior qualidade. Não é fácil na realidade, mas uma dica é mexer com os parâmetros do próprio Guitarix o que nos leva à próxima sessão.

## Criando seu próprio timbre

Como você pode ver na foto da interface, a quantidade de botões, alavancas e coisinhas para girar aqui é enorme. Na sessão do amplificador é possível escolher o tipo e a configuração das válvulas (como visto em #2 a usada é &#8220;12ax7&#8243;). Aumentando o `Drive` e o valor de `Clean/Dist` você cria a distorção com o carater das válvulas selecionadas. Mudando o volume de entrada (Pre Gain) e saída (Master Gain) você vai estar fazendo a amplificação do sinal, sendo o primeiro o que chamamos de pré-amplificador. Esses botões de volume que podem te ajudar a tirar uma distorção legal, mas é um trabalho árduo, como é com um amplificador na vida real também.

Eu até gosto de ficar horas mexendo nos parâmetros, mas não sou particularmente bom nisso. Por isso eu recomendo que vocês façam como eu e dêem uma explorada nos timbres já prontos e modifiquem os que lhe agradarem mais. Se você me conhece pessoalmente e quer pegar um café e ficar horas discutindo sobre timbres e efeitos de guitarra, eu aceito o convite.

## Gravando

Você pode conectar com o Jack o sinal sendo gerado pelo `gx_head_fx` ou pelo `gx_head_amp` (se quiser apenas o som amplificado sem efeitos) a algum programa de gravação. Mais uma vez veja este [post](http://blog.lfzawacki.com/linux-guitarrista-pobre/) para um exemplo similar em que o Audacity é usado para gravação. Outros programas que podem servir para gravação são o [qtractor](http://qtractor.sourceforge.net/) ou o [qjackrcd](http://sourceforge.net/p/qjackrcd/home/Home/). Em posts futuros esta parte do processo terá mais atenção.

## Demonstração

Retirado diretamente do site do Guitarix, bastante divertida e mostrando com é possível fazer um tom bem encorpado com ele:

<iframe class='youtube-player youtuber' type='text/html' width='425' height='355' src='http://www.youtube.com/embed/t91xJUos10A?rel=0&fs=1' webkitAllowFullScreen mozallowfullscreen allowFullScreen frameborder='0'></iframe>

## Referências

*   [Introducing Guitarix](http://www.linuxjournal.com/content/introducing-guitarix)
*   [Fórum](http://guitarix.sourceforge.net/forum) : legal para conseguir ajuda e achar presets e dicas de como fazê-los
*   [Wiki do Guitarix](http://sourceforge.net/apps/mediawiki/guitarix/index.php?title=Main_Page "Main_Page")

### Você provavelmente curtirá:
<div style="clear: both"></div><div style="border: 0pt none ; margin: 0pt; padding: 0pt;">[<div style="border: 0pt none ; margin: 0pt; padding: 0pt; width: 150px; height: 225px;"><div style="border: 0pt none ; margin: 0pt; padding: 0pt; background: transparent url(http://blog.lfzawacki.com/wp-content/uploads/2012/07/sabotage.jpg) no-repeat scroll 0% 0%; -moz-background-clip: border; -moz-background-origin: padding; -moz-background-inline-policy: continuous; width: 150px; height: 150px;"></div><div style="border: 0pt none; margin: 3px 0pt 0pt; padding: 0pt; font-family: ; font-style: normal; font-variant: normal; font-weight: normal; font-size: 12px; line-height: normal; font-size-adjust: none; font-stretch: normal; -x-system-font: none; color: #333333;">Uma Jornada Musical</div></div>](http://blog.lfzawacki.com/uma-jornada-musical/)[<div style="border: 0pt none ; margin: 0pt; padding: 0pt; width: 150px; height: 225px;"><div style="border: 0pt none ; margin: 0pt; padding: 0pt; background: transparent url(http://blog.lfzawacki.com/wp-content/uploads/2012/07/music.png) no-repeat scroll 0% 0%; -moz-background-clip: border; -moz-background-origin: padding; -moz-background-inline-policy: continuous; width: 150px; height: 150px;"></div><div style="border: 0pt none; margin: 3px 0pt 0pt; padding: 0pt; font-family: ; font-style: normal; font-variant: normal; font-weight: normal; font-size: 12px; line-height: normal; font-size-adjust: none; font-stretch: normal; -x-system-font: none; color: #333333;">Music StackExchange</div></div>](http://blog.lfzawacki.com/528/)[<div style="border: 0pt none ; margin: 0pt; padding: 0pt; width: 150px; height: 225px;"><div style="border: 0pt none ; margin: 0pt; padding: 0pt; background: transparent url(http://blog.lfzawacki.com/wp-content/uploads/2012/10/mate.jpg) no-repeat scroll 0% 0%; -moz-background-clip: border; -moz-background-origin: padding; -moz-background-inline-policy: continuous; width: 150px; height: 150px;"></div><div style="border: 0pt none; margin: 3px 0pt 0pt; padding: 0pt; font-family: ; font-style: normal; font-variant: normal; font-weight: normal; font-size: 12px; line-height: normal; font-size-adjust: none; font-stretch: normal; -x-system-font: none; color: #333333;">Matehackers abre as portas!</div></div>](http://blog.lfzawacki.com/matehackers-abre-as-portas/)[<div style="border: 0pt none ; margin: 0pt; padding: 0pt; width: 150px; height: 225px;"><div style="border: 0pt none ; margin: 0pt; padding: 0pt; background: transparent url(http://blog.lfzawacki.com/wp-content/plugins/related-posts-thumbnails/img/default.png) no-repeat scroll 0% 0%; -moz-background-clip: border; -moz-background-origin: padding; -moz-background-inline-policy: continuous; width: 150px; height: 150px;"></div><div style="border: 0pt none; margin: 3px 0pt 0pt; padding: 0pt; font-family: ; font-style: normal; font-variant: normal; font-weight: normal; font-size: 12px; line-height: normal; font-size-adjust: none; font-stretch: normal; -x-system-font: none; color: #333333;">Minhas palestras em potencial para o FISL 14!</div></div>](http://blog.lfzawacki.com/minhas-palestras-em-potencial-para-o-fisl-14/)</div><div style="clear: both"></div><!-- Developer mode initialisation; Version: 1.2.9;Relation: both; All categories: 1;Found 4 posts;Basic sizes;Got sizes 150x150;Post-thumbnails enabled in theme;Post has thumbnail 760;Postthname: thumbnail;Image URL: http://blog.lfzawacki.com/wp-content/uploads/2012/07/sabotage.jpg;Using title with size 100. Using excerpt with size 0;Post-thumbnails enabled in theme;Post has thumbnail 795;Postthname: thumbnail;Image URL: http://blog.lfzawacki.com/wp-content/uploads/2012/07/music.png;Using title with size 100. Using excerpt with size 0;Post-thumbnails enabled in theme;Post has thumbnail 840;Postthname: thumbnail;Image URL: http://blog.lfzawacki.com/wp-content/uploads/2012/10/mate.jpg;Using title with size 100. Using excerpt with size 0;Post-thumbnails enabled in theme;Post has no thumbnail;Getting image from post body;Found wrong formatted image: ;Image URL: ;Image is empty or no file. Using default image;Using title with size 100. Using excerpt with size 0;Plugin execution time: 0.011596918106079 sec; -->![](G6dT7ROqdJE)