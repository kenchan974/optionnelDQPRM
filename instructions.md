# Instructions
Ce fichier décrit les instructions nécessaires aux étudiants de l'optionnel du DQPRM 2017 pour la réalisation des travaux dirigées.
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

## Litterate Programming
Chaque paire d'étudiants doit réaliser le calcul de l'activité cumulée pour chaque organe contenu dans le fichier `TAC_modifie.txt`.
### Python/Pweave
Il est possible d'utiliser plusieurs outils pour faire du LP. Dans les exercices suivants, nous utiliserons le couple `Python/Pweave`. Par ailleurs, par simplicité pour les formateurs, les bibliothèques python `pandas` et `matplotlib` sont imposées.

Inspirer vous du fichier `demo_Pweave.pmd` pour créer votre document.
### EXERCICE 1:
Dans un première section du document, déterminer les versions des bibliothèques `pandas et `matplotlib` que vous allez utiliser. 
Ces informations sont donnés par les attributs `__version__` de chaque bibliothèque.

```python
pandas.__version__
matplotlib.__version__
```
	
### EXERCICE 2:
Compléter le script ci-dessous pour modifier le fichier TAC.txt. Ajouter le nouveau fichier sur votre dépôt `git`.
```python
with open('nom_du_fichier_tac.txt', 'r') as fichier:
    lines = fichier.readlines() # retourne une liste de string
	
with open('nom_de_votre_nouveau_fichier', 'w') as f_out:
	# votre code ici
	# parcourir la liste et remplacer les occurences ',' par '.'
	# utiliser par exemple la fonction replace() 
```		
### EXERCICE 3:
Ouvrir le fichier `TAC_modifie.txt` à l'aide de la méthode `read_csv` de la bibliothèque `pandas`.
### EXERCICE 4:
Créer un graphique (ou plusieurs) qui affiche(nt) les courbes d'activités en fonction du temps et insérer le graphique dans le document 'rapport.md'.
### EXERCICE 5:
Calculer l'aire sous la courbe pour chacun des organes d'intérêt et noter directement les valeurs dans le rapport (sous forme de tableau pour les plus aguerris).
