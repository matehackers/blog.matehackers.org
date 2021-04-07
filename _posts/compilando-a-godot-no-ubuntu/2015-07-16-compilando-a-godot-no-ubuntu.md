---
layout: post
title: Compilando a Godot no Ubuntu
date: 2015-07-16
tags: ["ferramentas","funprogramming","godot","linux","software livre"]
---

A nova versão da Godot deverá vir com bastante coisas legais, como uma interface mais amigável, possibilidade de editar várias cenas ao mesmo tempo, etc. Mas já é possível experimentar isso utilizando a versão de desenvovimento. Nesse post vamos ver como compilar a engine no Ubuntu 14.04 64bits.

Primeiramente vamos instalar as dependências:`
sudo apt-get install scons pkg-config libx11-dev libxcursor-dev build-essential libasound2-dev libfreetype6-dev libgl1-mesa-dev libglu-dev libssl-dev libxinerama-dev
`

Agora vamos clonar o repositório de desenvolvimento:`

    git clone https://github.com/okamstudio/godot.git godot_devel

    cd gotod_devel

Dentro do diretório do código digite o comando:

    scons platform=x11

Espere terminar o processo de compilação e entre no diretório _/bin_ vai existir um arquivo chamado **godot.x11.tools.64** basta executar.

Eis a nova interface dela:

[![godot](/assets/2015/godot.png)](/assets/2015/godot.png)

Por enquanto é isso. Quam quiser saber um pouco mais de detales sobre esse processo, basta acessar a documentação no github: [https://github.com/okamstudio/godot/wiki/advanced#compiling--running](https://github.com/okamstudio/godot/wiki/advanced#compiling--running)
