---
layout: post
title: Lendo sinais analógicos do Arduino com Python
date: 2015-06-12
tags: ["Arduino","pyTchê","Python"]
---

Bueno, depois do Joel aterrorizar tanto que não iria dar tempo de concluir o projeto do robô até o [FISL 16](http://softwarelivre.org/fisl16), ontem resolvi ver como funciona o tal do Arduino, que vai ser utilizado no projeto, para saber das reais dificuldades de implementar a coisa toda.

Na verdade o que me animou mais foi conhecer o [Firmata](http://firmata.org/wiki/Main_Page), através do José, que possibilita que eu use, facilmente, o Arduino como uma extensão do meu computador, e o melhor ainda, permite que eu desenvolva todo o software necessário utilizando Python, com a lib [pyFirmata](https://github.com/tino/pyFirmata).

Para fazer o teste utilizei um arduino Uno e um potenciômetro de 10k.

[![Untitled Sketch_bb](/assets/2015/Untitled-Sketch_bb.png)](/assets/2015/Untitled-Sketch_bb.png)

Esse foi o código utilizado:

    # -*- coding: utf-8 -*-

    import time
    from pyfirmata import Arduino, util
    import sys, os

    b = Arduino('/dev/ttyACM0')

    pot = b.get_pin('a:0:i')

    iterator = util.Iterator(b)
    iterator.start()

    while True:

    	val = pot.read()
    	cm = 'espeak -vpt-brf -p 100 -s 155 "O valor recebido é '+str(val)+'"'

    	time.sleep(2)

    	print str(val)
    	os.system(cm)

    b.exit()

E ai a bagaça funcionando. A voz do robô está sendo sintetizada pelo [Espeak](http://espeak.sourceforge.net/), para quem usa a melhor distribuição linux do mundo, que não preciso dizer que é o Ubuntu, basta instalar via apt-get:

    sudo apt-get install espeak

<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">

<iframe class='youtube-player youtuber' type='text/html' width='768' height='480' src='http://www.youtube.com/embed/eK-35NTbKUE' webkitAllowFullScreen mozallowfullscreen allowFullScreen frameborder='0'></iframe>
</div></figure>
