# Contraintes et hypothèses

## 1. Statut

Le projet est actuellement une phase de conception documentaire d’un cas d’étude SIRH. Le Ministère de l’Énergie et des Ressources naturelles de Djibouti (MERN) est un contexte d’illustration, pas un client confirmé. Les contraintes ci-dessous distinguent les limites connues du projet des décisions qui restent à prendre. Elles ne valent ni validation ministérielle ni avis de conformité juridique.

## 2. Contraintes établies par le projet

- **Périmètre de travail :** produire une documentation cohérente avant de commencer l’implémentation. Le code, le déploiement et l’exploitation sont des étapes ultérieures.
- **Périmètre fonctionnel proposé :** dossiers des employés, services et postes, congés et absences, comptes et permissions, rapports simples et historique, selon les limites décrites dans `exigenceFonctionnel.md`.
- **Données personnelles :** la conception doit limiter les accès par rôle et par portée, prévoir la traçabilité des opérations importantes et éviter l’usage de données réelles tant que les protections et autorisations nécessaires ne sont pas établies.
- **Technologies :** aucune technologie, plateforme d’hébergement ou infrastructure n’est encore arrêtée. Les choix doivent être justifiés dans les documents d’architecture et d’outillage avant l’implémentation.
- **Calendrier et ressources :** dates, budget, équipe, volumes de données et charge utilisateur ne sont pas renseignés ; aucune estimation ne doit être considérée comme approuvée.
- **Fonctions exclues :** la paie complète, les déclarations fiscales, la comptabilité, les stocks, les achats, le recrutement externe, les échanges automatiques avec d’autres ministères et une application mobile dédiée sont hors du périmètre initial proposé.

## 3. Hypothèses de conception à confirmer

- Le système est envisagé comme une application web accessible à plusieurs catégories d’utilisateurs.
- Les comptes sont nominatifs et les permissions sont vérifiées sur le serveur, en tenant compte de l’utilisateur, de son rôle et de la portée des données.
- Les informations de démonstration pourront être fictives ; les données personnelles réelles ne seront introduites qu’après validation des exigences de sécurité, de conservation et d’accès.
- Les règles détaillées de gestion RH ne sont pas déduites du contexte géographique ni du nom du ministère. Elles devront être fournies ou approuvées par les parties prenantes d’une organisation réellement concernée.

## 4. Décisions bloquantes avant réalisation

Avant de lancer l’implémentation, il faudra au minimum :

1. valider le périmètre, les acteurs et les parcours fonctionnels ;
2. définir les données collectées, les champs obligatoires, les identifiants et les règles de détection des doublons ;
3. définir les types de congés et absences, leurs états, les transitions autorisées, le circuit de décision, les délais, les justificatifs, les règles de chevauchement et les modalités de correction ;
4. approuver une matrice d’accès par rôle, action, catégorie de données et portée ;
5. fixer les règles de conservation, d’archivage, de suppression, de sauvegarde et de reprise ;
6. confirmer les contraintes réglementaires et organisationnelles applicables auprès des responsables compétents ;
7. arrêter les objectifs de performance, disponibilité, compatibilité, l’infrastructure et les ressources du projet.

Toute décision qui n’a pas été confirmée doit rester identifiée comme hypothèse ou point ouvert dans les documents suivants ; elle ne doit pas être transformée implicitement en règle métier.
