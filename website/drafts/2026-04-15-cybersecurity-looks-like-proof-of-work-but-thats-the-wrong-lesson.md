---
layout: post
title: "cybersecurity looks like proof of work, but that's the wrong lesson"
date: 2026-04-15
description: "ai is making brute force cheaper, but the harder problem is still triage, ownership, and fixing what the scanner finds."
categories: [security, ai]
tags: [cybersecurity, ai, llm, proof-of-work, tradeoffs]
redirect_from:
  - /2026/04/15/cybersecurity-looks-like-proof-of-work-but-thats-the-wrong-lesson.html
  - /2026/04/15/cybersecurity-looks-like-proof-of-work-but-thats-the-wrong-lesson/
---

the [headline](https://www.dbreunig.com/2026/04/14/cybersecurity-is-proof-of-work-now.html) is catchy because it turns a messy systems problem into a clean economic metaphor. that is also why it is slightly misleading. security has always been a contest of budgets, attention, and patience. ai does not change the game so much as it lowers the cost of trying more things, which is not the same as raising the cost of being safe.

the timing matters because defenders are already drowning in logs, alerts, dependency churn, and half-fixed reviews. when people say "proof of work," they usually mean the attacker has to spend more compute. but the real shortage on the defender side is human context. a model can scan more code, yet every useful finding still needs triage, prioritization, and a maintainer who can ship the fix without breaking everything else.

the tradeoff people keep skipping is that cheaper search does not automatically produce better security. it can also produce more noise, more false confidence, and more pressure to treat scanning as a substitute for design. if the answer to ai-assisted offense is just more ai-assisted defense, the software stack becomes a permanent bidding war. that is a tax on every team, especially the ones that cannot afford a security department.

the better question is not whether ai makes attacks or defenses faster. it is which parts of the stack are still built on trust, reuse, and endless update channels that were never meant to survive industrialized scrutiny. the [hn thread](https://news.ycombinator.com/item?id=47769089) is where the useful disagreement shows up. read the comments for the signal, not the slogan.
