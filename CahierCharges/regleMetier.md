# Règles métier

## 1. Cadre

Les règles ci-dessous sont des propositions pour le cas d’étude de SIRH décrit dans le dépôt. Le Ministère de l’Énergie et des Ressources naturelles de Djibouti (MERN) sert de contexte d’exemple et n’est pas un client confirmé. Ces règles ne décrivent pas des procédures vérifiées ou approuvées par le Ministère. Elles devront être adaptées si le système est destiné à une organisation réelle.

Les règles portent sur le périmètre initial : dossiers des employés, services et postes, congés et absences, utilisateurs et permissions, rapports et historique. Les règles légales, conventionnelles ou propres à l’administration djiboutienne ne sont pas définies ici.

## 2. Règles proposées

### Dossiers des employés

- **RM-01 — Unicité du dossier :** chaque employé possède un dossier unique dans le système. L’identifiant permettant de détecter les doublons reste à choisir.
- **RM-02 — Champs obligatoires :** un dossier ne peut être créé ou enregistré comme complet si les champs obligatoires définis dans le dictionnaire de données sont absents.
- **RM-03 — Accès au dossier personnel :** un Agent du ministère ne peut consulter que son propre dossier et les champs explicitement prévus pour son accès.
- **RM-04 — Modification contrôlée :** seuls les utilisateurs RH disposant de la permission correspondante peuvent créer ou modifier les données administratives d’un dossier.
- **RM-05 — Affectation :** une affectation à un service ou à un poste ne peut référencer qu’un service et un poste existants et actifs.

### Services et postes

- **RM-06 — Code unique :** chaque service et chaque poste possède un identifiant ou code unique dans son référentiel respectif.
- **RM-07 — Désactivation :** un service ou un poste déjà utilisé n’est pas supprimé physiquement ; il peut être désactivé afin de préserver les références et l’historique. Cette proposition devra être confirmée lors de la conception détaillée.
- **RM-08 — Portée du responsable de service :** un Responsable de service ne consulte que les informations autorisées des agents rattachés à son service.

### Congés et absences

- **RM-09 — Demande associée à un employé :** toute demande de congé ou déclaration d’absence est rattachée à un employé identifié.
- **RM-10 — Cycle de traitement :** une demande suit des états définis. Le scénario proposé est : soumise, en examen, acceptée ou refusée ; une annulation peut être prévue selon les règles à définir.
- **RM-11 — Décision traçable :** toute décision ou transition d’état est associée à son auteur et à une date et heure, et apparaît dans l’historique prévu à cet effet.
- **RM-12 — Demande non modifiable après décision :** une demande ayant reçu une décision ne peut être modifiée directement ; toute correction suit une opération distincte et traçable. Cette règle est une hypothèse à confirmer.
- **RM-13 — Vérification des dates :** une période demandée doit comporter une date de début antérieure ou égale à la date de fin. Les règles de chevauchement, de durée, de solde et de justificatif restent à définir.
- **RM-14 — Autorité de décision :** seuls les rôles autorisés par le circuit de traitement peuvent enregistrer une décision. Le circuit entre Responsable de service et équipe RH reste à préciser.

### Comptes et permissions

- **RM-15 — Compte nominatif :** chaque compte est associé à un seul utilisateur identifié ; les comptes partagés ne sont pas prévus dans le scénario.
- **RM-16 — Accès selon le rôle :** toute action est permise uniquement si le compte est actif et détient la permission correspondant à l’action et aux données visées.
- **RM-17 — Administration limitée :** l’Administrateur gère les comptes et permissions ; ses droits sur les dossiers RH ne sont pas automatiquement étendus par son rôle technique.
- **RM-18 — Désactivation d’un compte :** un compte désactivé ne peut plus ouvrir de session, mais ses opérations historiques demeurent attribuées à cet utilisateur.

### Rapports et historique

- **RM-19 — Rapports soumis aux permissions :** un rapport ne présente que les informations que l’utilisateur est autorisé à consulter. Les indicateurs de direction devraient privilégier les données agrégées lorsque l’identification individuelle n’est pas nécessaire.
- **RM-20 — Historique protégé :** un utilisateur ordinaire ne peut ni modifier ni supprimer les entrées d’historique ; seuls les rôles explicitement autorisés peuvent les consulter.
- **RM-21 — Enregistrement des opérations :** les opérations déclarées importantes sont journalisées avec l’acteur, la date et l’heure, l’action et l’objet concerné. La liste finale et la durée de conservation sont à déterminer.

## 3. Registre des décisions métier ouvertes

Ces décisions ne peuvent pas être déduites du contexte d’exemple. Elles doivent être confirmées par les responsables métier compétents avant de figer les exigences concernées. L’état « à confirmer » ne signifie pas que la décision est approuvée.

| ID | Décision à prendre | Effet si elle reste ouverte | Validation requise avant |
| --- | --- | --- | --- |
| DM-01 | Types de congés et d’absences pris en charge, et démarches ouvertes aux agents | Modèle de demande et exigences EF-10/EF-13 incomplets | Validation des parcours fonctionnels |
| DM-02 | Droits, plafonds, mode de calcul, jours ouvrés et justificatifs selon chaque type | Règles de contrôle et calcul des périodes impossibles à spécifier | Conception détaillée et tests métier |
| DM-03 | Délais de dépôt et possibilité de demande rétroactive | Contrôles de recevabilité indéfinis | Conception détaillée |
| DM-04 | Circuit d’examen : acteurs, ordre, délégation, quorum éventuel et décision finale | Permissions et transitions d’état incomplètes | Approbation de la matrice des rôles et permissions |
| DM-05 | États autorisés, transitions, annulation, correction et réouverture après décision | Cycle de vie des demandes et historique incomplets | Modèle fonctionnel et conception des données |
| DM-06 | Traitement des chevauchements, des demandes concurrentes et des périodes non ouvrées | Validation des dates et conflits de demandes indéfinis | Conception détaillée et tests métier |
| DM-07 | Champs du dossier employé, champs obligatoires, identifiant métier et critères de doublon | EF-01, EF-06 et RM-01/02 ne peuvent être finalisées | Validation du dictionnaire de données |
| DM-08 | Catégories de données visibles et modifiables par rôle et par portée | EF-04, EF-09, EF-17 et rapports ne peuvent être configurés sûrement | Approbation de la matrice d’accès |
| DM-09 | Liste des opérations journalisées, informations enregistrées et personnes autorisées à consulter les journaux | EF-22 à EF-24 et RM-20/21 restent partiellement spécifiées | Conception sécurité et données |
| DM-10 | Durées de conservation, archivage, suppression et éventuelle anonymisation des dossiers et journaux | ENF-12 et les procédures de cycle de vie des données restent incomplètes | Validation des exigences de protection des données |

Les validations doivent être consignées avec leur date, leur auteur ou instance approbatrice et la version des documents concernés. Tant qu’une décision est ouverte, les règles correspondantes restent des hypothèses de conception et ne doivent pas être présentées comme une politique officielle du MERN ou d’une autre organisation.
