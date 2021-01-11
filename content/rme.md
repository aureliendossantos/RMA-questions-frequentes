---
title: "Portail de RME: RPG Maker Extender"
description: "RME étend les possibilités des évènements de RPG Maker VX Ace avec des outils pratiques et des centaines de nouvelles commandes."
portail: rme
aliases:
    - /scripts/rme/
    - /rpgmaker/scripts/rme/
---

![Bannière du portail RME](/rme/banniere.png)

RME propose une collection d'outils pour favoriser la personnalisation d'un projet [RPG Maker VX Ace]({{< ref "/rpgmaker/historique.md#rpg-maker-vx-ace" >}}). Le projet est désormais archivé, ce qui signifie que son développement ainsi que son support sont arrêtés. Cependant, le script reste disponible au téléchargement et peut être librement modifié.

L'idée reposant derrière RME est d'utiliser la commande d'appel de script pour étendre les fonctionnalités offertes par les évènements. Le fait de passer par l'appel de script permet plus de flexibilité dans les commandes, par exemple le fait de pouvoir passer des variables à la place de tous les arguments.

## Téléchargement

[Dernière version du script.](https://raw.githubusercontent.com/RMEx/RME/master/RME.rb)

Copiez le script de préférence en dernier, juste avant `Main`. Voir aussi : [installer un script]({{< ref "/rpgmaker/scripts.md#rpg-maker-vx-ace-et-antérieur" >}}).

## Manuel d'utilisation

Le manuel peut être accédé depuis le sommaire du portail, à utiliser avec la [liste des commandes](http://rmex.github.io/RMEDoc) du site de RME.

Pour aller plus loin, des exemples d'utilisation sont présentés dans la section "Tutoriels" du [wiki officiel](https://github.com/RMEx/RME/wiki).

## Fonctionnalités

RME ajoute plus de 700 commandes en tout genre à utiliser dans les évènements, par le biais d'appels de script. Les commandes sont listées dans la [liste des commandes](http://rmex.github.io/RMEDoc/) et sont catégorisées ainsi :

- **Carte** : passabilité, terrains, régions, etc.
- **Standard** : messages, teintes, opérations, etc.
- **Evènements** : mouvement, apparence, invocation, etc.
- **Clavier** : détection des touches du RGSS et du clavier réel.
- **Souris** : détection de la position, des clics et des sélections.
- **Images** : effets, collisions, images de curseur, images fixées à la map.
- **Spritesheets** : images sectionnées en plusieurs cellules, de la même façon que les personnages.
- **Panoramas** : panoramas multiples, vitesse, profondeur et effet.
- **Equipe** : argent, nombre de pas, de combats, de sauvegardes, etc.
- **Armes, Armures et Objets** : lecture des notes et des paramètres, dernier objet utilisé, etc.
- **Système** : lire le titre du jeu, la version, la monnaie et la position de départ.
- **Acteurs** : apparence, équipement, caractéristiques, compétences.
- **Techniques** : lecture des notes et paramètres.
- **Mathématiques** : trigonométrie et géométrie.
- **Groupes d'ennemis** : lecture du nom du groupe, des membres et de leur position.
- **Ennemis** : lecture du nom, des notes et des caractéristiques.
- **En combat** : lecture des caractéristiques actuelles des ennemis en combat.
- **Textes** : affichage de textes personnalisables à l'écran.
- **Date et Heure** : renvoie l'heure de l'ordinateur, de la seconde à l'année.
- **Client-Serveur** : connexion à un serveur, envoi et réception de messages.
- **Scènes** : appels de scènes (écran-titre, menus, etc) et gestion de la pile.
- **Sauvegardes** : gestion des fichiers de sauvegarde, lecture des variables d'une autre sauvegarde, etc.
- **Zones virtuelles** : zones rectangulaires, circulaires, etc. sur la carte utilisées dans la programmation de systèmes.
- **Champs de texte** : permet au joueur d'entrer du texte ou des nombres au clavier.
- **Presse-papier** : place du texte ou une commande d'évènement dans le presse-papier, ou lit son contenu.
- **Vibrations** : vibrations du moteur gauche et droit de la manette Xbox.
- **Sons** : volume, vitesse et fondu des BGM, BGS, ME et SE.
- **Caméra** : déplacements, verrouillage de l'axe X ou Y, ciblage d'un évènement, zoom et flou.
- **Ecran** : transitions, teintes, pixellisation, flou.
- **Fenêtres** : affichage de fenêtres de texte et de menus personnalisés.
- **Effets spéciaux** : réflexion, activer/désactiver l'obscurité lors d'un changement climatique.

### Interrupteurs, variables et labels

- Ajout des raccourcis `S[id]` et `V[id]` pour manipuler les interrupteurs et variables dans les appels de script.
- Ajout des labels `L[key]`, des labels locaux `SL[key]`, des variables locales `SV[id]` et extension des interrupteurs locaux `SS[id]`.
- Appel des interrupteurs/variables/labels locaux depuis un autre évènement ou une autre carte : `SV[id_map, id_event, id]`.

### Outils de test

Ces outils sont disponibles uniquement lorsque le jeu est lancé depuis l'éditeur.

- Testez les commandes RME ou d'autres appels de script en jeu avec le testeur de commandes (F3).
- Testez des tons d'écran directement sur la carte avec le testeur de teinte (F4).
