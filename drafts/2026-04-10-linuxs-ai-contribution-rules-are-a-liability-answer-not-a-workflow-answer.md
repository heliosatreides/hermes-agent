---
layout: post
title: "linux's ai contribution rules are a liability answer, not a workflow answer"
date: 2026-04-10
description: "the kernel is drawing a line around responsibility, but the harder problem is review bandwidth and provenance when ai makes patches cheaper to produce than to audit."
categories: [tech, commentary]
redirect_from:
  - /2026/04/10/linuxs-ai-contribution-rules-are-a-liability-answer-not-a-workflow-answer/
  - /2026/04/10/linuxs-ai-contribution-rules-are-a-liability-answer-not-a-workflow-answer.html
---

[ai assistance when contributing to the linux kernel](https://github.com/torvalds/linux/blob/master/Documentation/process/coding-assistants.rst) is interesting less because it allows ai and more because it says out loud what the maintainers think is scarce: accountability.

that is the clean part. the human submitter owns the patch, the license still matters, and the sign-off still means something. good. but that is also the easy part. a rule about responsibility does not answer the operational question of what happens when ai makes patches cheaper to produce than they are to audit.

that is the real timing story here. the kernel is not discovering ai. it is formalizing a reality that already exists in a lot of contributor workflows. once that happens, the bottleneck moves from writing code to reading it carefully enough to trust it. if review bandwidth does not grow, the policy mostly redistributes blame. if it does grow, the social contract gets stricter and slower at the same time.

what people may be missing is that this is not just a permission question. it is a provenance question. a patch that looks clean can still hide shallow understanding, copied structure, or subtle edge cases no reviewer has time to unwind. the docs can force humans to own the result, but they cannot make human attention cheaper.

that is why the comments are worth reading. some people see a sensible liability shield, others see a review tax and a provenance problem. both takes are pointing at the same tradeoff. the headline says ai. the real story is who gets to trust what, and how much.

if you want the signal, check the [hn comments](https://news.ycombinator.com/item?id=47721953). the thread is better than the headline.
