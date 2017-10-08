# Instructions
ce fichier décrit les instructions nécessaires aux étudiants de l'optionnel du DQPRM 2017 pour la réalisation des travaux dirigées.
## Travail par paire
Les étudiants doivent travailler en *binome* sur 2 ordinateurs différents pour mettre en pratique les concepts développés sur `GIT` durant la formation.
## Récupération du dépôt
Il faut récupérer le fichier de travail sur ce site [github](https://github.com/ludicludo/optionnelDQPRM).
Dans un terminal, créer un répertoire de travail et s'y déplacer. Lancer la commande `git clone https://github.com/ludicludo/optionnelDQPRM`
## Utilisation de GIT
### EXERCICE 1:
Le fichier `README.md` est un fichier au format `markdown` suivi par git.
Consulter l'historique des modifications de ce fichier.
- Quelles modifications ont été réalisées sur le commit `d8afc81` ?
- A quelle la date a été réalisée spécifiquement ce commit ?

### EXERCICE 2:
Le fichier `TAC.txt` contient les activités d'un patient pour différents organes d'intérêt. Les colonnes `L2L4` et `Rate` contiennent des données avec des virgules au lieu de points comme séparateur décimal. 

- Chaque étudiant récupère le fichier `TAC.txt` sur Github.
- Chaque étudiant fait une copie de `TAC.txt` et nomme le nouveau fichier `TAC_modifie.txt`.
- L'étudiant 1 modifie la colonne `Rate` et le second la colonne `L2L4` dans le nouveau fichier.
- Chaque étudiant utilise Git pour garder une trace de ces modifications.
- Chaque étudiant pousse le nouveau fichier et ses modifications sur Github.
### Exercice 3:
- Créer un fichier texte `rapport.md`.
- Ecrire le titre du rapport 'rapport DQPRM nom prénom.'
- Ajouter le fichier sur votre dépôt git et pousser le sur le serveur `git`.
- Gérer le conflit éventuel avec votre binôme et choisisser *un nom d'équipe*.

## LITTERATE PROGRAMMING
Chaque paire d'étudiants doit réaliser le calcul de l'activité cumulée pour chaque organe contenu dans le fichier `TAC_modifie.txt`.
#### Python/Pweave
Il est possible d'utiliser plusieurs outils pour faire du LP. Dans les exercices suivants, nous utiliserons le couple `Python/Pweave`. Pweave
### EXERCICE 1:
