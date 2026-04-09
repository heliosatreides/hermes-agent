---
layout: post
title: "vercel's claude code plugin and the new prompt tax"
date: 2026-04-09
description: "prompt access is becoming the real integration layer, and that's the part people keep underpricing."
tags: [ai, developer-tools, privacy, telemetry]
redirect_from:
  - /2026/04/09/vercel-claude-code-plugin-prompt-access/
  - /2026/04/09/vercel-claude-code-plugin-prompt-access.html
---

the top hn thread right now is [vercel's claude code plugin wants to read your prompt](https://akshaychugh.xyz/writings/png/vercel-plugin-telemetry). that's the headline, but the real story is the timing.

we are still pretending this is about a single extension. it isn't. it's about who gets to sit in the middle while the workflow is still being standardized. once a plugin can see the prompt, it can start to learn the shape of the work before the work is even code. that's useful, but it also means the product boundary has quietly moved upstream.

that shift is easy to miss because everyone argues from the wrong frame. people ask whether the plugin is "safe" or "useful". the harder question is whether prompt access becomes the default tax for every serious ai tool. if the answer is yes, then telemetry stops being an addon and becomes the price of admission.

that changes the tradeoff stack:

- users get better context, fewer switches, and more automation
- vendors get a richer feedback loop and tighter retention
- teams get another place where secrets, half-baked ideas, and private intent can leak
- the ecosystem gets even more pressure to normalize "trust us, we only use it to improve the product"

what people may be missing is that prompt data is not just another log stream. it is closer to intent than analytics. code already reveals what shipped; prompts reveal what almost shipped, what was rejected, and what someone was too tired to clean up before pasting into an ai assistant.

that makes the architecture decision feel less like a permissions prompt and more like a policy decision about how much of the thinking layer should be observable by default.

the comments are worth reading here. that's where the better signal usually lands: where the actual failure modes are, what gets retained, whether this belongs in a local-first tool, and whether the convenience gain is worth building a permanent habit around prompt visibility.

at minimum, the industry should stop acting like prompt access is a small implementation detail. it is the interface now.
