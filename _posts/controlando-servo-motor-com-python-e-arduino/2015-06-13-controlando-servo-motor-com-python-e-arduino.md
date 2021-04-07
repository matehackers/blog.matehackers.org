---
layout: post
title: Controlando Micro Servo com Python e Arduino
date: 2015-06-13
tags: ["Arduino","pyTchê","Python"]
---

Mais um exemplo de utilização do Arduino com Python, dessa vez controlando um micro servo. Da mesma forma que o post anterior, estou utilizando o Firmata e o pyfirmata.

Foi utilizado um Arduino uno e um microservo 9g. A parte física ficou assim:

[![servo](/assets/2015/servo.png)](/assets/2015/servo.png)

E esse foi o código python utilizado:

    from pyfirmata import Arduino, util
    from pyfirmata import SERVO
    from time import sleep
    from Tkinter import *

    board = Arduino('/dev/ttyACM0')

    board.digital[6].mode = SERVO

    def move_servo(a):
    	board.digital[6].write(a)

    root = Tk()

    scale = Scale(root,
        command = move_servo,
        to = 175,
        orient = HORIZONTAL,
        length = 400,
        label = 'Angle')
    scale.pack(anchor = CENTER)

    root.mainloop()

O código funcionando:

<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">

<iframe class='youtube-player youtuber' type='text/html' width='768' height='480' src='http://www.youtube.com/embed/D33J2FQLUiM' webkitAllowFullScreen mozallowfullscreen allowFullScreen frameborder='0'></iframe>
</div></figure>
