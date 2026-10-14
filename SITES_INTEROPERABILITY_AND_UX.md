# Sites KLE / SA / Enquêtes du Vivant — interopérabilité et UX appliquée

État : synthèse publique vérifiée le 14 octobre 2026. Périmètre : lecture des branches principales et des reçus de projet ; aucun nouvel essai en production effectué pour cette synthèse.

## Ce que ce terrain démontre

Lucas Benavenuto conçoit et fait évoluer un ensemble de services reliant recherche-action, participation et ressources pédagogiques. Le travail associe clarification des besoins, architecture de l’information, parcours utilisateurs, prototypage avec assistance IA et vérification des changements. Les trois sites ont des fonctions distinctes et conservent l’autorité sur leurs propres contenus.

| Surface | Fonction | Exemples examinés |
| --- | --- | --- |
| [La KLE](https://lakle.fr) | Cadre méthodologique et accès aux projets, publications et ressources | Lecture de ressources SA, flux éditoriaux, retours d’usage et espace équipe |
| [Souveraineté en Action](https://sa.lakle.fr) | Participation, rencontres et transmission de pratiques collectives | Relations entre événements et ressources, bibliothèque et flux de ressources |
| [Enquêtes du Vivant](https://enquetesduvivant.lakle.fr) | Enquêtes pédagogiques et restitution adaptée aux publics | Fiches segmentées, retours facultatifs, téléchargement et administration des réponses |

## Interopérabilité : découvrir un objet en préservant sa source

Le cas concret est celui d’une ressource SA découverte depuis KLE : le site lecteur sélectionne une représentation publique et renvoie à la page d’origine. L’objet conserve son identité, son éditeur et son adresse de référence.

La lecture KLE vérifie la version du flux, la source, les adresses attendues, les identifiants et les dates. Elle écarte les doublons et les entrées non conformes ; une date mal formée ne doit pas faire disparaître les ressources valides voisines. Des tests ciblés couvrent ces cas dans la branche principale.

Les événements disposent d’une architecture de fédération légère : JSON pour l’affichage croisé, RSS pour l’abonnement et iCalendar pour l’agenda. La documentation distingue l’organisateur d’un rendez-vous du site qui le relaie. Le modèle est réutilisable par d’autres surfaces ; sa généralisation à des partenaires supplémentaires reste à éprouver.

Sur SA, les relations événement–ressource sont projetées depuis le registre existant. Une rencontre peut ainsi conduire vers une restitution ou une fiche pratique, et une ressource retrouver son contexte. Ces relations constituent un travail d’architecture de l’information, sans créer un second catalogue concurrent.

## UX : rendre le fonctionnement compréhensible et les retours exploitables

Le travail UX porte sur les fonctions réellement proposées aux visiteurs : comprendre une ressource, rejoindre une rencontre, reprendre un outil et faire un retour. Les tests éditoriaux KLE vérifient notamment un langage orienté vers les besoins et la présence des liens utiles.

Les retours KLE sont attachés à un contenu identifié. Le composant présente une interaction compacte puis un formulaire détaillé à la demande. Enquêtes du Vivant propose un retour facultatif sur la clarté, l’utilité et la difficulté ressentie, avec texte libre et email optionnel. Le formulaire distingue l’échec d’envoi de la confirmation reçue du serveur.

Les fiches EDV disposent d’adaptations déterministes selon le contexte : personne, collectif, facilitation, institution ou organisation. Ce mécanisme adapte des contenus éditoriaux préparés ; il ne démontre pas une personnalisation générative par IA.

Ces réalisations montrent une conception de parcours et une instrumentation des retours. Une amélioration mesurée de la compréhension, de la satisfaction ou du transfert autonome demanderait des observations utilisateurs comparatives.

## Fonctions réalisées et limites de validation

| Fonction | Preuve examinée | Portée de la conclusion |
| --- | --- | --- |
| Sélection de ressources SA dans KLE | Lecteur et tests de fédération présents sur main | Implémentation vérifiée par lecture ; tests non réexécutés pendant cette passe |
| Relations événements–ressources SA | Fonctions de projection et tests dédiés sur main | Relations explicites dans le code |
| Retour d’expérience EDV | Composant et route API dédiés sur main | Fonction implémentée ; réception actuelle en production non retestée |
| Fiches adaptées EDV | Contenus segmentés et sélection déterministe sur main | Adaptation éditoriale implémentée |
| Administration EDV | README et routes de soumission, export et ressources | Capacités présentes ; disponibilité dépendante de la configuration de déploiement |
| Abonnements, partage et mailing KLE | Reçu de projet du 5 octobre : confirmation, retrait, compilation et contrôles navigateur rapportés | Vérification historique documentée ; aucune nouvelle délivrabilité revendiquée |
| Fédération de ressources SA vers EDV | Composant documenté sur main, note encore CANDIDATE avec gates de publication | Ne pas présenter la disponibilité de bout en bout comme acquise |

## IA : conception assistée et pilote d’exécution borné

Le développement des sites mobilise des outils IA sous conduite humaine : cadrage, changements proposés, revue, tests et décision de publication. Ce travail de conception assistée est distinct d’un service agentique autonome disponible pour les visiteurs.

Un reçu de projet du 29 septembre décrit également un passage d’un modèle local depuis le cockpit de préparation AG : production d’un résultat candidat privé, avec relecture humaine et sans modification automatique des documents. C’est une trace historique d’intégration bornée. Elle ne valide pas un runtime Nexus complet, une disponibilité permanente ou une qualité généralisable.

Les sites constituent un terrain d’application des principes Nexus : autorité des sources, dérivés, validation, mémoire et continuité. Nexus ne doit pas être présenté comme le backend universel des trois applications.

## Solidité des preuves

Il existe des preuves concrètes de conception et d’implémentation : code intégré, tests ciblés et reçus de publication. Leur portée reste attachée au cas examiné.

La QA SA présente deux exécutions réussies le 8 octobre sur la révision `da61eec4b287ace495e7707e7ec152192f48fb4c`. Une exécution ultérieure, sur `5a41b731ab8f2dc3c7aac8634cadee6c282e12ec`, est signalée en échec ; sa cause n’a pas été diagnostiquée ici. Cette synthèse ne revendique donc pas une CI actuelle entièrement verte.

L’architecture détaillée de Living Provenance Graph et de projection d’activité reste une conception WORKING dans la note examinée. Les fonctions existantes ne suffisent pas à déclarer ce graphe entièrement implémenté.

## Registre de vérification

Sources techniques privées consultées ; seuls leurs rôles et repères de version sont exposés. Leur code, les données des participants et les contrats internes restent contrôlés.

| Corpus examiné | Révision main observée | Pièces déterminantes |
| --- | --- | --- |
| KLE | `8ea95971d6340ba1ec253c501f31c43f06e1766d` | Lecteur de ressources SA ; tests de fédération ; composant de retour ; carte des flux ; état courant et reçus historiques |
| SA | `64074c00f3838088a0000f6a6a99b4ea59f84e8c` | Projections événement–ressource ; note de régression des flux ; historique QA |
| EDV | `e745c2fba4d5197cde265a5f2a3d1d2e1e73c05d` | Fiches adaptées ; composant de retour ; routes API ; README ; note de fédération candidate |

Pour une revue technique accompagnée, ces repères permettent de retrouver les pièces exactes. Cette publication constitue une synthèse de preuves, sans ouvrir les dépôts privés.

## Ce que cela apporte à un projet partenaire

Ce terrain illustre une capacité à traduire des besoins collectifs en interfaces et en flux de données cohérents, à préserver les responsabilités éditoriales et à intégrer des retours dans l’évolution du service. La contribution associe pilotage, conception UX, architecture de l’information et réalisation assistée par IA. Les effets sociaux et pédagogiques restent des objets d’évaluation.
