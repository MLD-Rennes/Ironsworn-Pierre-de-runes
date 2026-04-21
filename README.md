# Ironsworn-Pierre-de-runes

Script nanDECK pour créer un deck pour Ironsworn, un système d'Oracle sous forme de 
cartes à tirer.
Version originale créée par Sébastien Morand en 2024.
Script réalisé par Matze en 2026. 

Vous pouvez créer vos propres oracles et imprimer ces cartes pour un usage personnel.
Leur taille (88x63mm) permet de les utiliser avec des pochettes protectrices
pour cartes standards. L'impression doit être faite au format A4, en recto-verso
avec retournement sur le bord court.

## Utilisation des cartes

Voir le document *Ironsworn-VF-Deck-Pierres-Runes-Economie-RectoVerso-1-5.pdf*
pour une explication détaillée du fonctionnement du deck de cartes oracles.

## Création d'un deck

Pour créer un deck, vous devez installer le logiciel [nanDECK](https://nandeck.com/), 
**version 1.28.3**.
Les fichiers importants sont : 
- creator.nde : Script décrivant la logique de création des cartes
- runestones-data.csv : Fichier décrivant les données des oracles.
- runes-data.csv : Noms de runes à afficher au verso
- img/runes/*.jpg : Images de runes à afficher au verso.
    - Les noms des images doivent correspondre au nom des runes indiquées dans 
      le fichier runes-data.csv

### Enregistrement des données des oracles.

Pour personnaliser vos oracles, vous pouvez saisir vos propres données dans le 
fichier *runestones-data.csv*. 
Vous devez saisir, dans l'ordre, les différents champs correspondants au onze oracles : 
- Action (x4)
- Thème (x4)
- Lieu (x2)
- Description de Lieux (x2)
- Trouble de village (x2)
- Rôle de personnage (x2)
- Objectif de personnage (x2)
- Description de personnage (x4)
- Action de combat (x1)
- Contrecoup mystique (x1)
- Rebondissement (x1)

Certains champs possèdent plusieurs valeurs sur chaque carte. 
En conséquence, vous devez renseigner davantage de données pour ces champs
(cf. facteur indiqués à la suite des noms de champs).

La première ligne du fichier de données est complètement arbitraire et sert
simplement de rappel. Vous pouvez la modifier si vous le souhaitez.

Le fichier de données CSV est encodé au format *Latin1*.

### Enregistrement de runes (optionel)

Au verso des cartes, des noms et symboles de runes sont affichés pour 
vous donnez un peu d'inspiration. Vous pouvez créer vos propres symboles
et noms. 
Vous devez modifier le fichier *runes-data.csv* de la même manière 
que pour l'enregistrement des données d'oracle. Vous devez indiquez 
un nom et une signification pour la rune. 
**ATTENTION:** les noms de runes doivent être associés à une image, avec le même nom, dans
le dossier *img/runes/* pour que le nanDECK les reconnaisse.

### Créer le deck de cartes

Une fois les données enregistrées pour votre deck d'oracles, 
vous pouvez lancer *nanDECK* construire les cartes.
En haut à gauche, cliquer sur *Open Deck* puis sélectionnez le fichier *creator.nde*,
pour ouvrir le script servant à construire les cartes.
Le script s'affiche au centre si vous souhaitez le lire ou le modifier.
Si vous souhaitez utiliser d'autre fichiers de données, vous pouvez modifier 
les directives *LINK* .

Une fois ceci fait, ou si vous souhaitez garder les noms de fichier déjà 
défini, vous pouvez cliquer sur *Validate Deck* puis *Build Deck*, sur la gauche 
de la fenêtre, pour construire chaque carte.
Après un certain temps, les cartes vont se constuire. 
Vous pouvez les visualiser sur la gauche. Des flèches en-dessous des cartes 
permettent de changer la carte visible. Cliquer sur *Card Preview* 
pour observer les cartes plus en détails, zoomer, etc.

Une fois ceci fait, vous pouvez cliquer sur la gauche sur :
- *Print deck* pour imprimer les cartes directement en recto-verso.
- *Save images* pour enregistrer les cartes individuellement au format numérique
- *PDF* pour créer un pdf des images, à partager ou à imprimer

Vous pouvez maintenant jouer avec vos cartes ou en créer de nouvelles 
si le coeur vous en dit !

## Licence

Ces cates sont basés sur la traduction française d'[*Ironsworn*](ironsworn.pbta.fr) 
réalisée par Thomas Pereira et publiée par [500 Nuances de geek](500nuancesdegeek.fr) 
au sein de [La Caravelle](fr.tipeee.com/la-caravelle) en 2018. 
Le texte de la version française est publié sous licence [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.fr) 
