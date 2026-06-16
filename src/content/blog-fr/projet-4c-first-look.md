---
title: "Projet 4C — Premier aperçu de l'outil"
description: "Un premier aperçu de Projet 4C, l'outil de réconciliation des dépenses en couple que j'ai construit avec Claude pour remplacer notre calvaire mensuel sur Google Sheets."
pubDate: 2026-06-15
---

Le dernier post expliquait pourquoi Projet 4C existe. Celui-ci montre à quoi ça ressemble concrètement.

## Ce que ça fait

Projet 4C a un seul objectif : éliminer la friction dans la séparation des dépenses communes en couple.

Chaque mois, ma copine et moi uploadons chacun l'export CSV de nos cartes de crédit. L'outil les ingère, catégorise chaque transaction automatiquement, sépare les dépenses communes des dépenses personnelles, et nous dit qui doit combien à l'autre.

Plus besoin de passer les transactions une par une. Plus de Google Sheet manuel. Juste uploader, réviser, régler.

## Le tableau de bord

La première chose qu'on voit en ouvrant 4C, c'est le dashboard. D'un coup d'œil : les dépenses de chaque personne ventilées entre commun et personnel, et le montant du règlement au centre — qui doit quoi à qui. En dessous, les dépenses par catégorie pour les deux personnes côte à côte, une comparaison avec le mois précédent, et la liste des commerces les plus fréquentés.

![Tableau de bord 4C](/4c-dashboard.png)

## La vue des transactions

Chaque transaction est listée avec sa date, le commerçant, la carte, le montant, le type de dépense (commune ou personnelle) et la catégorie. Tout est filtrable — par personne, carte, type ou catégorie. On peut aussi corriger manuellement ce que la catégorisation automatique a mal interprété, directement dans la liste.

![Transactions 4C](/4c-transactions.png)

## L'écran d'upload

Chaque mois, on télécharge chacun le CSV de notre banque et on le glisse dans l'outil. Il gère le parsing, la déduplication et la catégorisation automatiquement. L'historique des uploads garde une trace de ce qui a déjà été importé.

![Upload 4C](/4c-upload.png)

## Les tendances de dépenses

Une fois quelques mois de données accumulés, l'onglet Tendances devient vraiment intéressant. Tendances par catégorie dans le temps, composition mensuelle, moyennes glissantes. Le genre de visibilité qu'on n'a pas quand on regarde juste un tableur.

![Tendances 4C](/4c-trends.png)

## Où on en est

La boucle principale fonctionne de bout en bout. Uploader les CSV, réviser, régler. La vue des tendances montre déjà des patterns qu'on ne voyait pas avant.

D'autres fonctionnalités sont en cours — mais ça, c'est pour un prochain post.
