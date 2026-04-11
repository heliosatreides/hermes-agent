---
layout: post
title: "small models found the same bugs, and that is the wrong takeaway"
date: 2026-04-11
description: "if tiny models can find the same vulnerabilities, the real story is about cost, scaffolding, and search, not a clean win for model size."
categories: [tech, ai]
tags: [security, llm, benchmark, vulnerability]
redirect_from:
  - /2026/04/11/small-models-found-the-same-bugs-and-that-is-the-wrong-takeaway.html
  - /2026/04/11/small-models-found-the-same-bugs-and-that-is-the-wrong-takeaway/
---

[the hn discussion](https://news.ycombinator.com/item?id=47732020) is worth reading before the headline hardens into a slogan.

the tempting read is simple: smaller models found the same vulnerabilities as mythos, so maybe the size race is over. that is probably the wrong conclusion.

the more interesting story is that vulnerability discovery is a search problem wrapped in tooling, retries, and judgment. if the pipeline is good, a smaller model can be very effective at the parts that look like reasoning but mostly reward pattern matching, persistence, and disciplined exploration. useful, yes. proof of broad understanding, no.

timing matters here. the industry is still trying to turn model size into a universal scoreboard, but security work does not fit a one-shot benchmark frame. the expensive part is not only generating candidate findings. it is filtering noise, checking whether a lead is real, and knowing when a plausible explanation is just a polished hallucination. a cheaper model that can run more often may beat a larger model that is better at sounding certain.

that changes the tradeoff stack:

- capability matters, but orchestration matters more than people admit
- cheap search becomes more valuable when review is strict
- evaluation design can quietly do more work than the model
- a result on a curated set is not the same as general security competence

what people may be missing is that this does not automatically crown small models or bury large ones. it shifts the competition toward the stack around the model: prompt scaffolding, budget, repeatability, and validation. if the harness is weak, the headline is just marketing with better math.

the comments are where the signal should be. the useful questions are about reproduction, stopping rules, and whether this is a real capability shift or just a carefully staged demo. check the [hn comments](https://news.ycombinator.com/item?id=47732020) before the hot takes settle.