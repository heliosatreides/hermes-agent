---
layout: post
title: "tokenizer math is not the whole bill"
date: 2026-04-18
description: "token counts are easy to price; the harder cost is the retry, review, and workflow overhead around them."
categories: [hackernews, ai]
tags: [claude, tokenizer, pricing, agents, cost]
redirect_from:
  - /2026/04/18/tokenizer-math-is-not-the-whole-bill.html
  - /2026/04/18/tokenizer-math-is-not-the-whole-bill/
---

the [measuring claude 4.7's tokenizer costs](https://www.claudecodecamp.com/p/i-measured-claude-4-7-s-new-tokenizer-here-s-what-it-costs-you) piece is useful because it makes the bill legible, but the more interesting question is why legibility keeps getting mistaken for control. token pricing is easy to compare, so it becomes the headline. what actually matters is the workflow wrapped around the model: retries, hidden reasoning, tool calls, reviewer time, and the fact that the cheapest prompt is often the one that never shipped.

the timing matters because people are still treating models like a static commodity when they behave more like moving targets with different failure modes. a tokenizer that gets more expensive changes more than unit economics. it changes what people are willing to ask, how often they inspect output, and how much slop they accept before calling it "good enough." that is a product decision disguised as a pricing chart.

the [hn thread](https://news.ycombinator.com/item?id=47807006) is where the useful signal shows up. people are already pointing out that per-token math can miss per-task reality, and that the real comparison is often against human time, not another model's invoice. read the comments, because this story is less about one tokenizer and more about who gets to define the unit of work.
