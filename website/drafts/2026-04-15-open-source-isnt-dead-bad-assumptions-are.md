---
layout: post
title: "open source isn't dead. bad assumptions are."
date: 2026-04-15
description: "closing code does not erase the attack surface. it just changes who gets to inspect it."
categories: [security, software]
tags: [open-source, ai, security, cal.com, tradeoffs]
redirect_from:
  - /2026/04/15/open-source-isnt-dead-bad-assumptions-are.html
  - /2026/04/15/open-source-isnt-dead-bad-assumptions-are/
---

the [cal.com story](https://www.strix.ai/blog/cal-com-is-closing-its-code-due-to-ai-threats) is a useful reminder that ai changes the economics of finding bugs, not the economics of shipping software. if your answer to automated vulnerability discovery is to close the code, you have not removed the attack surface. you have just moved it behind fewer eyes.

the timing makes the move feel more inevitable than it is. when defenders feel outgunned, secrecy starts to look like strategy. but secrecy only buys time if the real bottleneck is inspection. in practice, the bottleneck is usually fix speed, review depth, dependency hygiene, and the ability to respond without breaking users. none of that gets easier because the repo is private.

the tradeoff is not open source versus safety. it is accountability versus friction. open code gives attackers and defenders the same map. closed code can slow casual copying, but it also concentrates trust and makes outside review harder exactly when the pace of automated probing is rising. that is a governance decision, not a technical breakthrough.

the [hn thread](https://news.ycombinator.com/item?id=47780712) is where the real signal is. the good comments ask whether this is a security move or a business move, what changes in ci, and whether ai is actually exposing a new risk or just revealing old open-source economics more quickly. read the comments before you decide the headline means what it says.
