# Exigences non fonctionnelles

## 1. Cadre

Ce document complète les exigences fonctionnelles du cas d’étude SIRH. Il ne constitue pas une validation du MERN ni une déclaration de conformité à une loi particulière. Les objectifs chiffrés ci-dessous sont des **cibles de conception provisoires** : ils devront être confirmés avec les parties prenantes et adaptés à l’infrastructure retenue avant la réalisation.

## 2. Exigences proposées

| ID | Domaine | Exigence vérifiable | Vérification prévue |
| --- | --- | --- | --- |
| ENF-01 | Sécurité | Toute fonction protégée doit vérifier l’authentification, l’état actif du compte, la permission et la portée des données côté serveur. Un contrôle d’accès refusé ne doit pas révéler les données demandées. | Tests d’accès autorisé/refusé pour chaque rôle et chaque portée. |
| ENF-02 | Sécurité | Les secrets d’authentification ne doivent jamais être stockés en clair. Les mots de passe doivent être protégés par un algorithme de hachage adapté à cet usage ; les secrets de l’application doivent être séparés du code source. | Revue de configuration et inspection du stockage en environnement de test. |
| ENF-03 | Confidentialité | Les échanges avec l’application doivent être chiffrés en transit dans tout environnement déployé. Les sauvegardes contenant des données personnelles doivent être protégées contre l’accès non autorisé. | Revue de configuration du déploiement et vérification des droits d’accès aux sauvegardes. |
| ENF-04 | Traçabilité | Une opération définie comme traçable doit produire une entrée comprenant l’acteur, l’horodatage, l’action et l’objet concerné. Un utilisateur ordinaire ne doit pas pouvoir modifier ni supprimer cette entrée via l’application. | Tests fonctionnels et revue des événements produits. |
| ENF-05 | Intégrité | Les validations métier doivent être appliquées côté serveur. Une erreur de validation ou d’autorisation ne doit pas laisser une modification partielle des données. | Tests de validation et tests d’échec des opérations. |
| ENF-06 | Performance | Avec un jeu de données et une charge de référence à définir, au moins 95 % des consultations courantes doivent répondre en moins de 2 secondes, hors temps de réseau externe. La charge de référence doit être fixée avant les tests de performance. | Mesure instrumentée sur l’environnement cible ou un environnement représentatif. |
| ENF-07 | Disponibilité | La disponibilité attendue et les plages de service doivent être décidées avant le choix de l’hébergement. Aucun taux de disponibilité n’est fixé tant que cet usage n’est pas précisé. | Revue de l’architecture et mesure selon une période d’observation convenue. |
| ENF-08 | Sauvegarde et reprise | Une stratégie doit définir la fréquence des sauvegardes, leur durée de conservation, les responsabilités et les objectifs de reprise (perte maximale de données et délai de restauration). Une restauration doit être éprouvée avant mise en service. | Exercice documenté de restauration et comparaison aux objectifs convenus. |
| ENF-09 | Utilisabilité | Les formulaires doivent identifier les champs obligatoires, expliquer les erreurs en termes compréhensibles et conserver les données déjà saisies lorsqu’une validation échoue, lorsque cela est techniquement possible sans compromettre la sécurité. | Scénarios d’usage et revue avec des utilisateurs représentatifs. |
| ENF-10 | Compatibilité | L’interface web doit fonctionner sur les navigateurs et tailles d’écran qui seront retenus dans la matrice de compatibilité du projet. Cette matrice reste à établir avant les tests système. | Tests sur la matrice de navigateurs et d’écrans validée. |
| ENF-11 | Maintenabilité | Les décisions d’architecture, la configuration nécessaire à l’exécution et les procédures de déploiement et de restauration doivent être documentées et versionnées avec le projet, sans secrets ni données réelles. | Revue documentaire et déploiement reproductible en environnement non productif. |
| ENF-12 | Protection des données | Seules les données nécessaires aux fonctions approuvées doivent être collectées. Les durées de conservation, règles d’archivage et modalités de suppression doivent être définies avant l’utilisation de données réelles. | Revue du dictionnaire de données et vérification des procédures retenues. |

## 3. Décisions à valider

Avant la conception technique détaillée, les parties prenantes doivent confirmer les cibles de performance, la charge attendue, les plages de service, les objectifs de reprise, les navigateurs pris en charge et les règles applicables aux données personnelles. Les valeurs proposées dans ce document ne doivent pas être interprétées comme des engagements contractuels ou des obligations légales.
