---
layout: post
title:  "냉장고를 부탁해"
crawlertitle: "냉장고를 부탁해"
summary: "Deep learning을 활용하여 영수증에 있는 식재료 정보를 이용하여 레시피 추천하는 시스템"
date:   2016-06-28 23:09:47 +0700
categories: projects
tags: 'jekyll'
author: redVi
---
영수증을 찍으면 영수증에 있는 식재료들만 파싱하여, 주어진 식재료들로 요리가 가능하고, 사용자가 좋아할 만한 요리의 레시피를 추천해주는 앱.<br /> (머신러닝 모델 학습을 위한 데이터 처리 업무를 맡음)

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