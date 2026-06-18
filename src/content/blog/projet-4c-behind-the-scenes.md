---
title: "Projet 4C — Behind the Scenes"
description: "The stack, the workflow, and how I built a couples expense reconciliation tool with zero prior React experience — again using Claude."
pubDate: 2026-06-16
---

Same approach as the website: describe what I want, let Claude lead on the implementation, and stay in the driver's seat on the decisions. Different project, same process.

## My setup

- **Windows PC**
- **[Claude Cowork](https://claude.ai)** with a Pro subscription

## The stack

- **[Next.js 15](https://nextjs.org)** — the framework. React-based, handles routing, server-side logic, and the full app structure.
- **[Supabase](https://supabase.com)** — database and authentication. Stores all transactions, categories, and user data. Handles login.
- **[Tailwind CSS](https://tailwindcss.com)** — styling. Utility-first CSS that makes building a clean UI fast without writing a stylesheet from scratch.
- **[PapaParse](https://www.papaparse.com)** — CSV parsing. Handles reading the bank export files we upload each month.
- **[Vercel](https://vercel.com)** — hosting. One-click deploys straight from GitHub.

## How working with Claude looked

Same workflow as the website — Claude writes directly into my local repo, I review, commit, and push. But 4C is a more complex project: user authentication, a database, multi-page app logic, charts, CSV ingestion.

The back-and-forth was more involved. I'd describe a feature — "I want to be able to flag a transaction as shared or personal and have that save automatically" — and Claude would handle the implementation across multiple files. When something broke, we debugged together. When I had a design opinion, I said so.

I still never had to understand React hooks to use them. I never had to write a Supabase query from scratch. The gap between what I wanted and what got built stayed small the whole time.

## The honest takeaway

The website was a proof of concept — could I build something real with Claude and zero web experience? 4C is the answer. A full-stack app with auth, a database, real data, and two people actually using it every month.

If the website was one evening, 4C was a few — but the approach was identical.
