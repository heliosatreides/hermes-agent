---
layout: post
title: "idiomatic design is not a restore point"
date: 2026-04-12
description: "a recent h n essay argues for bringing back idiomatic interfaces, but the real problem is that software keeps shipping without a clear opinion about the job it is for."
categories: [design, product]
tags: [hn, ux, software]
redirect_from:
  - /2026/04/12/idiomatic-design-is-not-a-restore-point.html
  - /2026/04/12/idiomatic-design-is-not-a-restore-point/
---

the top h n story today is [bring back idiomatic design](https://essays.johnloeber.com/p/4-bring-back-idiomatic-design), and the basic point lands: software keeps getting less legible while pretending to be more flexible.

but "bring back" is doing a lot of work here.

we did not lose idiomatic design because teams stopped caring. we lost it because every product now has three bosses: growth, compliance, and cross-platform consistency. each one rewards generic patterns, and generic patterns are where intuition goes to die. the result is not just uglier ui. it is ui that no longer tells you which actions are safe, reversible, or even primary.

the catch is that idiom is not a virtue by itself. an interface can be idiomatic and still be a trap if the underlying workflow is novel, messy, or contested. not every task deserves the same affordances, and copying "what users already know" often just imports old confusion into a new context.

that is why the interesting question is not whether design should be idiomatic. it is whether a product has the courage to choose a small number of real conventions and then defend them ruthlessly. the best systems make a few things obvious and leave the rest alone. the worst systems pile on exceptions until every control feels borrowed.

if you read one thing besides the essay, read the comments on h n. there is more signal there than in the headline argument, especially around forms, date pickers, and the way "flexibility" quietly became a synonym for "we could not decide." [hn discussion](https://news.ycombinator.com/item?id=47738827)

