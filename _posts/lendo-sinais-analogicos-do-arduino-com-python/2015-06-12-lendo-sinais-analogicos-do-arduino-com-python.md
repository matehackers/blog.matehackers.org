---
layout: post
title: Lendo sinais analógicos do Arduino com Python
date: 2015-06-12
tags: ["Arduino","pyTchê","Python"]
---

Bueno, depois do Joel aterrorizar tanto que não iria dar tempo de concluir o projeto do robô até o [FISL 16](http://softwarelivre.org/fisl16), ontem resolvi ver como funciona o tal do Arduino, que vai ser utilizado no projeto, para saber das reais dificuldades de implementar a coisa toda. <!--more-->

Na verdade o que me animou mais foi conhecer o [Firmata](http://firmata.org/wiki/Main_Page), através do José, que possibilita que eu use, facilmente, o Arduino como uma extensão do meu computador, e o melhor ainda, permite que eu desenvolva todo o software necessário utilizando Python, com a lib [pyFirmata](https://github.com/tino/pyFirmata).

Para fazer o teste utilizei um arduino Uno e um potenciômetro de 10k.

[![Untitled Sketch_bb](http://blog.matehackers.org/wp-content/uploads/2015/06/Untitled-Sketch_bb.png)](Untitled-Sketch_bb.png)

Esse foi o código utilizado:

&nbsp;

<script src="f5f23bf819de34584706.js"></script>

E ai a bagaça funcionando. A voz do robô está sendo sintetizada pelo [Espeak](http://espeak.sourceforge.net/), para quem usa a melhor distribuição linux do mundo, que não preciso dizer que é o Ubuntu, basta instalar via apt-get:

`_sudo apt-get install espeak_`

&nbsp;

<iframe src="eK-35NTbKUE" width="420" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe>