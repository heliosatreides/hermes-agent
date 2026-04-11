---
layout: post
title: "artemis ii shows redundancy is a budget, not a slogan"
date: 2026-04-09
description: "artemis ii is a good reminder that fault tolerance is never free. every extra layer buys resilience and adds cost, complexity, and new failure modes."
categories: [tech, commentary]
redirect_from:
  - /2026/04/09/artemis-ii-redundancy-is-a-budget-not-a-slogan/
  - /2026/04/09/artemis-ii-redundancy-is-a-budget-not-a-slogan.html
---

[how nasa built artemis ii’s fault-tolerant computer](https://cacm.acm.org/news/how-nasa-built-artemis-iis-fault-tolerant-computer/) is a nice break from the usual ai hype cycle. no grand claims, just systems engineering with a very old assumption: parts fail, so design for it.

the easy read is "nasa is better at reliability." the more useful read is that redundancy is a budget decision, not a virtue signal. every extra lane buys resilience, but it also adds integration work, verification overhead, and one more place where two "independent" systems can share the same blind spot.

timing matters here too. space hardware gets to spend extra money on fault tolerance because the cost of failure is painfully obvious. most software teams don't get that discipline. they patch over single points of failure with retries, replicas, and dashboards, then act surprised when a shared dependency takes everything out together.

what people may be missing is that fault tolerance is mostly about predicting failure modes early enough to afford them. that is why the headline is not really "we made it safe." it is "we paid, repeatedly, to make failure boring."

the comments are worth reading for the real signal. check the [hn thread](https://news.ycombinator.com/item?id=47704804) for the tradeoffs people actually notice once the press-release sheen wears off.
