---
layout: post
title:  "네이버 상품 image retrieval 프로젝트"
crawlertitle: "How to use jekyll"
summary: "2019 네이버 해커톤 대회 참여"
date:   2019-02-28 23:09:47 +0700
categories: projects
tags: 'jekyll'
author: redVi
---
2019년 네이버 AI 해커톤 (VISION-AI) 대회 참가 프로젝트

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