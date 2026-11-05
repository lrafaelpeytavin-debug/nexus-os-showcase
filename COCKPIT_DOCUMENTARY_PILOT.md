# Un assistant documentaire dans le travail d'un conseil d'administration

## Ce qu'une personne peut faire

Dans le cockpit interne de La KLE, un membre peut poser une question sur les documents accessibles dans son espace et obtenir une réponse candidate accompagnée des passages utilisés. L'objectif est concret : préparer une discussion, clarifier une proposition et revenir au texte qui l'appuie.

Le 5 novembre 2026, le porteur du projet a demandé trois priorités à discuter à partir d'un document de préparation du conseil d'administration. Une réponse en trois points est apparue dans sa session authentifiée. Il a ensuite ouvert les trois passages cités pour les comparer aux propositions. Le texte partagé du document est resté distinct de cette réponse personnelle.

Ce parcours marque une évolution du pilote : l'assistance générale déjà observée est complétée par un premier échange documentaire effectivement reçu dans l'interface. Il fournit un cas de travail pour les prochaines améliorations.

## Comment le travail circule

```text
une question dans un espace authentifié
→ documents accessibles à cette personne
→ sélection de passages et contexte de travail
→ génération avec un modèle local
→ contrôles de la réponse et des références
→ réponse candidate, passages cités et historique
→ lecture, correction et prochain geste humain
```

Le modèle rédige à partir du contexte transmis. L'application porte l'identité du lecteur, la sélection documentaire, les références et la conservation de l'échange. La personne garde la main sur ce qu'elle reprend pour une réunion ou un document collectif.

L'inférence de ce cas est reliée à un fournisseur Ollama local dans les reçus techniques privés. Le cockpit web et la mémoire documentaire externe ont leurs propres dépendances : la disponibilité hors connexion de l'ensemble reste à éprouver.

## Où en sont les capacités

| Capacité | État au 5 novembre 2026 |
|---|---|
| Question générale et réponse visible | Usage confirmé par le porteur |
| Question sur un document de son espace | Premier parcours utile confirmé, avec trois passages affichés |
| Vérification des références | Passages consultables ; contrôle complet des versions sources encore à approfondir |
| Retour après déconnexion ou interruption | Qualification en cours |
| Mémoire de projet étendue au Drive | Raccord en préparation, au-delà du corpus actuellement offert |
| Telegram et Discord | Travaux de raccordement conservés ; nouvelle preuve d'usage attendue |
| Délai de réponse et usage simultané | Mesures comparatives à établir |

La prochaine épreuve d'usage sera la reprise autonome par un autre membre : retrouver le fil, vérifier une source, corriger une proposition et poursuivre le travail. Elle permettra d'observer l'utilité et la charge de relecture au-delà de ce premier cas.

## Une trajectoire d'amélioration mesurable

Le travail porte d'abord sur les délais vécus dans l'interface, la reprise des échanges et une copie lisible avec ses références. Les modèles seront ensuite comparés sur les mêmes questions et documents, en conservant les droits d'accès et les critères de fidélité. Une réponse plus rapide n'est utile que si elle reste vérifiable et facile à reprendre.

Les changements sont documentés selon quatre états : préparé, intégré au code, installé, puis utilisé. Les hypothèses et les résultats négatifs restent dans la trajectoire de recherche.

## Pour quels usages explorer un pilote

- **Associations et collectifs :** préparer les réunions, comprendre les propositions et conserver les corrections et les suites.
- **Coopératives et réseaux :** reprendre une mémoire de projet entre plusieurs personnes tout en respectant les responsabilités et les espaces.
- **Partenaires techniques ou scientifiques :** comparer les choix de contexte, les reprises et l'effort de correction sur un cas délimité.

L'offre à éprouver est un pilote d'intégration et d'accompagnement avec un usage défini, un suivi et un bilan. Le temps économisé, la maintenance et le coût d'exploitation devront être mesurés dans ce cadre.

[Retour à la présentation](README.md) · [Preuves d'usage](PROOF_OF_USE.md) · [Modèle d'architecture](ARCHITECTURE_OVERVIEW.md)

