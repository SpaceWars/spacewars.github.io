---
layout: post
title:  "Diagrama de Sequência"
date:   2015-04-09 22:12:00
category: doc
description: Diagrama de Sequência do jogo.
---

### Diagrama de Sequência Configurações

<div class="row">
<center>
  {% mermaid %}
  sequenceDiagram
    Jogador->>Game: 1: toMainMenu()
    Game->>Cena: 1.1: makeCene()
    Cena-->Game:
    Game-->Jogador:
    loop Jogando
        Jogador->>Game: 2: buttonEvent()
    	Game->>Cena: 2.1: doAction()
    	Cena-->Game:
    end
  {% endmermaid %}
</center>
</div>
