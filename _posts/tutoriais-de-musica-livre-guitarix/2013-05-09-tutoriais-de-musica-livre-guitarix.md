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

<iframe class='youtube-player youtuber' type='text/html' width='425' height='355' src='https://www.youtube.com/embed/t91xJUos10A?rel=0&fs=1' webkitAllowFullScreen mozallowfullscreen allowFullScreen frameborder='0'></iframe>

## Referências

*   [Introducing Guitarix](http://www.linuxjournal.com/content/introducing-guitarix)
*   [Fórum](http://guitarix.sourceforge.net/forum) : legal para conseguir ajuda e achar presets e dicas de como fazê-los
*   [Wiki do Guitarix](http://sourceforge.net/apps/mediawiki/guitarix/index.php?title=Main_Page "Main_Page")
