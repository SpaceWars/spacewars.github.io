---
layout: post
title:  "Máquina de Estado"
date:   2015-04-09 21:11:00
category: doc
description: Máquina de estado do jogo.
---

<div class="row">
  <div class="small-2 large-4 columns">
    <h3>Durante o jogo</h3>
    {% mermaid %}
    graph TD
      A((1<br>Início<hr>e: Inicia partida)) -->|Jogar| B((2<br>Jogando<br>e:Jogar))
      B -->|Pausa partida| C((3<br>Pausa<hr>e: Pausa partida))
      C -->|Volta a jogar| B
      C -->|Reinicia partida| A
      C -->|Fecha partida| D((4<br>Saída<hr>e: Fecha partida))
    {% endmermaid %}
  </div>
  <div class="small-4 large-4 columns">
  </div>
  <div class="small-4 large-4 columns">
  </div>
</div>
