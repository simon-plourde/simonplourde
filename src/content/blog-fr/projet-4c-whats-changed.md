---
title: "Projet 4C — Ce qui a changé depuis le premier aperçu"
description: "Logos de marchands, connexion Google, un moteur de règles, l'historique des règlements — beaucoup de choses ont été ajoutées depuis la première preview."
pubDate: 2026-06-20
---

[Le premier aperçu](/fr/blog/projet-4c-first-look/) montrait la boucle principale en fonctionnement. Beaucoup de choses ont été ajoutées depuis.

## Logos des marchands

Chaque transaction affiche maintenant un petit logo à côté du nom du marchand. Sous le capot, l'application associe les noms de marchands à leur domaine et récupère le favicon via le service d'icônes de Google. C'est un petit détail, mais ça rend la liste des transactions beaucoup plus facile à parcourir — on reconnaît les marchands visuellement avant même de lire le nom.

![Logos des marchands dans la liste des transactions](/4c-merchant-logos.PNG)

Ce n'est pas parfait. Les petits marchands ou ceux sans domaine connu affichent une icône générique. Mais pour le quotidien — épicerie, restos, abonnements — ça fonctionne bien.

## Connexion Google

La connexion se fait maintenant via Google OAuth. Un clic, pas de mot de passe à retenir. Il reste une option email/mot de passe local cachée derrière un lien pour les cas particuliers, mais en pratique on utilise juste Google.

![Écran de connexion Google](/google-login.PNG)

## Moteur de règles

Celui-là a changé la façon dont l'application se ressent au quotidien. Le moteur de règles permet de définir comment certains marchands doivent toujours être catégorisés et divisés. "Virgin Plus" est toujours Personnel, toujours Utilitaires. "Marché d'alimentation" est toujours Commun, toujours Épicerie.

Une fois les règles configurées, uploader un nouveau CSV catégorise tout automatiquement sans révision manuelle. L'app suggère aussi de nouvelles règles basées sur les marchands non catégorisés ou souvent mal tagués — donc elle devient plus intelligente avec l'usage.

## Historique des règlements

Il y a maintenant un historique complet des règlements. Chaque mois, on marque le solde comme réglé, et ça se logue avec le montant, qui a payé, et quand. Utile pour vérifier qu'on n'a rien manqué.

## La suite

L'expérience de base est solide. Ce qui reste, c'est du polish — meilleur support mobile, quelques cas limites, et rendre l'invitation d'un deuxième utilisateur plus simple sans avoir à toucher Supabase directement. Plus de détails quand c'est fait.
