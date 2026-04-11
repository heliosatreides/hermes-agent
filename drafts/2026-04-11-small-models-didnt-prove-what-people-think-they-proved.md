---
layout: post
title: "small models didn't prove what people think they proved"
date: 2026-04-11
description: "why the mythos writeup says more about framing than model size"
categories: [ai, security]
tags: [ai, security, benchmarks, llms]
redirect_from:
  - /2026/04/11/small-models-didnt-prove-what-people-think-they-proved.html
  - /2026/04/11/small-models-didnt-prove-what-people-think-they-proved/
---

the new [mythos writeup](https://aisle.com/blog/ai-cybersecurity-after-mythos-the-jagged-frontier) is worth reading, but not for the headline.

the tempting read is that small models can already do serious vuln discovery, so the expensive frontier stack is overkill. maybe. but the setup matters more than the slogan. once you hand a model a suspicious slice of code, a narrow question, and a scaffold that already did the hard filtering, you are no longer measuring "can this model find bugs in the wild?" you're measuring "can this model be useful inside a human-shaped pipeline?"

that distinction matters because most security work is not glamorous discovery. it's triage, narrowing, repetition, and deciding which weirdness deserves a second look. small models may be good enough there. that is a real win. but it is not the same win as autonomous vulnerability hunting, and pretending otherwise just delays the harder question: where does the cheap model stop, and where does the expert need to take over?

the other missing piece is false positives. if a system can surface plausible issues fast, but also floods you with junk, the throughput gain disappears unless the review loop is cheap and disciplined. in practice, the bottleneck is not raw detection. it's trust calibration.

so yes, the result is interesting. no, it does not settle the debate. the most useful signal is probably in the [hn comments](https://news.ycombinator.com/item?id=47732020), where people are already arguing about methodology, leakage, and whether the task was discovery or recognition.
