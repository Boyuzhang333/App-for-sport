# App-for-sport
Présentation du logiciel
Ce logiciel permet aux utilisateurs, même en mode invité, de personnaliser leur expérience en entrant des informations telles que leur âge, taille et poids, puis en choisissant le type de plan qu’ils souhaitent suivre. Chaque type de plan inclut des informations supplémentaires à renseigner selon les objectifs personnels. Une fois les données saisies, le système fournit une répartition détaillée des macronutriments (glucides, protéines, lipides) adaptée à leurs besoins.

Dans une phase ultérieure, une API de calcul des calories des aliments pourra être intégrée, offrant ainsi une planification alimentaire encore plus précise et personnalisée. Pour les utilisateurs connectés, des fonctionnalités supplémentaires seront disponibles, telles que la possibilité de commenter, de définir des préférences personnelles, et de suivre leurs progrès dans le cadre de leur plan nutritionnel
Fonctionnalités et exigences de qualité

Interface principale :

EX1 : La première interface doit contenir une boîte de sélection de langue.

EX2 : La première interface doit permettre de sélectionner l'âge.

EX3 : La première interface doit permettre de sélectionner le poids.

EX4 : La première interface doit permettre de sélectionner le sexe.

EX5 : La première interface doit offrir un choix entre une visite en mode invité ou un accès après inscription.

EX6 : La première interface doit inclure un bouton "Terminer" pour confirmer les paramètres.

Navigation vers la deuxième interface :

EX7 : Après avoir appuyé sur le bouton "Terminer", la deuxième interface s'affiche.

EX8 : La deuxième interface doit proposer différentes options de planification alimentaire (multi-sélection possible).

EX9 : La deuxième interface doit inclure un bouton "Terminer" pour confirmer la sélection.

Navigation vers la troisième interface :

EX10 : Après avoir appuyé sur le bouton "Terminer" de la deuxième interface, on accède à la troisième interface.

EX11.1 : La troisième interface affiche la répartition des trois macronutriments (glucides, protéines, lipides) sur une semaine, en fonction des plans sélectionnés.

EX11.2 : Le système propose un accès détaillé aux plans en cliquant dessus.

Fonctionnalités liées au "Plan Orange" :

EX12.1 : Le système peut appeler une API de calcul du métabolisme de base pour estimer la dépense métabolique en fonction de l'âge, du sexe et du poids.

EX12.2 : La page de détails offre la possibilité de renseigner des informations facultatives : pratique d'exercices aérobiques ou anaérobiques.

EX12.3 : Les dépenses énergétiques moyennes liées aux exercices peuvent être ajoutées au métabolisme de base (optionnel).

EX13 : Le système génère un plan basé sur une répartition énergétique glucides-protéines-lipides selon un ratio de 5:3:2 (6 kcal/g, 4 kcal/g, 9 kcal/g).

EX14 : Le système recommande une perte de poids raisonnable de 3 à 5 % du poids initial sur un mois.

EX15 : Le système affiche un avertissement sur la page de détails du plan Orange : en cas de stagnation de poids pendant une semaine, réduire les glucides de 15 g.

Calculs personnalisés :

EX16 : Le système calcule la quantité totale hebdomadaire des trois macronutriments en fonction des quantités données par kg de poids corporel.

EX17 : Répartition hebdomadaire :

Les protéines sont réparties uniformément sur les 7 jours (1/7 par jour).

Journées riches en glucides (2 jours) : glucides = 25 % de la semaine ; lipides = 7,5 % de la semaine.

Journées pauvres en glucides (2 jours) : glucides = 7,5 % de la semaine ; lipides = 25 % de la semaine.

Journées modérées en glucides (3 jours) : glucides = 35 % de la semaine, répartis équitablement sur les 3 jours ; lipides = 35 % de la semaine, répartis équitablement.

EX18 : La page de détails affiche les 7 combinaisons possibles de distribution, toujours dans l'ordre suivant : jours modérés, jours faibles, jours riches en glucides.

Considérations techniques
Technologie frontale : Utilisation d'une interface utilisateur mobile adaptative.
Déploiement : Application envisagée comme une application web.
Stockage des données utilisateur : Dans un premier temps, pas de base de données ; stockage simple pour les tests initiaux.
