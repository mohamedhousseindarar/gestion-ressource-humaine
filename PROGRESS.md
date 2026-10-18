# Avancement du projet SIRH

Ce fichier résume les travaux réalisés dans le dépôt jusqu’à présent. Il décrit l’état de la documentation, pas l’avancement d’une implémentation logicielle.

## Présentation et état initial

Le dépôt porte sur la **conception d’un logiciel de gestion des ressources humaines (SIRH)**. Lors de son analyse, il contenait principalement une arborescence de documents de projet et un README très succinct. Les dossiers couvrent l’analyse, le cahier des charges, l’architecture, les données, les outils, les tests et la gestion de projet. La plupart des fichiers étaient encore vides.

L’objectif retenu pour le travail actuel est de concevoir et documenter le SIRH avant de commencer son implémentation en code.

## Travaux réalisés

### Analyse

- [choix_modele_cycle_v.md](../Analyse/choix_modele_cycle_v.md) : justification du choix du modèle de cycle de vie en V, comparaison avec les modèles en cascade, agile, en spirale et incrémental, et présentation des conditions de réussite et des limites.
- [context.md](../Analyse/context.md) : contexte du besoin SIRH, problèmes liés à la dispersion possible des informations, apports attendus du système et raisons du choix du projet. Les fonctions citées sont indiquées comme des exemples à confirmer.
- [objectif.md](../Analyse/objectif.md) : objectif principal de concevoir et documenter le SIRH avant l’implémentation, objectifs spécifiques et résultat attendu de la phase de conception.
- [problematique.md](../Analyse/problematique.md) : problème traité, question centrale et questions auxquelles la conception doit répondre.

### Planification générale

- [plan_general.md](plan_general.md) : création du dossier `Plan/` et du plan général. Il présente le périmètre actuel, les phases et leurs livrables, les points de validation liés au modèle en V, les responsabilités envisagées, les critères de réussite et les modalités de suivi.

## État actuel

- La documentation établit le contexte général, les objectifs et la problématique du projet.
- Le modèle en V est retenu comme cadre de référence pour organiser conception et validation.
- Le plan général décrit l’enchaînement proposé, de l’analyse jusqu’aux étapes futures d’implémentation et de livraison.
- Le périmètre fonctionnel détaillé, les acteurs réels, les échéances, les responsabilités nominatives et les choix techniques restent à confirmer.
- Aucun code applicatif ni test logiciel n’a été réalisé dans le cadre des travaux consignés ici.

## Éléments restant à compléter

Les documents suivants sont présents dans le dépôt, mais restent à rédiger ou à valider :

- **Analyse** : acteurs et périmètre (`Analyse/acteurs.md`, `Analyse/perimetre.md`).
- **Cahier des charges** : exigences fonctionnelles et non fonctionnelles, contraintes et règles métier (`CahierCharges/`).
- **Architecture** : architecture générale, backend et sécurité (`Architecture/`).
- **Données** : dictionnaire de données (`BaseDonnee/dictionnaireDonnee.md`).
- **Outils** : choix et justification des outils (`Outils/choixOutils.md`).
- **Tests** : stratégie de test et critères de validation (`Test/strategieTest.md`).
- **Gestion de projet** : planning détaillé, tâches et risques (`gestionProjet/`).

Après clarification et validation de ces éléments, le plan détaillé pourra préciser les tâches, durées, ressources et échéances. La phase d’implémentation restera une étape ultérieure, guidée par la documentation validée.
