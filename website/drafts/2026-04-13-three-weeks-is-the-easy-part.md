---
layout: post
title: "three weeks is the easy part"
date: 2026-04-13
description: "ai can compress the first draft, but it does not compress trust, support, or edge cases."
categories: [ai, software]
tags: [claude, codex, product, startup, tradeoffs]
redirect_from:
  - /2026/04/13/three-weeks-is-the-easy-part.html
  - /2026/04/13/three-weeks-is-the-easy-part/
---

the most interesting part of [this show hn post](https://news.ycombinator.com/item?id=47749674) is not the headline. it is the quiet admission that the author wrote specs, an architecture doc, and a style guide before letting claude and codex fill in the blanks. that is the real pattern here: ai does not remove judgment, it rewards people who already know where the judgment belongs.

a lot of readers hear "3 weeks" and translate it into "the work got cheaper." that is too simple. what actually got cheaper was the first draft. the expensive parts of software were still there, just pushed into a thinner slice of the stack: permissions, audit trails, rate limits, onboarding, retries, data hygiene, and the long tail of support questions that arrive after the demo. for tools that touch customer accounts, those are not extras. those are the product.

there is also a timing trap. a solo builder can now move fast enough to make a project look complete before it has been tested by real use. that changes the meaning of shipping. it is easier to confuse "finished enough to launch" with "structured enough to survive contact with users." the comments already point at the useful questions: multi-account support, self-hosting, x support, rust, maintenance. that is where the signal lives, not in the number of weeks.

the tempting takeaway is that ai has finally made one person look like a team. the better takeaway is smaller and more annoying: it has made preparation matter more. the people who will win with these tools are not the ones who can generate the most code, but the ones who can delete the most nonsense before the model ever touches the keyboard. if you read the thread, skip the applause and look for the tradeoffs. that's where the real story is.
