---
layout: post
title: Tutoriais de Música Livre – Audacity
date: 2013-04-02
tags: ["audacity","audio","linux","livre","musica","software livre","software-musica"]
---

![](logo.jpg)

O [Audacity](http://audacity.sourceforge.net/) é em muitos aspectos um dos meus programas favoritos no Linux (mas ele também tem versões ótimas para Mac e Windows), principalmente por ser aquele cara que sempre resolve a treta que tu tem nas mãos. Ele é um daqueles programas que podem fazer coisas incríveis e milagrosas a lá Photoshop, mas que também tem a simplicidade do bom e velho paint (que nojinho). Neste artigo eu vou mostrar como fazer algumas coisas simples como gravação, corte de áudio, remoção de ruído e aplicação de efeitos.

## Instalação

Siga as instruções [no site oficial](http://audacity.sourceforge.net/download/) e no caso de qualquer problema faça perguntas nos comentários.

## Interface

A interface do Audacity é esta aqui:

![](gui.png)

Eu vou dar uma comentada rápida nela, você pode pular isso não estiver interessado.

Os botões de 'Tocar', 'Pausar', 'Parar' e 'Gravar' lá em cima são bem intuitivos (**#1**). Logo ao lado temos os "Modos do Cursor" (**#2**), como eu vou chamar, que é o que controla o que o seu cursor vai fazer quando clicar na onda. O caso de uso mais geral é o que vem por padrão que é apenas selecionar trechos de áudio ao clicar o mouse, as outras opções envolvem editar partes da onda e modificar seus valores, algo um pouco menos útil.

As barrinhas com (L, R) ao lado (**#3**) são os monitores de volume da entrada e da saída. Isto quer dizer que você verá elas se mexendo quando estiver gravando ou reproduzindo algo e é bom para se guiar enquanto estiver tentando deixar as configurações do jeito que você quer. Perto dessas barras você tem o ajuste de volume da entrada e saída (**#4**), e deve ser óbvio para que isso serve.

A próxima barra (**#5**) tem coisas como copiar/recortar/colar sessões do áudio, remover partes do áudio, introduzir silêncio, mudar o zoom, entre outras opções um pouco mais avançadas.

A maioria das funções nessas barras tem um atalho no teclado. As mais óbvias são o copiar/recortar (**ctrl+c**, **ctrl+x**), colar (**ctrl+p**) e também tocar (**barra de espaço**) e gravar (**r**).

A última parte importante de observar é a sessão onde ficam as faixas de áudio (**#6**) e algumas configurações ao lado de cada uma. Usando essa interface é possível silenciar faixas específicas (Mute), tocar elas sozinhas (Solo) e ajustar o volume e o balanço em faixas estéreo.

## Gravando

Para gravar algo, apenas aperte o botão com a bolinha vermelho, ou o atalho 'r' e faça algum som no seu microfone.

Cada nova gravação vai sendo colocada em um nova pista e isto é legal para se organizar, mas se você quiser gravar algo na pista em que o cursor está atualmente você pode apertar **shift+r** ou mesmo segurar **shift** ao pressionar o botão de gravar.

## Importando clipes de áudio

Importar clipes de áudio é tranquilo. 'File->Import->Audio' e escolha um arquivo no seu disco. A maioria dos formatos populares (quiçá todos) é suportada, então pode ficar tranquilo. Para uma maior compatibilidade de formatos você pode instalar o [FFmpeg](http://wiki.audacityteam.org/wiki/FFmpeg_integration).

## Cortando e removendo partes do áudio

Arrastando o mouse sobre partes do áudio você pode selecioná-lo. Apertando **delete** (ou **ctrl+k**) você pode apagar pedaços. No entanto isto nem sempre é o que você quer pois acaba por mover todo o áudio que vem depois (tente e veja o que estou dizendo). Para apagar pedaços do áudio sem mover todo o resto é possível usar a opção 'Silence Audio' que é um botão no menu ou o atalho **ctrl+l**.

Usando as opções de copiar e colar é possível também mover pedaços de áudio, duplicá-los, e etc... Neste quesito a interface é intuitiva, pelo menos para quem já está acostumado a usar um computador há algum tempo.

## Aplicando efeitos

Agora as coisas ficam interessantes mesmo com o menu '**Effect**'. Você pode fazer desde coisas simples como amplificação, equalização, mudança de velocidade e tom, fade in/out, etc... até coisas mais complicadas como compressão dinâmica (usado para normalizar o volume de uma faixa), remoção de ruído ambiente, eco, reverberação e muitos outros que podem ser fornecidos por terceiros. Para ter um exemplo do número de plugins que é possível conseguir gratuitamente dê uma olhada nos que tenho aqui:

![](effects.png)

Eles são de código livre e foram instalados como pacotes no meu sistema operacional. Os formatos de plugin suportados podem ser vistos [aqui](http://audacity.sourceforge.net/download/plugins) e se você quer instalar alguns pode fazer (no Linux) uma busca no seu gerenciador de pacotes por 'audio plugins' ou alguns dos formatos citados na página do Audacity, como por exemplo 'ladspa'.

Dito isto, para aplicar efeitos apenas selecione a pista e a área a qual você deseja que seja afetada, e escolha o efeito no menu. Quando o efeito tiver algo configurável, como por exemplo o volume de um plugin de amplificação, o Audacity vai lhe mostrar uma janela onde pode ser feita essa configuração.

## Mixando e salvando

Depois de gravar algumas pistas e aplicar seus efeitos você pode selecionar todas as pistas (usando **ctrl+a** ou arrastando o mouse) e escolher a opção 'Tracks->Mix and Render' para unir todas em uma só pista.

Para salvar um arquivo como resultado você pode usar a opção 'File->Export'. Caso queira exportar arquivos em formato MP3 dê uma olhada [aqui](http://wiki.audacityteam.org/index.php?title=Lame_Installation "Lame_Installation") para saber o que é preciso instalar.

## Desfazer infinito

O Audacity é super seguro, no sentido de que ele tem a função 'desfazer' com passos infinitos. Isso quer dizer que enquanto você tiver espaço no seu disco ele vai te permitir voltar atrás nas mudanças que você fez, como por exemplo: deleção de trechos de áudio, aplicação de efeitos, movimentação de áudio, customização de parâmetros de uma pista. Isto quer dizer que é muito tranquilo ficar gravando e editando com ele por horas.

## Vídeo-demonstrações

Eu mesmo pensei em gravar alguns vídeos demonstrando várias funções do Audacity, mas achei [este canal legal no Youtube](https://www.youtube.com/user/wixstudio/videos?query=audacity) em que o cara já faz isto. Pontos para ele e **recomendo**!

## Na próxima...

Eu irei demonstrar o Guitarix um simulador de amplificador valvulado no Linux. Se preparem para tirar um som esperto de suas guitarras! Além disso para fazer a ponte com este episódio, vamos usar o Audacity para gravar tudo :)

![](tux.png)

# Continuem usando software livre e deixem comentários, sugestões e correções!
