# TP Git / GitHub – Mon assistant de révision

## 1. Présentation du projet

Ce TP consiste à créer un petit programme Python et à apprendre à suivre ses modifications avec Git et GitHub.

Le programme `main.py` est un assistant de révision simple. Il demande le prénom de l'utilisateur, la matière qu'il révise et la durée prévue de révision, puis affiche un objectif.

## 2. Évolution du programme

Le fichier `main.py` a évolué en quatre versions successives :

- **V1 – Création du programme :** affichage du titre et d'un message de bienvenue.
- **V2 – Ajout du prénom :** le programme demande le prénom et affiche un message personnalisé.
- **V3 – Ajout de la matière :** le programme demande la matière révisée et l'affiche.
- **V4 – Ajout de la durée :** le programme demande le nombre de minutes et affiche l'objectif de révision.

Chaque version correspond à une modification du même fichier `main.py`, enregistrée dans l'historique Git avec un commit.

## 3. Outils nécessaires

- Python installé sur l'ordinateur.
- Visual Studio Code (VS Code).
- Git installé et configuré.
- Un compte GitHub.

## 4. Exécution du programme avec VS Code

1. Ouvrir Visual Studio Code.
2. Choisir **File > Open Folder** et ouvrir le dossier du projet.
3. Ouvrir le fichier `main.py`.
4. Si nécessaire, choisir l'interpréteur Python.
5. Cliquer sur **Run Python File** (le bouton ▶).
6. Saisir le prénom, la matière et la durée demandés dans le terminal.
7. Enregistrer les modifications avec **Ctrl + S**.

## 5. Commandes Git utilisées

- `git init` : initialise un dépôt Git dans le dossier du projet.
- `git add main.py` : prépare les modifications de `main.py` pour le prochain commit.
- `git commit -m "message"` : enregistre un état du projet dans l'historique local avec un message.
- `git push` : envoie les commits locaux vers le dépôt distant GitHub.
- `git pull` : récupère les changements du dépôt distant et les intègre dans la branche locale.

Le nom `origin` est le nom donné au dépôt distant GitHub.

## 6. Questions du TP1

**1. Où la version V3 a-t-elle été créée et quelle commande permet de la récupérer sur le PC ?**  
La V3 a été créée directement sur GitHub. La commande `git pull origin main` permet de récupérer cette version sur le PC.

**2. Pourquoi utiliser `git add` avant `git commit` ?**  
Parce que `git add` place les modifications dans la zone de préparation (staging). Ensuite, `git commit` enregistre les modifications préparées dans l'historique.

**3. Que signifie `origin` ?**  
C'est le nom habituellement utilisé pour désigner le dépôt distant, ici le dépôt GitHub.

**4. Que se passe-t-il si le dépôt local et le dépôt GitHub sont déjà identiques et qu'on exécute `git pull` ?**  
Git ne télécharge aucun nouveau changement et indique que la branche est déjà à jour (`Already up to date`).

## 7. Différence entre git push et git pull

`git push` envoie les commits du PC vers GitHub.  
`git pull` récupère les changements de GitHub vers le PC.
