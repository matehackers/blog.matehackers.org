---
layout: post
title: Aumentando a Entropia em Servidores Linux
date: 2013-02-05
---

Segue aqui uma coisa legal que aconteceu no meu trampo e pretendo postar no mateblog.

Estavamos numa situação onde por alguma razão um dos nossos serviços: o mupdate "sentava" a máquina ficando stuck em 100% de utilização de cpu. Isso nos gerou vários cabelos brancos visto que esse serviço é fundamental no nosso serviço de emails.

Dando uma googleada achei o seguinte:
[http://blog.gmane.org/gmane.<wbr />mail.imap.cyrus/month=<wbr />20061001/page=20](http://blog.gmane.org/gmane.mail.imap.cyrus/month=20061001/page=20)

Onde esse cara fala que setar muitas acls em folders imap acaba por fazer o servidor utilizar toda a cpu. O que acontece é que para setar acls é utilizada uma conexão ssl. Como temos muitos folders IMAP e para cada folder é necessária uma nova autenticação esse processo acabar por consumir a entropia do sistema. A entropia é o nível de randomicidade que o sistema de vocês tem disponível. Teclado, mouse, vídeo e outros dispositivos  com entrada são fontes de entropia. No nosso servidor mupdate ao dispararmos:
**
**** cat /proc/sys/kernel/random/entropy_avail**

temos sempre valores abaixo de 1000. Com isso o kernel ficava sem entropia o que obrigava o mesmo a preemptar tudo para gerar novas chaves travando o nosso sistema!

Rodando o mesmo comando na minha estação de trabalho tive o valor: 2689 o que faz sentido visto que servidores não tem muitos dispositivos de entrada e saída fora a interface de rede!  Aqui uma explicação sobre possíves fontes de entropia:
[https://www.ibm.com/<wbr />developerworks/<wbr />mydeveloperworks/blogs/<wbr />752a690f-8e93-4948-b7a3-<wbr />c060117e8665/entry/um_<wbr />devrandom_infindavel?lang=pt_<wbr />pt](https://www.ibm.com/developerworks/mydeveloperworks/blogs/752a690f-8e93-4948-b7a3-c060117e8665/entry/um_devrandom_infindavel?lang=pt_pt)

Ai acabamos por instalar o haveged que injeta entropia sempre que essa cai abaixo de 1000. Que segundo o archwiki-> [https://wiki.archlinux.org/<wbr />index.php/Haveged  ](https://wiki.archlinux.org/index.php/Haveged) é um limiar perigoso.

O Christian Perrone deu uma explicação excelente na lista do matehackers sobre a importância da entropia, me dei o direito de postar aqui!

<span><span style="font-family: tahoma,sans-serif;">SSL precisa gerar chaves aleatórias e estas chaves são geradas usando geradores de números aleatórios e o gerador de número aleatório precisa de uma semente que é alterada continuamente de tanto em tampo tempo ou de tantos em tantos ciclos, geralmente se usa um algorítmo de criptografia tipo o AES que extraí um pouco de dados do pool do Kernel e usa estes dados como chave para criptografar o estado atual e assim por diante. Se o pool do kernel está com entropia baixa o gerador de números aleatórios pode começar a ficar previsível. O Kernel geralmente cria dois devices, o /dev/random e o /dev/urandom, o /dev/random vai bloquear a leitura enquanto não houver entropia suficiente para retornar números aleatórios, já o /dev/urandom é um gerador de número aleatório que não garante a entropia, ou seja, não é uma boa escolha para gerar números aleatórios para criptografia</span></span>