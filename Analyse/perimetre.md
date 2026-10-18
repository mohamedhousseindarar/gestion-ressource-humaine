## Cadre du périmètre

Ce document définit le périmètre fonctionnel proposé pour la première version du logiciel de gestion des ressources humaines (GRH), conçu comme un exemple pour le Ministère de l’Énergie et des Ressources naturelles de Djibouti (MERN). Le MERN constitue un contexte d’illustration et n’est pas un client confirmé. Les fonctions décrites sont donc des propositions de conception, et non des besoins vérifiés ou validés par le Ministère.

Le périmètre précise les services que la première version du logiciel devra couvrir et les domaines qu’elle laissera de côté. Cette délimitation aide à concentrer la conception sur les besoins RH retenus, à éviter d’étendre le projet à des fonctions sans lien direct avec cette première version et à préparer une estimation plus claire de sa réalisation.

## Fonctions incluses dans la première version

La première version du logiciel couvrira les fonctions suivantes :

### Gestion des employés et de leurs dossiers

Le système permettra de créer, consulter et mettre à jour les dossiers des employés. Les informations conservées devront être définies dans le dictionnaire de données. Leur consultation et leur modification seront limitées selon les rôles et les permissions attribués.

### Gestion des services et des postes

Le système permettra de représenter les services de l’organisation et les postes qui leur sont associés. Ces informations pourront servir à organiser les dossiers des employés et à situer leur affectation dans la structure proposée.

### Gestion des congés et des absences

Le système permettra d’enregistrer et de suivre les congés et les absences. Les types de demandes, leurs étapes de traitement, les règles applicables et les personnes autorisées à les examiner restent à préciser dans les exigences et les règles métier.

### Gestion des utilisateurs et des permissions

Le système permettra de gérer les comptes utilisés pour accéder au logiciel et les permissions associées aux rôles. Les droits devront suivre le principe selon lequel chaque utilisateur accède uniquement aux fonctions et informations nécessaires à ses responsabilités.

### Tableau de bord et rapports simples

Le système proposera un tableau de bord et des rapports simples pour consulter des informations de suivi liées aux fonctions incluses. Le contenu exact de ces vues, les indicateurs à afficher et les conditions d’accès restent à définir. Les rapports devront respecter les règles de confidentialité des données RH.

### Historique des opérations importantes

Le système conservera une trace des opérations importantes effectuées, par exemple certaines créations, modifications ou actions de traitement. La liste des opérations à tracer, les informations enregistrées et les personnes autorisées à consulter cet historique devront être définies lors de la conception détaillée.

## Éléments exclus de la première version

Les fonctions suivantes ne font pas partie du périmètre initial :

- **Paie complète et déclarations fiscales** : le logiciel ne calculera pas l’ensemble des éléments de paie et ne produira pas les déclarations fiscales associées.
- **Gestion comptable et budgétaire du ministère** : il ne remplacera pas un système comptable ou budgétaire et ne prendra pas en charge le suivi général des budgets.
- **Gestion des stocks, du carburant et des achats** : ces activités ne relèvent pas des fonctions RH retenues pour la première version.
- **Recrutement en ligne avec candidatures externes** : le système ne proposera pas de portail public de recrutement ni de gestion de candidatures provenant de personnes extérieures.
- **Interconnexion automatique avec les systèmes d’autres ministères** : aucun échange automatisé de données avec des systèmes externes n’est prévu dans ce périmètre.
- **Application mobile dédiée** : la première version ne comprendra pas d’application conçue spécifiquement pour les téléphones mobiles.

## Évolutions possibles

Les éléments exclus pourront être réexaminés dans une version ultérieure si un besoin est établi, si les acteurs concernés le confirment et si les contraintes techniques, organisationnelles et de sécurité sont étudiées. Leur mention ici ne signifie pas qu’ils sont planifiés ou approuvés.
