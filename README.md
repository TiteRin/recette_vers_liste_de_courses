# Recette vers liste de courses

## Braindump
Objectif : automatiser la liste de courses à partir d’une recette, mais en tant qu’objet physique

L’idée serait de générer des cartes à imprimer, soit à partir d’une recette en ligne, soit à partir d’une saisie manuelle. 
Les cartes contiendraient alors deux QR codes : 
- un QR code pour afficher la recette sur le téléphone au moment de la préparation (redirection vers la page ou affichage d’un contenu texte)
- un QR code permettant d’ajouter à une note (Google Keep ?) les ingrédients sélectionnés pour la recette

Le plus intéressant (challengeant) est le deuxième QR Code. Je ne sais pas encore comment ni si c’est possible, mais il faudrait pouvoir afficher la liste des ingrédients contenus dans la recette, e.g.
- [ ] Épinards (frais ou surgelés)
- [ ] Pois chiche (une grosse boîte)
- [ ] Pâte ou épices à curry
- [ ] Riz
- [ ] Amandes effilées

Et pouvoir sélectionner ceux qu’on garde pour ajouter à la liste. Si par exemple j’ai encore quarante douze boîtes de pois chiches dans mes placards ainsi qu’un sac de riz, je peux ne garder que :
- [ ] Épinards (frais ou surgelés)
- [ ] Pâte ou épices à curry
- [ ] Amandes effilées

Et ce serait automatiquement (comment ?) ajouté à la liste de courses. 
Dans un premier temps, ça pourrait peut-être être un contenu à coller dans une note, mais on verra

Le but ultime serait alors d’imprimer puis de plastifier les fiches ainsi obtenues pour les sortir au moment de choisir les repas de la semaine. Avec une photo et un joli template, ce serait encore mieux, mais c’est pas obligatoire. 

Comme je ne souhaite pas faire appel à l’IA, la saisie sera manuelle (mais si quelqu’un veut fork et rajouter de l’IA, qui suis-je pour vous en empêcher, c’est open), et sûrement que ce sera un simple script sans aucune persistence de données pour commencer. 
De toute façon, si ce n’est pour les statistiques, je ne vois pas l’intérêt de persister les données autrement que générer un fichier pdf ou image. Comme ça, le QR code peut fonctionner sans accès à Internet.

Bon, par contre, comment faire un QR code qui ajouter dans notre téléphone… Ça… je vais regarder. 
Je sais qu’il est possible de faire quelque chose dans Home Assistant, donc peut-être que l’application permettra de choisir la cible du QR Code, on verra bien. 

Voilà voilà.

J’espère que ce README ne restera pas dans cet état trop longtemps, sinon ça veut dire que l’idée sera restée à l’état de bloubiboulga. 
