---
layout: post
title: Tutoriais de Música Livre
date: 2013-02-01
tags: ["computação e música","linux","musica","oficina","tutoriais"]
---

Dia 16/01 eu organizei no [Matehackers](http://matehackers.org/) a Oficina de Música Livre e apresentei para algumas pessoas alguns programas e técnicas que eu mesmo ando usando para produzir conteúdo sonoro no ambiente Linux. Eu já venho a algum tempo pensando em de alguma maneira apresentar estas ferramentas na forma de pequenos **tutoriais** e finalmente resolvi fazer isto enquanto documento o que foi apresentado na oficina.

## Música Livre?

O nome da oficina é propositalmente estranho, porque afinal a música normalmente já é livre. Eu posso abrir a boca e cantar uma melodia, comprar um instrumento e aprender a tocar, ouvir uma canção e repoduzí-la eu mesmo, certo? Isso tudo é verdade, mas também é verdade que os consumidores, como somos vistos pela industria musical, cada vez mais querem se meter no papel de produtores e esse _livre_ no título quer dizer _livre_ para produzir as músicas que queremos.

## A situação da Produção Musical no Linux

Então, supondo que queiramos produzir a nossa própria música, quão útil pode ser um sistema operacional livre? Bastante na realidade! A seleção de softwares é extensa e eles estão todos disponíveis gratuitamente e a um clique de distância usando um gerenciador de pacotes da sua distribuição favorita.

Quer alguns exemplos? Para gravação, corte e edição de áudio temos o excelente [Audacity](http://audacity.sourceforge.net/). O Audacity pode ser usado também com centenas de efeitos como ecos, filtros, simulações de equipamento analógico, entre outros ; que estão disponíveis na forma de plugins, facilmente obtidos nos repositórios da sua distribuição Linux.

Para trabalhar com MIDI e fazer sequenciamento de notas existe o [Seq24](http://www.filter24.org/seq24/), [MuseScore](http://musescore.org/), além do [Hydrogen](http://www.hydrogen-music.org/hcms/) que é ótimo para escrever linhas de bateria e já vem com um grande conjunto de amostras sonoras para serem usadas. Para sintetizar sons para essas mensagens MIDI você pode usar o [ZynAddSubFx](http://zynaddsubfx.sourceforge.net/), [Yoshimi](http://yoshimi.sourceforge.net/), [QSynth](http://qsynth.sourceforge.net/), entre muitos outros...

Para os guitarristas temos o simulador de amplificador valvulado [Guitarix](http://guitarix.sourceforge.net/), a pedaleira virtual de efeitos [Rakarrak](http://rakarrack.sourceforge.net/) e o [TuxGuitar](http://tuxguitar.herac.com.ar/) para visualizar e editar arquivos de tablatura (funciona com todos os formatos mais populares).

Para soluções integradas de gravação, com suporte a gravação de áudio e MIDI em várias trilhas, aplicação de efeitos em tempo real e coisas assim temos diversas DAWs como o [Ardour](http://ardour.org/) e o [Qtractor](http://qtractor.sourceforge.net/) (meu favorito no momento).

Todos estes programas podem ser usados em conjunto por meio do kit [Jack](http://jackaudio.org/), que age como uma espécie de mesa de virtual de mixagem, onde podemos enviar áudio e MIDI entre os diferentes aplicativos.

## Começando a jornada

Feita esta introdução estarei fazendo uma série de posts sobre cada uma dessas ferramentas. O primeiro é um que eu escrevi há muito tempo voltado para o uso do **Rakarrack** para aplicar efeitos no som de guitarra e depois disso um bem detalhado sobre o **Audacity**!

*   [Tutorial do Rakarrack](http://blog.matehackers.org/linux-e-o-guitarrista-pobre-lines-o-code/)

### Vejo vocês na próxima!