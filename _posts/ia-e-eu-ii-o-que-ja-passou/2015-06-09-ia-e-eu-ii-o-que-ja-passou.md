---
layout: post
title: "IA e eu II: O que já passou"
date: 2015-06-09
tags: ["cic","educação"]
---

![](giphy.gif)Se você ficou decepcionado que o post anterior não continha nenhuma menção à Matrix ou ao Arnold Schwarzenegger, não se preocupe. Hoje vamos começar a dar uma olhada no que _já foi feito_ em termos de Inteligência Artificial. Porém, se você não aguenta mais historinha recomendo pular este post aqui também. Nos vemos no futuro.

## Há milhões de anos atrás, no futuro..

O primeiro trabalho a ser considerado efetivamente "Inteligência Artificial" foi feito em 1943 por Warren McCulloch e Walter Pits, no qual foi proposto o modelo de funcionamento de um neurônio artificial. Este neurônio podia assumir os estados "ligado" e "desligado", determinado em resposta aos estímulos proporcionados pelos outros neurônios vizinhos. Foi demonstrado também que uma rede de neurônios artificial conseguia computar qualquer função computável e sugerido que a mesma poderia aprender. Em 1949 Donald Hebb demonstrou uma simples regra pela qual a força de conexão entre os neurônios poderia ser modificada, a qual ficou conhecida como Aprendizado Hebbiano. Logo em seguida, em 1950, foi construído o primeiro computador de rede neural chamado de SNARC que fora feito com 3000 tubos de vácuo e conseguia simular uma rede de 40 neurônios.

<!--more-->

Embora o neurônio artificial seja considerado o primeiro trabalho, o termo Inteligência Artificial só viria a ser cunhado mais de 10 anos depois em Darthmouth nos Estados Unidos em um workshop organizado por John McCarthy que duraria dois meses e cujo propósito era estudar teoria dos autômatos, redes neurais e inteligência. Embora não tenha produzido nenhum progresso, o worksho serviu para introduzir as principais figuras da área entre si.

Nos seus primeiros anos a IA obteve bastante sucesso. Um a um, os items da lista "uma máquina nunca vai poder fazer X" compilada por Turing foram sendo desbancados. Newel and Simon criaram o primeiro GPS (General Problem Solver), um programa desenhado para imitar a maneira como humanos pensam ao invés de simplesmente seguir regras lógicas. Na classe limitada de desafios que conseguia resolver, a ordem dos subobjetivos que o programa tentava seguir era similar à humana. Na IBM, Nathaniel Rochester criaria o primeiro Provador de Teoremas Geométricos, o qual conseguia provar teoremas que vários estudantes consideravam complexos. Arthur Samuel refutou a ideia de que programas somente conseguiriam fazer o que lhes eram dito criando um programa de computador que conseguia jogar um jogo melhor que o seu criador.

Foi nessa época também que McCarthy criaria sua linguagem de programação _Lisp_ que viraria a linguagem dominante em IA e com a qual ele faria o primeiro algoritmo que aceitava novos axiomas, sendo então o primeiro autômato que conseguia adquirir novas capacidades sem necessitar ser reprogramado. Outras contribuições significativas foram o programa SAINT (1963) que conseguia resolver problemas de Cálculo típicos do primeiro ano de curso, o programa ANALOGY (1968) respondia a perguntas de analogia geométrica como as de testes de QI, o programa STUDENT (1967) resolvia problemas algébricos e o programa SHRDLU (1972) era capaz de executar instruções do tipo "Encontre um bloco maior do qu você está segurando agora e o coloque na caixa". Foi nessa época também que foram feitas melhorias no processo de aprendizado Hebbiano que ficaram conhecidas como redes _adalines_.

**Coisas que falaram para o Alan Turing que um computador jamais conseguiria fazer:**
> Be kind, resourceful, beautiful, friendly, have initiative, have a sense of humor, tell right from wrong, make mistakes, fall in love, enjoy strawberries and cream, make someone fall in love with it, learn from experience, use words properly, be the subject of its own thought, have as much diversity of behavior as man, do something really new.

## Honeymoon is over

O sucesso inicial foi seguido de um período de relativa estagnação. O fato de que estes algoritmos só conseguiam fazer manipulação simbólica e não conheciam nada sobre o domínio que trabalhavam provou ser um grande empecilho. Além diss a maioria dos primeiros programas de IA tentavam resolver o problema tentando várias combinações até que o resultado fosse atingido, o que não era factível para instâncias de problemas marginalmente maiores. Foi nesta época que Minsky e Papert provaram que um neurônio artificial agora conhecido como _perceptron_ era restrito no tipo de funções que conseguia representar e o financiamento de pesquisas na area se tornou escasso.

Já na década de 1970, houve o surgimento dos sistemas baseados em conhecimento prévio como o programa DENDRAL que viu uma melhora significativa de desempenho na tarefa de inferir a estrutura molecular à partir da massa dos seus componentes. O programa que inicialmente tentava todas as alternativas possíveis passou a utilizar de conhecimento de especialistas em química para identificar subestruturas conhecidas o que reduzia significadamente o número de tentativas. O primeiro caso de sucesso comercial reportado destes sistemas especialistas era um programa que ajudava na compra de novos computadores e que teria economizado à empresa US$40 milhões por ano, o que explica o fato destes sistemas continuarem sendo usados até hoje.

Bonus Fact: A microsoft incorporou vários sistemas especialistas no Windows para corrigir problemas.

## Science, bitch

Paralelamente, houve o ressurgimento das redes neurais no final da década de 1980, proporcionado pela reinvenção do algoritmo de _back-propagation_, uma maneira eficiente de atualizar os pesos das conexões nos neurônios, e também uma melhoria nas práticas de pesquisa na área que passou a exigir um maior rigor científico acompanhado do uso de bancos de dados padrões que permitiam o teste e comparação dos resultados entre diferentes algoritmos.

Em uma outra linha recente, a ênfase no algoritmo da lugar ao uso de grandes quantidades de dados inspirado no trabalho de Yarowsky (1995) que demostrou se possível reconhecer se o uso da palavra 'plant' significava uma flor ou uma fábrica com precisão acima de 96% sem utilizar de labels fornecidos por humanos, apenas com a definição do dicionário desta palavra. Trabalhos como o dele sugerem um "gargalo de conhecimento" na IA, ou seja, o conhecimento que o um sistema precisa pra resolver um problema pode vir de grandes massas de dado ao invés de intervenções de especialistas na área.

Hoje em dia, a IA está em várias aplicações de campos diferentes, como por exemplo:

*   Na área de robótica veicular com carros auto guiados.
*   Na área de reconhecimento de fala.
*   Planejamento automático de tarefas.
*   Jogos, com destaque para o computador DEEP BLUE da IBM que derrotou o campeão mundial de xadrez, Garry Kasparov.
*   Controle de SPAN em mensagens de e-mail.
*   Militar e Logística.
Esta são apenas algumas das aplicações da Inteligência Artificial hoje, um campo de intensa pesquisa e promessas.

No próximo post a vamos deixar de historinha e explorar o conceito de redes neurais.

Fonte: Russell, Stuart, and Peter Norvig. "Artificial intelligence: a modern approach." (1995).