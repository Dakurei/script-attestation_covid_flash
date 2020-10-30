Attestation Covid Flash v1.1
============================

Petit script en javascript pour réaliser un QR Code d'attestation de déplacement Covid à l'aide de paramètres passés dans la requête et automatiquement datée à une création faite il y a 30 minutes et datée à une sortie il y a 15 minutes.

> Version basée sur le QR Code généré depuis le formulaire: [Attestation de déplacement dérogatoire](https://media.interieur.gouv.fr/deplacement-covid-19/)

> Dépôt disponible ici: [attestation-deplacement-derogatoire-q4-2020](https://github.com/LAB-MI/attestation-deplacement-derogatoire-q4-2020)

Enregistrez l'url dans vos favoris avec les paramètres renseignés pour pouvoir automatiquement vous procurer une version numérique de l'attestation à présenter !

**/!\\ ATTENTION /!\\**
**Les paramètres doivent être encodés pour passer dans une url !**

## Paramètres:
| Nom       | Valeur                | Exemple                                                      |
|-----------|-----------------------|--------------------------------------------------------------|
| lastname  | Nom de famille        | Dupont                                                       |
| firstname | Prénom                | Jean                                                         |
| birthday  | Date de naissance     | 01%2F01%2F1956 (équivaut à **01/01/1956**)                   |
| birthtown | Ville de naissance    | Paris                                                        |
| address   | Adresse actuelle      | 1%20rue%20de%20la%20Paix (équivaut à **1 rue de la Paix**)   |
| zipcode   | Code postal           | 75001                                                        |
| town      | Ville                 | Paris                                                        |
| reason    | Raison du déplacement | 1 (chiffre entre 1 et 9 correspondant aux motifs ci-dessous) |

**Le motif de déplacement est par défaut celui du déplacement professionnel si non précisé !**

### Liste des motifs

| Code | Motif |
|------|-------|
| 1    | Déplacements entre le domicile et le lieu d'exercice de l'activité professionnelle ou les déplacements professionnels ne pouvant être différés (*A utiliser par les travailleurs non salariés, lorsqu'ils ne peuvent disposer d'un justificatif de déplacement établi par leur employeur*) |
| 2    | Déplacements pour effectuer des achats de fournitures nécessaires à l'activité professionnelle, des achats de première nécessité dans des établissements dont les activités demeurent autorisées (liste sur gouvernement.fr) et les livraisons à domicile (*Y compris les acquisitions à titre gratuit (distribution de denrées alimentaires...) et les déplacements liés à la perception de prestations sociales et au retrait d'espèces*) |
| 3    | Consultations et soins ne pouvant être assurés à distance et ne pouvant être différés et l’achat de médicaments |
| 4    | Déplacements pour motif familial impérieux, pour l'assistance aux personnes vulnérables et précaires ou la garde d'enfants |
| 5    | Déplacements des personnes en situation de handicap et de leur accompagnant |
| 6    | Déplacements brefs, dans la limite d'une heure quotidienne et dans un rayon maximal d'un kilomètre autour du domicile, liés soit à l'activité physique individuelle des personnes, à l'exclusion de toute pratique sportive collective et de toute proximité avec d'autres personnes, soit à la promenade avec les seules personnes regroupées dans un même domicile, soit aux besoins des animaux de compagnie |
| 7    | Convocation judiciaire ou administrative et rendez-vous dans un service public |
| 8    | Participation à des missions d'intérêt général sur demande de l'autorité administrative |
| 9    | Déplacement pour chercher les enfants à l’école et à l’occasion de leurs activités périscolaires |

## Exemple
Exemple d'une url préformattée pour générer des attestations automatiquement:
> https://dakurei.github.io/script-attestation_covid_flash/?lastname=Dupont&firstname=Jean&birthday=01%2F01%2F1956&birthtown=Paris&address=1%20rue%20de%20la%20Paix&zipcode=75001&town=Paris&reason=1

## Autre
Pour accéder à l'outil avec les données par défaut: [Cliquez ici](https://dakurei.github.io/script-attestation_covid_flash/)

---
*Dernière mise à jour du format du QR Code le: 29 Octobre 2020*
