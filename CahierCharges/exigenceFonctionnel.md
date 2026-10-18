# Exigences fonctionnelles

## 1. Cadre et statut des exigences

Ce document décrit les fonctions proposées pour la première version d’un logiciel de gestion des ressources humaines (GRH), dans le cadre d’un cas d’étude utilisant le Ministère de l’Énergie et des Ressources naturelles de Djibouti (MERN) comme exemple. Le MERN n’est pas un client confirmé. Aucune exigence ci-dessous n’a été recueillie ou validée par le Ministère ; ces exigences sont des hypothèses de conception à préciser si le projet est appliqué à une organisation réelle.

Les exigences sont formulées de manière vérifiable. Leur priorité est considérée comme nécessaire au périmètre proposé, mais devra être réévaluée lors d’une validation métier réelle. Les règles détaillées concernant les congés, les absences et les données conservées restent à préciser.

## 2. Acteurs concernés

- **Administrateur** : administre les comptes, les rôles et les permissions.
- **Responsable RH** : supervise les dossiers et le traitement des opérations RH.
- **Agent RH** : réalise les opérations RH courantes autorisées.
- **Responsable de service** : consulte les informations nécessaires au suivi des agents de son service et intervient sur les demandes qui lui sont attribuées.
- **Agent du ministère** : consulte son propre dossier et soumet les demandes proposées.
- **Direction du ministère** : consulte les tableaux de bord et rapports autorisés.

Ces profils sont hypothétiques. Les droits exacts sont des choix de conception proposés dans ce document, et non des pratiques vérifiées au MERN.

## 3. Exigences fonctionnelles

### 3.1 Dossiers des employés

| ID | Exigence |
| --- | --- |
| EF-01 | Le système doit permettre à un Agent RH ou à un Responsable RH autorisé de créer un dossier d’employé avec les informations obligatoires définies par le modèle de données. |
| EF-02 | Le système doit permettre aux utilisateurs RH autorisés de consulter et de modifier les dossiers selon leurs permissions. |
| EF-03 | Le système doit permettre de rechercher et de filtrer les dossiers selon les critères autorisés, par exemple le nom, le service ou le statut professionnel. |
| EF-04 | Le système doit permettre à un Agent du ministère de consulter uniquement les informations de son propre dossier qui lui sont accessibles. |
| EF-05 | Le système doit permettre aux utilisateurs RH autorisés de rattacher un employé à un service et à un poste. |
| EF-06 | Le système doit signaler les données obligatoires manquantes et les doublons détectés selon les identifiants retenus. |

### 3.2 Services et postes

| ID | Exigence |
| --- | --- |
| EF-07 | Le système doit permettre au Responsable RH ou à l’Agent RH autorisé de créer, consulter, modifier et désactiver les services et les postes. |
| EF-08 | Le système doit permettre de consulter les employés affectés à un service ou à un poste, selon les permissions de l’utilisateur. |
| EF-09 | Le système doit permettre à un Responsable de service de consulter les informations professionnelles des agents rattachés à son service, dans les limites de ses droits. |

### 3.3 Congés et absences

| ID | Exigence |
| --- | --- |
| EF-10 | Le système doit permettre à un Agent du ministère de soumettre une demande de congé ou de déclarer une absence selon les types de démarches activés. |
| EF-11 | Le système doit permettre à l’employé de consulter l’état et l’historique de ses propres demandes. |
| EF-12 | Le système doit permettre aux acteurs habilités de consulter les demandes qui leur sont attribuées et d’enregistrer une décision ou un commentaire. |
| EF-13 | Le système doit permettre aux utilisateurs RH autorisés de consulter et de mettre à jour le suivi administratif des congés et absences. |
| EF-14 | Le système doit présenter l’état de chaque demande (par exemple soumise, en examen, acceptée, refusée ou annulée) et conserver les changements d’état. |

### 3.4 Comptes et permissions

| ID | Exigence |
| --- | --- |
| EF-15 | Le système doit permettre à un Administrateur autorisé de créer, modifier, désactiver et réactiver un compte utilisateur. |
| EF-16 | Le système doit permettre à l’Administrateur d’attribuer un ou plusieurs rôles définis au compte d’un utilisateur. |
| EF-17 | Le système doit appliquer les permissions associées au rôle avant d’autoriser la consultation ou la modification d’une fonction ou d’une donnée. |
| EF-18 | Le système doit empêcher un utilisateur désactivé d’accéder au système. |

### 3.5 Tableaux de bord et rapports

| ID | Exigence |
| --- | --- |
| EF-19 | Le système doit afficher à chaque rôle un tableau de bord limité aux indicateurs autorisés pour ce rôle. |
| EF-20 | Le système doit permettre de produire des rapports simples à partir des données incluses dans le périmètre, notamment des effectifs par service et des états de suivi des demandes, sous réserve des permissions. |
| EF-21 | Le système doit permettre de filtrer les rapports selon des critères disponibles et autorisés. |

### 3.6 Historique des opérations

| ID | Exigence |
| --- | --- |
| EF-22 | Le système doit enregistrer les opérations importantes définies comme traçables, notamment les créations et modifications de dossiers, changements de permissions et décisions sur les demandes. |
| EF-23 | Chaque entrée d’historique doit associer l’opération à l’utilisateur, à la date et à l’heure, à l’objet concerné et au type d’action. |
| EF-24 | Le système doit permettre aux seuls utilisateurs habilités de consulter l’historique et de le filtrer selon les critères autorisés. |

## 4. Hors périmètre fonctionnel

La première version ne couvre pas la paie complète ni les déclarations fiscales, la comptabilité et le budget, les stocks, le carburant et les achats, le recrutement en ligne de candidats externes, l’interconnexion automatique avec les systèmes d’autres ministères, ni une application mobile dédiée. Ces exclusions ne préjugent pas d’évolutions futures.

## 5. Points à préciser

Avant une utilisation réelle, il faudrait notamment définir les champs du dossier employé, les identifiants uniques, les statuts professionnels, les types et règles de congés/absences, le circuit de décision, les délégations, les indicateurs et rapports attendus, la durée de conservation des données et journaux, ainsi que la matrice détaillée des permissions. Les références à des décisions « acceptées » ou « refusées » décrivent un mécanisme générique et ne fixent aucune règle administrative ou légale du MERN.
