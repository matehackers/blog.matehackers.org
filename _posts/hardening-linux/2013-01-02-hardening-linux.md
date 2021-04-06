---
layout: post
title: Hardening Linux
date: 2013-01-02
tags: ["linux"]
---

Boa tarde, gostaria de lembrar a todos os usuários unix por ai no mundo selvagem da rede de computadores!

Primeira dica: Quando você está conectado a internet é importante ficar atento aos serviços que seu computador roda para tarefas cotidianas, por exemplo, desenvolvedores normalmente usam algum banco de dados para testarem suas aplicações e ao não configurar os serviços corretamente, eles ouvem em todas as interfaces. É muito importante manter os serviços rodando em suas devidas portas e interfaces específicas, assim, nunca se esqueça de modificar as portas específicas que vocês querem.

Para conferir o que está rodando sobre quais portas, você pode rodar um netstat, o netstat é um utilitário que mostra estatísticas da rede de seu computador, ele possui uma série de opções e possíveis argumentos, os que mais utilizo são -n (não resolver nomes) -a (tudo) -p (exibir o PID do processo ouvindo na porta) -o (mostra o tempo / estado) gerando o comando netstat -napo

Isso me permite descobrir tudo que está rodando no computador, assim, sempre tenha cuidado ao ver 0.0.0.0:PORTA, pois isso indica que o serviço está rodando em todas as interfaces, acessível pela internet.

Segunda dica: Firewall bem configurado, existem regras que muita gente desconhece como --tcp-reset do iptables, qualquer firewall que vocês usem, NUNCA esqueçam que é necessário sempre tapar tudo que vocês não querem e depois liberar o que vocês querem permitir o acesso.

Terceira dica: Acesso SSH, o SSH por si só respeita uma série de regras que podem ser configuradas em /etc/security/access.conf, configure-o conforme seu cenário ideal(não esqueça nunca de adicionar LOCALhost, caso contrário, você perde a box localmente, a não ser que seja essa a intenção) para impedir que os usuários efetuem login na máquina, mesmo com usuários, senhas e firewall desativado.

&nbsp;

That's it for today!

&nbsp;