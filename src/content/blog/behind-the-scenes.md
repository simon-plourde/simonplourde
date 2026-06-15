---
title: "The Stack, the Workflow, and the Deploy — Behind the Scenes of Building This Site"
description: "What actually went into building simonplourde.com — the tools chosen, how working with Claude looked in practice, and how it all got deployed live."
pubDate: 2026-06-14
---

Last post I covered the evening at a high level. Here's what was actually happening under the hood.

## My setup

- **Windows PC**
- **[Claude Cowork](https://claude.ai)** with a Pro subscription

## The stack

- **[Astro](https://astro.build)** — the framework. Outputs plain HTML files, no database or server-side logic. Simple, fast, and easy to host.
- **[GitHub](https://github.com)** — where the code lives. I used **[GitHub Desktop](https://desktop.github.com)** to commit and push without touching the command line.
- **[Cloudflare Workers & Pages](https://pages.cloudflare.com)** — hosting. I already used Cloudflare at work for DNS, so keeping the domain and hosting in the same platform was a natural choice.
- **[Wrangler](https://developers.cloudflare.com/workers/wrangler/)** — Cloudflare's deployment tool. One command to build and push the site live.

## How working with Claude actually looked

Claude Cowork writes files directly into your connected folder — in this case, my local GitHub repo. So the workflow was: I describe what I want, Claude writes or edits the files, I review, commit, and push.

The back-and-forth felt natural. I'd say something like "I want a dark and light mode that follows the system setting but can also be toggled manually" — and Claude would handle the implementation, explain what it did, and flag anything I needed to know. When something broke, I'd paste the error and we'd debug it together.

I never had to go read documentation. I never had to understand CSS variables to have them work. The knowledge gap didn't stop the progress.

## The deployment

One command — `npx wrangler deploy` — builds the site and pushes it live. Claude configured the deployment file, I ran the command, and the site was up. Pointing the domain was the most familiar part of the whole evening — DNS record in Cloudflare, a few minutes to propagate.

## The honest takeaway

The stack isn't magic — it's just tools. What made the evening work wasn't any particular technology, it was having something that could bridge the gap between what I wanted and what needed to be written. Claude handled the web knowledge. I handled the judgment calls — what the site should say, how it should feel, what mattered.

If you've been waiting until you "know enough" to start building — you probably already do.

*Next up — a new project. One my girlfriend and I will actually use. More on that soon.*
