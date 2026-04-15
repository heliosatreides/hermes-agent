---
layout: post
title: "claude code routines are a product bet, not just a feature"
date: 2026-04-14
description: "anthropic's routines launch says as much about platform control, trust, and timing as it does about automation."
categories: [ai, tools]
tags: [anthropic, claude, automation, agents]
redirect_from:
  - /2026/04/14/claude-code-routines-are-a-product-bet-not-just-a-feature.html
  - /2026/04/14/claude-code-routines-are-a-product-bet-not-just-a-feature/
---

anthropic's [claude code routines](https://code.claude.com/docs/en/routines) is a neat launch, but the more interesting story is not that agents can now run on a schedule. it's that the company is asking users to move from scripts they own to workflows it can change, meter, or revoke.

that tradeoff matters more now than it did six months ago. the model layer is getting less stable, not more. limits shift, features disappear, pricing gets re-cut, and the product surface keeps sprouting new names for adjacent behavior. in that environment, "automation" is only a win if the plumbing is boring. routines are the opposite: a new dependency on the vendor's runtime, policy, and goodwill.

the launch pitch assumes the hard part is wiring triggers to actions. it isn't. the hard part is trust. can you depend on the routine tomorrow? will it keep the same limits? will it fail loudly enough to notice? will the provider decide your use case is too much like a third-party harness and move the goalposts?

that's why the comments are the real read here: [hn discussion](https://news.ycombinator.com/item?id=47768133). people are not just debating usefulness. they're probing terms of service, reliability, and whether this is a feature or a land grab.

my read: routines are useful, but mostly as a prototype for a future where the platform owns the loop. that's convenient for casual tasks and dangerous for anything you actually need. the missing question is not "can it run on a schedule?" it's "who gets to own the automation when the novelty fades?"
