---
layout: post
title:  "Máquina de Estado"
date:   2015-04-09 21:11:00
category: doc
description: Máquina de estado do jogo.
---

<div class="row">
    <h3>Durante o jogo</h3>
  <div class="small-11 small-centered columns">
    {% mermaid %}
      graph TD
        A((1<br>Iniciando partida<br>e: Inicia partida)) -->|Inicia fase| B((2<br>Iniciando fase<br>e:Inicia fase))
        B -->|Joga fase| C((3<br>Jogando<br>e: Joga fase))
        C -->|Pausa| D((4<br>Jogo pausado<br>e: Pausa fase))
        D -->|Volta ao jogo| C
        D -->|Reinicia fase| B
        C -->|Morre| E((5<br>Morto<br>e: Morre))
        C -->|Conclui fase| F((6<br>Fase concluída<br>e: Conclui fase))
        F -->|Inicia nova fase| B
        E -->|Reinicia fase| B 
        D -->|Termina partida| G((7<br>Partida terminada<br>e: Termina partida))
        E -->|Termina partida| G
        F -->|Termina partida| G
    {% endmermaid %}
  </div>
</div>