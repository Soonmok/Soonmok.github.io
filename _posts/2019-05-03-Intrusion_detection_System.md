---
layout: post
title:  "Intrusion detection System"
crawlertitle: "Intrusion detection System"
summary: "Deep learning 기반 악성 행위 탐지 시스템"
date:   2019-05-15 23:09:47 +0700
categories: projects
tags: 'jekyll'
author: redVi
---
네트워크 패킷 로그에서 뽑아낸 feature 들을 사용하여, 악성행위를 구분하는 AI 기반 탐지기.

If you are still looking for confidence with JavaScript, I highly recommend you read the other titles in this series first:

Up & Going: Are you new to programming and JS? This is the roadmap you need to consult as you start your learning journey.

- Up & Going
- Scope & Closures
- this & Object Prototype
- Types & Grammar
- Async & Performance

[![railroad]({{ site.images | relative_url }}/rails.jpg)]({{ site.images | relative_url }}/rails.jpg)

If you've already read all those titles and you feel pretty comfortable with the topics they cover, it's time we dive into the evolution of JS to explore all the changes coming not only soon but farther over the horizon.

## `let` Declarations

However, we can now create declarations that are bound to any block, called (unsurprisingly) *block scoping*. This means all we need is a pair of `{ .. }` to create a scope. Instead of using var, which always declares variables attached to the enclosing function (or global, if top level) scope, use `let`:

{% highlight js %}
var a = 2;

{
    let a = 3;
    console.log( a );   // 3
}

console.log( a );       // 2
{% endhighlight %}