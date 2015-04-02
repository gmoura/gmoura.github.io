---
layout: post
title: "Documentando se CSS"
date: 2015-04-01 19:00:43 -0300
comments: true
sharing: true
categories: [css, style-guide, documentação] 
---

## Por que documentar ?

Esse post se dedica a falar sobre documentação de CSS, mas antes de conhecermos as maneiras de fazer, iremos entender a importância da documentação, seja ela para CSS ou para qualquer outro tipo de linguagem.

Documentação é aquele tipo de processo que todos os programadores conhecem, sabem que é importante mas poucos o fazem. O que não falta são desculpas para não documentar, como por exemplo: falta tempo, código deve ser auto explicativo, não sou bom com textos ou simplesmente não gosto.

Encontrar uma boa documentação que  explique o passo-a-passo (for dummies), de como as coisas funcionam tornaria o processo de adaptação de novos integrantes dentro da empresa ou projeto muito menos doloroso e mais rápido.
<!--more-->


Porém essa é uma realidade de poucas empresas ou projetos, na maioria das vezes quando se encontra uma documentação, ela está mal escrita e mal organizada. Um bom exemplo de como a documentação é importante, está nas linguagens que utilizamos, quanto melhor o nível da documentação, mais rápida será a curva de aprendizado. 

> Imagine sua linguagem de programação favorita com uma documentação desorganizada, agora, imagine ela sem documentação. Provavelmente você não estaria programando nela e muito menos a escolheria como sua favorita.

Ao meu ponto de vista só existem benefícios em documentar o código, como:

### Manutenção

De tempos em tempos os códigos passam por modificações/melhorias e saber qual era o objetivo e responsabilidades de uma classe ou mixin é essencial para que todos os programadores sigam a mesma linha de raciocínio.

### Código duplicado

Previne código duplicado e incentiva o reaproveitamento de código, pois antes de sair "codando", a documentação deve ser consultada.

### Padronização

Definir padrões para seu projeto faz com que todos os envolvidos entendam a mesma língua, traz transparência. Coisas como nomenclatura, semântica e estrutura de projeto ajuda na hora de encontrar erros ou achar determinados componentes.


**Convencidos de que documentação é um processo importante, iremos aprender como documentar seu CSS.**


## Let’s Rock

Alguns alguns pontos devem ser levados em consideração no início e durante a sua documentação:

* Ser de fácil acesso
* Bem estruturada 
* Padronizada
* Guias de boas práticas
* Exemplo de uso 
* Conter referências
* Constante atualização
* Bonita 

Um fator imporntante que deve ser pensado sobre a documentação é que a mesma deve está disponivel para todos envolvidos no projeto Então como podemos criar uma documentação de código CSS que atenda os requisitos acima, principalmente disponibilizá-la todos os envolvidos no projeto?

A solução é simples, criando um Style Guide.


Style Guide

Style Guide é um documento disponível online ou através de intranet. Esse documento contem todos os componentes, módulos, tipografia e grids, manuais de boas praticas, todos dispostos separadamente em um único lugar de acesso.

Esse documento pode ser criado de maneira manual ou por Geradores de Style Guide como KSS, Hologram, Styledocco, kaleistyleguide, entro outros.

Exemplos de CSS Style Guides 

..
..
.. 
Benefícios

Possibilita prototipação de alta fidelidade navegavel  
Facilita os Testes
Guia de referência

Dicas 

Um bom Style Guide não se limita em apenas listar os componentes em uma única página, deve conter também guias de boas práticas, dizendo o que deve ser feito e o que não deve ser feito em seu código CSS.

… exemplos best pratices de css

É interessante criar uma seção dedicada à explicar o significado de palavras, termos técnicos e termos exclusivos da empresa/projeto. Isso serve de grande ajuda para quem está iniciando no projeto, principalmente para os estagiários.

Definir uma metodologia de desenvolvimento do seu CSS é essencial para uma boa consistência do front-end de um projeto. Existem inúmeras metodologias como Atomic design, OOCSS, SMACSS, entre outros. Ou então defina a sua metodologia, contando que tal seja documentada no Style Guide.
 
Papel do Front-end e do Designer

Criar um Style Guide não é papel apenas para o desenvolvedor ou apenas do designer, deve ser feito em conjunto.

Em conjunto com o Designer defina a estrutura do seu Style Guide, crie um PSD com seções separadas para títulos, grids, botões, formulários, módulos, e assim por diante, categorizando os elementos de sua aplicação.

Caso haja dúvidas em como categorizar os elementos, você pode optar por usar frameworks como Bootstrap ou Foundation como referência para categorias de seus elementos.

Como fazer

Selecionei dois dos mais populares Geradores de Guia de Estilo do mercado, KSS e Hologram, vamos falar um pouco de cada um.
kss

Uma metodologia de documentação e um gerador de guia de estilo, funciona em pre-processadores, porém dedicado a conhecedores de Ruby.

.. exemplos
hologram 

Fofo e fácil de usar, utiliza da sintaxe markdown e também serve para documentar javascript

.. exemplos

Conclusão

Em aplicações de grande porte, como portais de notícias ou e-commerce, o CSS tende a crescer muito rápido pela grande quantidade de componentes desenvolvidos ao longo da vida do projeto. Sem documentação há grandes chances de existir código duplicado e conflitos de estilo e adotar como processo a documentação amenizará esses problemas.

