# Choix du modèle de cycle de vie en V

## Décision et condition de validité

Le modèle en V est retenu **à titre provisoire pour organiser la documentation et la future vérification** du SIRH. Il convient au besoin de relier exigences, conception et activités de validation, mais il ne présume pas que les besoins sont déjà stables ou approuvés. Le projet reste un cas d’étude et plusieurs décisions métier sont ouvertes ; le cycle de vie devra donc être confirmé au jalon de validation des besoins.

Si les parties prenantes ne peuvent pas préciser les processus ou les règles avant la conception détaillée, le projet devra prévoir des boucles de prototypage et de validation incrémentale, ou réexaminer le choix du modèle. Le modèle en V décrit la structure de vérification ; il n’interdit pas les retours entre étapes lorsqu’une hypothèse est infirmée.

## Principe du modèle en V

Le modèle en V organise le projet en deux branches liées :

- **Branche de conception** : faisabilité et spécification des besoins, conception générale, conception détaillée et réalisation.
- **Branche de vérification et de validation** : tests unitaires, tests d’intégration, tests système et recette métier.

À chaque étape de conception correspond une activité de test préparée en regard. Les tests ne sont donc pas reportés à la fin : leurs objectifs et leurs critères d’acceptation sont définis à partir des exigences auxquelles ils doivent répondre.


## Pourquoi ce modèle convient au projet GRH

Un logiciel RH traite des informations structurées et des processus métier qui doivent être cohérents : dossiers des employés, rôles et droits d’accès, absences, congés ou autres fonctions qui seront confirmées dans le périmètre fonctionnel. Une erreur dans une règle ou dans l’accès à une donnée peut avoir des conséquences opérationnelles. Il est donc utile de formaliser les exigences et de pouvoir vérifier chaque fonction à partir de celles-ci.


## Pourquoi ne pas retenir les autres modèles

Les modèles ci-dessous ne sont pas intrinsèquement mauvais ; ils répondent à d’autres contextes. Le choix dépend ici de la possibilité de stabiliser les exigences principales et du besoin de produire une conception ainsi qu’une validation traçables.

### Modèle en cascade

La cascade suit des phases successives, mais rend moins visible le lien entre chaque décision de conception et son niveau de test. Le modèle en V conserve une progression structurée tout en planifiant les vérifications en miroir des phases de spécification et de conception. Il rend ainsi la stratégie de validation plus concrète.


### Modèle en spirale

La spirale organise le développement autour de cycles répétés d’analyse et de réduction des risques. Elle est intéressante pour un projet vaste, incertain, innovant ou techniquement risqué, mais demande davantage d’efforts de pilotage et d’analyse des risques à chaque cycle. Pour le périmètre actuellement décrit, cette complexité supplémentaire n’est pas justifiée.

### Approche incrémentale et prototypage

Ces approches permettent de livrer une partie du système ou une maquette afin d’affiner les besoins. Elles sont particulièrement pertinentes lorsque les processus ou attentes restent difficiles à préciser, ce qui est encore possible dans ce projet. Elles ne sont pas retenues comme cadre principal à ce stade, mais le plan doit permettre des prototypes ou validations incrémentales pour lever les incertitudes avant de figer une spécification. Si ces incertitudes demeurent nombreuses, le choix du modèle en V devra être réexaminé.

## Conclusion

Le modèle en V fournit un cadre lisible pour relier les besoins, la conception et leur vérification. Pour ce projet, il reste un choix de travail et non une conclusion fondée sur des besoins déjà stabilisés. La validation des acteurs, du périmètre et des règles métier constitue un jalon préalable ; le résultat de ce jalon déterminera si le modèle en V est conservé seul ou complété par une démarche de prototypage et d’itération.
