---
title: "La stack, le workflow et le déploiement — Dans les coulisses de ce site"
description: "Ce qui s'est vraiment passé lors de la construction de simonplourde.com — les outils choisis, comment le travail avec Claude s'est déroulé en pratique, et comment tout a été mis en ligne."
pubDate: 2026-06-14
---

Dans le dernier post, j'ai couvert la soirée en surface. Voici ce qui se passait vraiment sous le capot.

## Mon setup

- **PC Windows**
- **[Claude Cowork](https://claude.ai)** avec un abonnement Pro

## La stack

- **[Astro](https://astro.build)** — le framework. Génère des fichiers HTML statiques, sans base de données ni logique côté serveur. Simple, rapide, et facile à héberger.
- **[GitHub](https://github.com)** — là où vit le code. J'ai utilisé **[GitHub Desktop](https://desktop.github.com)** pour committer et pousser sans toucher à la ligne de commande.
- **[Cloudflare Workers & Pages](https://pages.cloudflare.com)** — l'hébergement. J'utilise déjà Cloudflare au travail pour le DNS, donc garder le domaine et l'hébergement au même endroit était un choix naturel.
- **[Wrangler](https://developers.cloudflare.com/workers/wrangler/)** — l'outil de déploiement de Cloudflare. Une seule commande pour builder et mettre le site en ligne.

## Comment le travail avec Claude s'est vraiment déroulé

Claude Cowork écrit les fichiers directement dans ton dossier connecté — dans mon cas, mon repo GitHub local. Le workflow : je décris ce que je veux, Claude écrit ou modifie les fichiers, je révise, je committe et je pousse.

Le dialogue était naturel. Je disais quelque chose comme "je veux un mode sombre et clair qui suit les paramètres système mais qu'on peut aussi changer manuellement" — et Claude gérait l'implémentation, expliquait ce qu'il avait fait, et signalait ce que je devais savoir. Quand quelque chose ne fonctionnait pas, je collais l'erreur et on déboguait ensemble.

Je n'ai jamais eu à lire de documentation. Je n'ai jamais eu à comprendre les variables CSS pour qu'elles fonctionnent. Le manque de connaissances n'a pas freiné la progression.

## Le déploiement

Une commande — `npx wrangler deploy` — build le site et le met en ligne. Claude a configuré le fichier de déploiement, j'ai lancé la commande, et le site était en ligne. Pointer le domaine était la partie la plus familière de toute la soirée — un enregistrement DNS dans Cloudflare, quelques minutes de propagation.

## La vraie conclusion

La stack n'a rien de magique — ce sont juste des outils. Ce qui a fait fonctionner la soirée, ce n'était pas une technologie en particulier, c'était d'avoir quelque chose qui pouvait combler l'écart entre ce que je voulais et ce qui devait être écrit. Claude gérait les connaissances web. Je gérais les décisions — ce que le site devait dire, comment il devait se sentir, ce qui comptait.

Si tu attends d'en "savoir assez" pour commencer à construire — tu en sais probablement déjà assez.

*Prochain épisode — un nouveau projet. Un que ma copine et moi allons vraiment utiliser. À suivre.*
