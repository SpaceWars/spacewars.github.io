---
layout: post
title:  "Diagrama de Sequência - Configurações"
date:   2015-04-09 22:11:00
category: doc
description: Diagrama de Sequência do jogo referente às configurações.
---

### Diagrama de Sequência Configurações

<div class="row">
<center>
  {% mermaid %}
  sequenceDiagram
    Jogador->>Configurações: Acessa Configurações()
    Configurações-->Jogador: Mostra Tela()
    Jogador->>Configurações: Executa ação()
    Configurações-->>Estado do Jogo: Efetua comando()
    Estado do Jogo-->Configurações: Retorna alteração()
    Configurações-->Jogador: Mostra Tela()
  {% endmermaid %}
</center>
</div>