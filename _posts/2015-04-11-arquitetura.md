---
layout: post
title: "Documento de Arquitetura"
date: 2015-04-11 10:00:03
category: doc
description: Contém o Documento de Arquitetura de Software (DAS) do jogo.
---

## Introdução

No ano de 3500, os seres do planeta *Rohines* invadem a Terra em busca de água, algo que há muito já se tornara escasso e motivo para guerras intergalácticas. Nessa busca incansável, os *Rohinianos* destruíram parte do planeta e poucos seres humanos sobreviveram. Em **SpaceWars**, o jogador encorpora um dos poucos sobreviventes do Massacre *Rohiniano* e deve escapar da Terra e ir em direção à *Ascarth*, um planeta colonizado pelos seres humanos e um abrigo totalmente seguro. Mas para isso, o jogador deverá passar por toda a galáxia e enfrentar as piores raças inimigas que já viu!

### Finalidade

Este documento fornece uma visão arquitetural abrangente do sistema, usando diversas visões de arquitetura para representar diferentes aspectos do sistema. O Objetivo deste documento é formalizar as decisões arquiteturais importantes do projeto.

### Escopo

Este Documento de Arquitetura se aplica ao desenvolvimento do jogo **SpaceWars**, que está sendo desenvolvido na disciplina de Desenho de Software, na UnB

## Representação da Arquitetura

<center>
    <img src="/img/arquitetura.png" alt="Diagrama de Arquitetura" width="100%" />
</center>

## Metas e Restrições de Arquitetura

O jogo deve ser jogável em sistema operacional Linux e não requisitar placa de video dedicada. Deve conseguir manter o *framerate* mínimo de 30 fps e não requisitar mais que 1GB de RAM. A distribuissão deve ser gratuita sob licença GPL3, com direito ao código fonte.

<!-- # Visão de Casos de Uso

[Esta seção lista os casos de uso ou cenários do modelo de casos de uso se eles representam uma funcionalidade central e significativa do sistema final ou se têm uma ampla cobertura de arquitetura, ou seja, se experimentam muitos elementos arquiteturais ou se enfatizam ou ilustram um determinado ponto frágil da arquitetura.]

### Realizações de Casos de Uso

[Esta seção ilustra o funcionamento do software, apresentando algumas realizações (ou cenários) de casos de uso selecionadas e explica como os diversos elementos do modelo de design contribuem para a respectiva funcionalidade.]

# Visão Lógica

[Esta seção descreve as partes significativas do ponto de vista da arquitetura do modelo de design, como sua divisão em subsistemas e pacotes. Além disso, para cada pacote significativo, ela mostra sua divisão em classes e utilitários de classe. Apresente as classes significativas do ponto de vista da arquitetura e descreva suas responsabilidades, bem como alguns relacionamentos, operações e atributos de grande importância.]

### Visão Geral

[Esta subseção descreve toda a decomposição do modelo de design em termos de camadas e de hierarquia de pacotes.]

### Pacotes de Design Significativos do Ponto de Vista da Arquitetura

[Para cada pacote significativo, inclua uma subseção com o respectivo nome, uma breve descrição e um diagrama com todos os pacotes e classes significativos nele contidos.

Para cada classe significativa no pacote, inclua o respectivo nome, uma breve descrição e, opcionalmente, uma descrição de algumas de suas responsabilidades, operações e atributos mais importantes.]

# Visão de Processos

[Esta seção descreve a decomposição do sistema em processos leves (threads simples de controle) e processos pesados (agrupamentos de processos leves). Organize a seção em grupos de processos que se comunicam ou interagem. Descreva os modos principais de comunicação entre processos, como transmissão de mensagens e interrupções.]

# Visão de Implantação

[Esta seção descreve uma ou mais configurações da rede física (hardware) na qual o software é implantado e executado. Ela é uma visão do Modelo de Implantação. Para cada configuração, ela deve indicar no mínimo os nós físicos (computadores, CPUs) que executam o software e as respectivas interconexões (barramento, LAN, ponto a ponto e assim por diante.) Inclua também um mapeamento dos processos da Visão de Processos nos nós físicos.]

# Visão de Implementação

[Esta seção descreve a estrutura geral do modelo de implementação, a divisão do software em camadas e subsistemas no modelo de implementação e todos os componentes significativos do ponto de vista da arquitetura.]

### Visão Geral

[Esta subseção nomeia e define as diversas camadas e o seu conteúdo, as regras que determinam a inclusão em uma camada específica e as fronteiras entre as camadas. Inclua um diagrama de componentes que mostre os relacionamentos entre as camadas. ]

### Camadas

[Para cada camada, inclua uma subseção com o respectivo nome, uma lista dos subsistemas localizados na camada e um diagrama de componentes.]

# Visão de Dados (opcional)

[Uma descrição da perspectiva de armazenamento de dados persistentes do sistema. Esta seção será opcional se os dados persistentes forem poucos ou inexistentes ou se a conversão entre o Modelo de Design e o Modelo de Dados for trivial.] -->

## Tamanho e Desempenho

O Software final deve ser menor que 1GB e requisitarmenos de 1GB de RAM para executar com desempenho mínimo de 30fps.

<!-- # Qualidade

[Uma descrição de como a arquitetura do software contribui para todos os recursos (exceto a funcionalidade) do sistema: extensibilidade, confiabilidade, portabilidade e assim por diante. Se essas características tiverem significado especial, como, por exemplo, implicações de proteção, segurança ou privacidade, elas devem ser claramente delineadas.]
 -->