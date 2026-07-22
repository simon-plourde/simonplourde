---
title: "Projet 4C — The App Got a Full Redesign"
description: "New design, smarter autocategorization, a cash flow diagram, and more — the app got rebuilt from scratch."
pubDate: 2026-07-22
---

The [last update](/blog/projet-4c-whats-changed/) covered merchant logos, Google sign-in, and the rules engine. Since then, the whole thing got rebuilt from scratch — new design, smarter categorization, and a few new features worth showing.

## A new look

The previous version worked, but it looked like a prototype. This time I used Claude Fable 5 to rethink the interface entirely — cleaner layout, a proper sidebar, better use of space. It feels like an actual product now rather than something held together with duct tape.

![4C Dashboard](/4c-dashboard-v2.png)

## Better rules and autocategorization

The rules engine was already there, but it's gotten smarter. Merchants get categorized automatically on upload with much higher accuracy than before. The "Re-apply rules" button on the Transactions page lets you retroactively fix everything with one click when you add or update a rule — no need to re-upload.

![Transactions](/4c-transactions-v2.png)

## New on Trends: cash flow

The Trends page now includes a Sankey diagram showing where money actually goes — broken down by person and category across all months. It makes patterns obvious in a way that tables never could.

![Trends and cash flow](/4c-trends-v2.png)
