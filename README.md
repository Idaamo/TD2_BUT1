# TD2_BUT1

## Présentation du projet CommandAPI

Le projet a été créée pour but de faciliter la tâche des développeurs Java travaillant sur la librairie Spigot ou Paper. Ils permettent d'exécuter un serveur Minecraft avec la possibilité d'utiliser des plug-ins.

L'API a été rendue compatible pour les plug-ins dont la langue de programmation est le Java.
Sur Minecraft ou Spigot/Paper, des commandes natives sont disponibles, par exemple: plugins, permettant d'afficher la liste des plug-ins détectés.
Chaque commande a ou non une permission, plugins a comme permission "bukkit.command.plugins". En utilisant l'API pour cette commande, on pourra utiliser remapCommandByName("plugins", executor, main); afin de remapper la commande pour utiliser une nouvelle logique d'exécution (Spigot ou paper ne proposent pas de méthode directe permettant de le faire).

L'API était utilisable en ajoutant la dépendance à Maven ou Gradle, ou en téléchargeant la dépendance. (les liens ne fonctionnent plus)
