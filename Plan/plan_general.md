# Plan général du projet SIRH

## 1. Objet du plan

Ce document présente l’organisation générale du projet de conception d’un Système d’Information des Ressources Humaines (SIRH). Il définit les grandes phases, leurs objectifs et leurs principaux livrables afin de guider le travail depuis l’analyse du besoin jusqu’à la préparation de l’implémentation.

L’objectif immédiat du projet est de produire une documentation cohérente et validable avant d’écrire le code. La réalisation du logiciel constitue une phase ultérieure, qui ne sera engagée qu’après validation des besoins, du périmètre et des choix de conception.

## 2. Périmètre du projet

La phase actuelle comprend l’analyse des besoins et la préparation de la conception fonctionnelle et technique du SIRH. Elle couvre notamment la définition des acteurs, du périmètre, des exigences, des règles métier, de l’architecture envisagée, des données, des maquettes éventuelles et de la stratégie de vérification et de validation.

L’implémentation en code, le déploiement et l’exploitation ne font pas partie du résultat immédiat attendu. Ils sont décrits ici comme les étapes futures que la documentation doit préparer. Les fonctions exactes du SIRH restent à confirmer avec les acteurs concernés ; aucun calendrier ni aucune technologie définitive ne sont fixés dans ce plan.

## 3. Cycle de vie retenu

Le projet s’appuie sur le **modèle en V**. Les étapes de définition et de conception sont associées à des activités correspondantes de vérification et de validation. La préparation des tests commence donc dès la formalisation des exigences, même si leur exécution sur le logiciel interviendra après le développement.

| Étape de conception | Activité de validation associée |
| --- | --- |
| Analyse des besoins et exigences | Recette par rapport aux besoins des utilisateurs |
| Spécifications fonctionnelles | Tests système des fonctions attendues |
| Architecture et conception des composants | Tests d’intégration entre composants |
| Conception détaillée | Tests unitaires des composants |
| Implémentation future | Exécution des tests préparés et correction des écarts |

## 4. Phases et livrables

| Phase | Travaux principaux | Livrables attendus | Point de validation |
| --- | --- | --- | --- |
| 1. Cadrage et analyse | Identifier le contexte, les acteurs, les problèmes, les objectifs, les contraintes et le périmètre | Dossier d’analyse : contexte, problématique, objectifs, acteurs et périmètre | Les parties prenantes confirment le besoin et les limites du projet |
| 2. Spécification | Décrire les exigences fonctionnelles et non fonctionnelles, les règles métier et les critères d’acceptation | Cahier des charges et exigences traçables | Les exigences sont compréhensibles, cohérentes et validées |
| 3. Conception fonctionnelle | Décrire les parcours, les cas d’utilisation, les processus et, si utile, les maquettes | Modèles fonctionnels et maquettes validées | Les acteurs confirment que les parcours répondent à leurs besoins |
| 4. Conception technique et des données | Définir l’architecture, les composants, les choix techniques envisagés et le modèle de données | Architecture, dictionnaire de données et décisions techniques documentées | La conception est cohérente avec les exigences et les contraintes |
| 5. Préparation de la qualité et des tests | Associer les exigences aux méthodes de vérification, cas de test et critères de recette ; organiser les revues documentaires | Stratégie de test, matrice de traçabilité et plan d’assurance qualité | Chaque exigence importante peut être vérifiée |
| 6. Préparation de la réalisation | Décomposer le travail futur, ordonner les tâches, estimer les ressources et traiter les risques | Plan détaillé, planning à préciser et registre des risques | Le dossier permet d’estimer et de lancer l’implémentation |
| 7. Implémentation future | Développer les composants conformément aux spécifications et réaliser les tests prévus | Code, résultats de tests et documentation technique mise à jour | Les tests unitaires, d’intégration et système sont satisfaisants |
| 8. Recette et livraison futures | Faire valider le logiciel par les représentants métier, corriger les écarts et préparer la mise en service | Procès-verbal de recette, guide utilisateur et dossier de livraison | Les critères d’acceptation sont remplis et la livraison est autorisée |

## 5. Organisation et responsabilités

Les responsabilités précises seront attribuées lorsque l’équipe et les acteurs seront identifiés. À titre de répartition fonctionnelle :

- les **acteurs métier** expriment leurs besoins et valident les règles, les parcours et les critères d’acceptation ;
- le **responsable du projet** coordonne le travail, suit les livrables, les décisions, les échéances et les risques ;
- l’**équipe d’analyse et de conception** rédige les spécifications, les modèles et l’architecture ;
- l’**équipe de réalisation et de test**, lors de la phase future, implémente le système, exécute les tests et documente les résultats.

Une même personne peut assumer plusieurs rôles dans un projet de petite taille, mais la validation métier doit rester explicite.

## 6. Suivi, qualité et gestion des changements

L’avancement sera suivi à partir des livrables et des critères de validation de chaque phase. Les documents devront être relus pour vérifier leur clarté, leur cohérence entre eux et leur traçabilité aux besoins. Les décisions importantes et les changements de périmètre seront consignés ; toute modification d’une exigence devra entraîner la revue des modèles, choix techniques et tests concernés.

Les risques seront suivis pendant tout le projet, notamment les besoins incomplets ou changeants, les retards de validation, les difficultés liées aux données RH et les choix techniques non confirmés. Des actions de réduction seront définies dans le plan de gestion des risques.

## 7. Calendrier et ressources

Les dates, durées, ressources et dépendances détaillées ne sont pas indiquées dans le dépôt. Elles seront établies dans un plan détaillé après clarification du périmètre, identification des participants et estimation de la charge des livrables. Le présent plan fixe l’ordre logique du travail, sans inventer de dates.

## 8. Critères de réussite

La phase actuelle sera considérée comme réussie lorsque :

- le besoin, les acteurs et le périmètre auront été examinés et validés ;
- les exigences et règles métier seront documentées de façon compréhensible ;
- la conception fonctionnelle, l’architecture et les données seront cohérentes entre elles ;
- les exigences seront reliées à des moyens de vérification et à des critères d’acceptation ;
- les risques et les tâches de réalisation future seront identifiés ;
- la documentation permettra à une équipe de préparer l’implémentation sans devoir deviner les décisions métier principales.

## 9. Révision du plan

Ce plan général sera mis à jour si le périmètre, les acteurs, les contraintes ou les décisions d’architecture changent. Le plan détaillé, la stratégie de test et le plan de gestion des risques préciseront les éléments opérationnels propres à chaque domaine.
