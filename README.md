Attestation Covid Flash v1.0
============================

Petit script en javascript pour réaliser un QR Code d'attestation de déplacement Covid à l'aide de paramètres passés dans la requête et automatiquement datée à une création faite il y a 30 minutes et datée à une sortie il y a 15 minutes.

> Version basée sur le QR Code généré depuis le formulaire: [Attestation Couvre Feu Covid-19](https://media.interieur.gouv.fr/attestation-couvre-feu-covid-19/)

**Le motif de déplacement est par défaut celui du déplacement professionnel !**

Enregistrez l'url dans vos favoris avec les paramètres renseignés pour pouvoir automatiquement vous procurer une version numérique de l'attestation à présenter !

**/!\\ ATTENTION /!\\**
**Les paramètres doivent être encodés pour passer dans une url !**


Paramètres:
| Nom       | Valeur             | Exemple                                                    |
|-----------|--------------------|------------------------------------------------------------|
| lastname  | Nom de famille     | Dupont                                                     |
| firstname | Prénom             | Jean                                                       |
| birthday  | Date de naissance  | 01%2F01%2F1956 (équivaut à **01/01/1956**)                 |
| birthtown | Ville de naissance | Paris                                                      |
| address   | Adresse actuelle   | 1%20rue%20de%20la%20Paix (équivaut à **1 rue de la Paix**) |
| zipcode   | Code postal        | 75001                                                      |
| town      | Ville              | Paris                                                      |

Exemple d'une url préformattée pour générer des attestations automatiquement:

> https://dakurei.github.io/script-attestation_covid_flash/?lastname=Dupont&firstname=Jean&birthday=01%2F01%2F1956&birthtown=Paris&address=1%20rue%20de%20la%20Paix&zipcode=75001&town=Paris

Pour accéder à l'outil: [Cliquez ici](https://dakurei.github.io/script-attestation_covid_flash/)

---
*Dernière mise à jour du format du QR Code le: 29 Octobre 2020*