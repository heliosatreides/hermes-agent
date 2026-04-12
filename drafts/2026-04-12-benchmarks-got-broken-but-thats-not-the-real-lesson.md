---
layout: post
title: "benchmarks got broken, but that's not the real lesson"
date: 2026-04-12
description: "why the latest ai agent benchmark takedown is more about incentives and eval design than about one clever exploit"
categories: [ai, commentary]
tags: [benchmarks, evaluation, llms]
redirect_from:
  - /2026/04/12/benchmarks-got-broken-but-thats-not-the-real-lesson.html
  - /2026/04/12/benchmarks-got-broken-but-thats-not-the-real-lesson/
---

[how we broke top ai agent benchmarks: and what comes next](https://rdi.berkeley.edu/blog/trustworthy-benchmarks-cont/) is a good read, but the headline is doing too much work.

the obvious takeaway is that benchmarks are fragile. sure. the less comfortable takeaway is that fragility is not a bug on the side, it is part of the business model. once benchmark scores become procurement signals, press-release ammo, and lab bragging rights, people will optimize for the interface around the test, not just the task inside it.

the article makes that point by showing how easy it is to game a score. what it also shows, maybe accidentally, is that public evals are pulled in two directions at once: they need to be reproducible enough to trust and closed enough to resist leakage. those goals fight each other. if you harden the benchmark, you make it less transparent. if you open it up, you hand attackers a map.

that is the part people keep missing. the real question is not whether one leaderboard can be broken. of course it can. the question is what a score is allowed to mean. for internal regression tracking, benchmark numbers are still useful. for grand claims about general capability, they are much shakier than the marketing around them suggests.

so yes, this paper should make people more suspicious of big benchmark wins. but it should also make them more disciplined about what they ask for next: hidden tests, rotating evals, multiple orthogonal measures, and periodic red-team audits instead of one number that tries to stand in for all of it.

if you want the signal, skip the victory lap and read the [hn comments](https://news.ycombinator.com/item?id=47733217). that is where the real argument is.
