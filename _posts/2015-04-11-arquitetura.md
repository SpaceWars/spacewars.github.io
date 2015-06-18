---
layout: post
title: "Documento de Arquitetura"
date: 2015-04-11 10:00:03
category: doc
description: Contém o Documento de Arquitetura de Software (DAS) do jogo.
---

# Doc. de Arquitetura

## Introdução

No ano de 3500, os seres do planeta *Rohines* invadem a Terra em busca de água, algo que há muito já se tornara escasso e motivo para guerras intergalácticas. Nessa busca incansável, os *Rohinianos* destruíram parte do planeta e poucos seres humanos sobreviveram. Em **SpaceWars**, o jogador encorpora um dos poucos sobreviventes do Massacre *Rohiniano* e deve escapar da Terra e ir em direção à *Ascarth*, um planeta colonizado pelos seres humanos e um abrigo totalmente seguro. Mas para isso, o jogador deverá passar por toda a galáxia e enfrentar as piores raças inimigas que já viu!

### Finalidade

Este documento fornece uma visão arquitetural abrangente do sistema, usando diversas visões de arquitetura para representar diferentes aspectos do sistema. O Objetivo deste documento é formalizar as decisões arquiteturais importantes do projeto.

### Escopo

Este Documento de Arquitetura se aplica ao desenvolvimento do jogo **SpaceWars**, que está sendo desenvolvido na disciplina de Desenho de Software, na UnB

## Representação da Arquitetura

<center>
    <img src="/img/arquitetura.png" alt="Diagrama de Arquitetura" width="50%"/>
</center>

## Metas e Restrições de Arquitetura

O jogo deve ser jogável em sistemas operacionais Linux e Mac OS X e não requisitar placa de video dedicada. Deve conseguir manter o *framerate* mínimo de 30 fps e não requisitar mais que 1GB de RAM. A distribuição deve ser gratuita sob licença GPL3, com direito ao código fonte.

## Visão de Cenários

Devido ao fato do SpaceWars não ter sido descrito usando casos de uso, aqui, serão utilizados os cenários descritos. O conjunto de cenários a seguir representam a justificativa para a arquitetura proposta:

* Menu Inicial
* Iniciar fase
* Dinâmica do SpaceWars
* Movimentar Spaceship
* Atira
* Perde o Jogo
* Avança de Nível
* Créditos
* Configurações

### Cenários Significativos para a Arquitetura

* __Menu Inicial:__ Neste cenário, o usuário terá o poder de escolher a ação desejada: Jogar, Configurar, ver Créditos ou sair do jogo.
* __Iniciar Fase:__ Neste cenário, o usuário será capaz de escolher a fase desejada e dar início ao jogo. É o cenário responsável por dar início aos outros cenários.
* __Dinâmica do SpaceWars:__ Este cenário representa a lógica do jogo, onde o usuário poderá se movimentar, atirar, perder o jogo ou avançar de nível.
* __Movimentar SpaceShip:__ Aqui, o usuário será capaz de controlar a nave, que representa o usuário dentro do game. O usuário poderá se mover para frente, para trás, para a esquerda e para a direita.
* __Atirar:__ Para conseguir cumprir o objetivo do jogo, o jogador deverá destruir os inimigos que aparecerem na tela, para isso ele deverá atirar neles, apertando o botão específico para tal ação.
* __Perde o jogo:__ Caso o jogado seja atingido por algum inimigo, ele perde o jogo e entra num menu com as opções de sair ou reiniciar a partida.
* __Configurações:__ O usuário deve conseguir controlar algumas configurações do jogo, como volume da música e dos sons do jogo, se deseja jogar em modo fullscreen ou em modo janela e se deseja exibir o frame rate do jogo.

## Visualização Lógica

### Visão Geral

A aplilcação está divida em, basciamente, três camadas: Engine, Game e Layers.

* __Engine:__ Tudo relacionado às engines necessárias para que o jog aconteça. Módulos que cuidam das ações realizadas pelos inimigos, por exemplo.
* __Game:__ Onde se encontram as cenas e sprites do jogo. Utilizando da engine, as cenas e sprites são responsáveis por renderizar o game para o usuário.
* __Layers:__ Camada criada, basicamente, para separar as Layers específicas de menu.

<center>
    <img src="/img/arq-camadas.png" alt="Visão Lógica" width="80%" />
</center>

### Visão Lógica

#### Camada Engine

<center>
    <img src="/img/arq-action.png" alt="Camada Engine - Pacote action"  />
    <img src="/img/arq-enemy.png" alt="Camada Engine - Pacote enemy"  />
    <img src="/img/arq-event.png" alt="Camada Engine - Pacote event"  />
    <img src="/img/arq-gunfire.png" alt="Camada Engine - Pacote gunfire"  />
</center>

### Camada Game

<center>
    <img src="/img/arq-sprites.png" alt="Camada Game - Pacote sprites"  />
    <img src="/img/arq-scenes.png" alt="Camada Game - Pacote scenes"  />
</center>

### Camada Layer

<center>
    <img src="/img/arq-menu.png" alt="Camada Layer - Pacote menu"  />
    <img src="/img/arq-baselayers.png" alt="Camada Layer - Pacote base_layers"  />
</center>

## Tamanho e Desempenho

O Software final deve ser menor que 1GB e requisitarmenos de 1GB de RAM para executar com desempenho mínimo de 30fps.

