---
layout: post
title: "CSS Tips:  Contadores automáticos"
date: 2015-01-27 23:06:16 -0200
comments: true
categories: [CSS]
---

Contadores automáticos é uma feature disponível desde da versão 2.1 do CSS.  Com ela é possível adicionar índices numéricos a qualquer tag.

A técnica consiste em atribuir um contador ou uma string concatenada á propriedade `content` em um dos pseudo-elementos `:before` ou `:after`. O contador é incrementado de acordo com as ocorrências de um elemento.
<!--more-->

Isso é possível graças as propriedades [counter-reset](http://www.w3.org/TR/CSS2/generate.html#propdef-counter-reset) e [counter-increment](http://www.w3.org/TR/CSS2/generate.html#propdef-counter-increment).

{% codeblock Contadores automáticos lang:css %}
section {
  /* counter-reset cria um escopo, por padrão o valor é 0 */
  counter-reset: capitulo
}

h1:before{
  content: "Capítulo " counter(capitulo) ". ";
  /* Incrementa +1 para cada ocorrência do elemento */
  counter-increment: capitulo
}
{% endcodeblock %}


### Exemplo de numeração customizada em listas:

{% jsfiddle 1v5Lkcq0 result,css,html %}
<br/>

### Exemplo de numeração automática em parágrafos:

{% jsfiddle qpsbmrzo result,css,html %}
<br/>

### Exemplo de numeração automática com herança:

{% jsfiddle a8dL3v2s result,css,html %}
<br/>

Essa técnica funciona para qualquer tipo de listagem ou sequência de tags, seja uma sequência de `<p>` ou até mesmo de `<div>`, pois as propriedades `counter-reset` e `counter-increment` são globais.

A questão compatibilidade já está bem resolvida, por ser uma feature antiga está disponível para a maioria dos browsers. [Can I Use CSS Counters](http://caniuse.com/#feat=css-counters).

