---
layout: post
title:  "바이오 개체간 연관성 분석을 위한 데이터마이닝 기법 연구"
crawlertitle: "How to use jekyll"
summary: "2018 Data informatics Lab 연구과제"
date:   2018-01-28 23:09:47 +0700
categories: projects
tags: ['project']
author: redVi
---
단백질 개체 시퀀스를 자연어 처리 알고리즘으로 분류하고, 그 결과를 시각화한 연구과제 <br /> (Bio-Vec)

If you are still looking for confidence with JavaScript, I highly recommend you read the other titles in this series first:

Up & Going: Are you new to programming and JS? This is the roadmap you need to consult as you start your learning journey.

- Up & Going
- Scope & Closures
- this & Object Prototypes
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
