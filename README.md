# Desafio jogo Detona Ralph DIO

O desafio é desenvolver um jogo Detona Ralph utilizando
HTML, CSS e Javascript! O objetivo do game é acertar o Ralph sempre que ele aparecer
em uma janela. Toda vez que isso acontecer você vai ganhar 1 ponto.

## Linguagem de programação utilizada

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## Explicando o Sistema

Neste sistema estamos trabalhando com views, values e actions!

Onde:

> View: É responsavel por controlar a parte visual, como a redução na tela de vidas para o Jogador.

> Values: É responsavel por controlar valores que funcional por trás do sistema, como armazenar a váriavel responsável por guardar o tempo onde inicia a contagem do timer.

> Actions: Eventos que ocorrem por trás do sistema, como a diminuição automatica do timer.

A função **Init()** é responsavel por iniciar o jogo recebendo toda a lógica vinda de suas funções auxiliares.

A função **countDown()** é responsavel por:

- [x] Decrecer o valor do timer
- [x] Mostrar o decrecimo na tela
- [x] Verificar se o timer chegou em 0 e mandar uma mesagem de Game Over

A função **randomSquare()** é responsavel por:

- [x] Percorrer todas as janelas e verificar se elas possuem a _class="enemy"_
- [x] Remover ou adicionar a _class="enemy"_ quando necessário
- [x] Gerar um número aleatório para reposicionar o Ralph em janelas diferentes

A função **addListenerHitBox()** é responsável por:

- [x] Percorrer todas as janelas e verificar se elas receberam um "click"
- [x] Verificar se a janela clicada é a mesma em que está o Ralph e mandar as informações cabiveis ao player
- [x] Verificar se a janela clicada é **diferente** da janela onde está o Ralph e mandar as informações cabiveis ao player

## Bônus feature: Decremento de vidas do player!

Como feature adicional e diferencial do projeto, tomei a liberdade de adicionar um sistema de
decrecimo de vidas do player caso o jogador erre a janela do Ralph! Quando o contador de vidas
chegar em _0_, o player será notificado de que não tem mais vidas e seu score. A cada janela clicada de forma
incorreta seu score também é afetado, perdendo **1 ponto** por cada erro!
