# TD2_BUT1

## Présentation du projet CommandAPI

Le projet a été créée pour but de faciliter la tâche des développeurs Java travaillant sur la librairie Spigot ou Paper. Ils permettent d'exécuter un serveur Minecraft avec la possibilité d'utiliser des plug-ins et d'autres fonctionnalités.

### Minecraft

Minecraft est un jeu vidéo de type aventure « bac à sable » développé par le Suédois Markus Persson, alias Notch, puis par la société Mojang Studios. (Wikipédia, 19/10/2026 à 13h05, [Lien direct](https://fr.wikipedia.org/wiki/Minecraft))

### API

L'API a été rendue compatible pour les plug-ins dont la langue de programmation est le Java.
Sur Minecraft ou Spigot, des commandes natives sont disponibles, par exemple: "plugins", permettant d'afficher la liste des plug-ins détectés.
Chaque commande a ou non une permission, "plugins" a comme permission "bukkit.command.plugins". En utilisant l'API pour cette commande, on pourra utiliser remapCommandByName("plugins", executor, main); afin de remapper la commande pour utiliser une nouvelle logique d'exécution (Spigot ne proposant pas de méthode directe permettant de le faire). On peut également modifier la logique avec remapCommandByName("bukkit.command.plugins", executor, main); afin de cibler les commandes utilisant cette permission.

L'API était utilisable en ajoutant la dépendance à Maven ou Gradle, ou en téléchargeant la dépendance. (les liens ne fonctionnent plus)
Une fork a été mise à disposition permettant de remapper plusieurs commandes en une seule ligne: [Lien direct](https://github.com/omega7711/CommandAPI)
