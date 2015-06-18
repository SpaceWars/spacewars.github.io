---
layout: post
title:  "Documentação Suplementar"
date:   2015-06-17 21:50:03
category: doc
description: Documentação Suplementar
---

# Documentação Suplementar

## Objetivos

Tem como objetivo a destruição dos inimigos no cenário assim como alcançar o ponto final da fase sem colidir com nenhum objeto ou ser acertado por um tiro das naves inimigas.

## Escopo


Um jogo agressivo, brutal, *oldschool* e tenso. Seus nervos serão tensionados ao limite para expor suas emoções com o auxilio de cometas, e naves espaciais.

## Referências

- [Space Invaders](http://en.wikipedia.org/wiki/Space_Invaders)
- [Pydoc oficial](http://pydoc.net/Python/cocos2d/)
- [Pandoc](http://en.wikipedia.org/wiki/Pandoc)
- [Shut'em Up](https://pt.wikipedia.org/wiki/Jogo_eletr%C3%B4nico_de_tiro)

## Funcionalidade

Os inimigos alienigenas aparecem na tela de forma aleatória, bem como os detritos espaciais. A medida que o jogador vai avançando, a quantidade de objetos (tanto alienigenas quanto detritos) aparecendo na tela aumenta, proporcionando ao jogador oportunidade de obter mais experiência e aumentando a dificuldade do jogo. Ao atingir certas quantidades de experiência, o usuário poderá liberar outras fases, com características diferentes.


## Usabilidade

**SpaceWars** é um jogo no estilo *Shut'em up*. O jogo será controlado pelo tecladoou joystick.

## Confiabilidade

O jogo não deverá quebrar enquanto estiver sendo usado pelo usuário.

## Performance

- Leitura de entradas em tempo menor que 0.9 segundos
- Deverá manter FPS maior que 25, sendo 60 o ideal.

## Suportabilidade

- O jogo deverá ser *Open Source*, no intuito de permitir contribuição da comunidade.

## Restrições de Design

#### Python

- O jogo deve dar suporte para Python 2.7

#### Sistema Operacional

- O jogo deve ser jogavel em sistemas Linux com kernel 3.0 ou mais recente.