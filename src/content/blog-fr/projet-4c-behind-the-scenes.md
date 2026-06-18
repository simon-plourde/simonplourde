---
title: "Projet 4C — Dans les coulisses"
description: "La stack, le workflow, et comment j'ai construit un outil de réconciliation des dépenses en couple sans aucune expérience React — encore une fois avec Claude."
pubDate: 2026-06-16
---

Même approche que pour [le site web](/fr/blog/behind-the-scenes/) : décrire ce que je veux, laisser Claude mener l'implémentation, et garder le contrôle sur les décisions. Projet différent, même processus.

## Mon setup

- **PC Windows**
- **[Claude Cowork](https://claude.ai)** avec un abonnement Pro

## La stack

- **[Next.js 15](https://nextjs.org)** — le framework. Basé sur React, gère le routing, la logique côté serveur et toute la structure de l'application.
- **[Supabase](https://supabase.com)** — base de données et authentification. Stocke toutes les transactions, catégories et données utilisateurs. Gère la connexion.
- **[Tailwind CSS](https://tailwindcss.com)** — le styling. CSS utilitaire qui permet de construire une interface propre rapidement sans écrire une feuille de style from scratch.
- **[PapaParse](https://www.papaparse.com)** — le parsing CSV. Gère la lecture des exports bancaires qu'on uploade chaque mois.
- **[Vercel](https://vercel.com)** — l'hébergement. Déploiements en un clic directement depuis GitHub.

## Comment le travail avec Claude s'est déroulé

Même workflow que pour le site — Claude écrit directement dans mon repo local, je révise, je committe et je pousse. Mais 4C est un projet plus complexe : authentification, base de données, logique d'application multi-pages, graphiques, ingestion de CSV.

Le dialogue était plus poussé. Je décrivais une fonctionnalité — "je veux pouvoir marquer une transaction comme commune ou personnelle et que ça se sauvegarde automatiquement" — et Claude gérait l'implémentation sur plusieurs fichiers. Quand quelque chose ne fonctionnait pas, on déboguait ensemble. Quand j'avais une opinion sur le design, je la donnais.

Je n'ai toujours pas eu à comprendre les React hooks pour les utiliser. Je n'ai jamais écrit une requête Supabase from scratch. L'écart entre ce que je voulais et ce qui a été construit est resté petit tout au long du projet.

## La vraie conclusion

Le site web était une preuve de concept — est-ce que je pouvais construire quelque chose de réel avec Claude et zéro expérience web ? 4C est la réponse. Une application full-stack avec auth, une base de données, de vraies données, et deux personnes qui l'utilisent réellement chaque mois.

Si le site a pris une soirée, 4C en a pris quelques-unes — mais l'approche était identique.
