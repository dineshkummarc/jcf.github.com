---
layout: post
title: "jQuery Animate"
date: 2010-10-10 20:11
comments: true
sharing: true
footer: true
sidebar: false
---

jQuery's `animate` does a lot more than just scaling and translating nodes in a DOM and because of this it can be used to achieve some interesting effects.

<!--more-->

## How it works

When you call `animate` on a jQuery object you typically pass a hash of properties to change like so.

{% codeblock lang:javascript %}
// Here background colour on `#selector` fades to black.
$('#selector').animate({backgroundColor: '#000'});
{% endcodeblock %}

The interesting thing is you don't have to use a selector to construct the initial jQuery object. You can simply pass jQuery a hash and this will define your initial properties.

{% codeblock lang:javascript %}
$({a: 0}).animate({a: 5},
  step: function() {
    console.log(a);
  }
);
{% endcodeblock %}

The result of running the above example will be 0 to 5 output in your console log. Duration still works as it would with a typical `animate`.

## A real-world application

A more realistic example that reflects something I did recently is below.

{% codeblock lang:javascript %}
$progress_bar = $('#progress_bar');

$({counter: 0, width: 0}).animate({counter: 50, width: 200},
  step: function() {
    $progress_bar.css({width: this.width});
    $progress_bar.innerText(Math.ceil(this.counter));
  }
);
{% endcodeblock %}
