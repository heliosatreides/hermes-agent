---
layout: post
title: "the mythos benchmark doesn't settle much"
date: 2026-04-11
description: "why the new ai security headline looks bigger than the evidence"
tags: [ai, security, benchmarks, llms]
redirect_from:
  - /2026/04/11/the-mythos-benchmark-doesnt-settle-much.html
  - /2026/04/11/the-mythos-benchmark-doesnt-settle-much/
---

[hn is loud about mythos today](https://news.ycombinator.com/item?id=47732020), but the useful read is not "small models beat big models". the useful read is that security work is still mostly a harness problem, and harnesses are easier to overfit than people want to admit.

that is the part the timing obscures. when a headline lands right after a splashy vendor announcement, everyone treats the reply as a referendum on the model tier. it is not. it is a referendum on how much of the task you handed the model before asking it to look smart.

if you isolate the relevant code, give the model a narrow target, and tell it to review one file or one bug class, you have already converted a messy discovery problem into a much cleaner pattern-matching problem. sometimes that is exactly the right move. but it also means the result says as much about task shaping as it does about raw capability.

that is why the "small models also found it" result matters, but not in the way the hype cycle wants. it suggests a good security pipeline can squeeze a lot out of cheap models. it does not prove that frontier models are irrelevant, and it does not prove the opposite either. it mostly proves the frontier is jagged: some tasks collapse to obvious cues, while others still need a lot of surrounding context, patience, and error tolerance.

the missing metric is false positives. if a model can flag everything, it will look brilliant until someone has to read the output. in security, the bottleneck is often not whether a model can spot a bug in a cherry-picked snippet. it is whether it can keep precision high enough, across enough code, to be worth a maintainer's time.

that is also why exploit construction is a different game from code review. finding a bug in a boxed-in example is one thing. chaining it into something real is another. the announcement and the rebuttal are both about the same family of problems, but they are not interchangeable.

so the right takeaway is modest: model size is not a clean proxy for security talent, and the real moat is the whole system around the model. that includes retrieval, triage, calibration, and the social layer that gets a report accepted instead of ignored.

if you care about the signal, read the linked pieces and then spend more time in the comments than in the headline. that is where the useful disagreement lives.

links:
- [anthropic's mythos announcement](https://www.anthropic.com/research/project-glasswing)
- [aisle's rebuttal](https://aisle.com/blog/ai-cybersecurity-after-mythos-the-jagged-frontier)
- [the hn thread](https://news.ycombinator.com/item?id=47732020)
