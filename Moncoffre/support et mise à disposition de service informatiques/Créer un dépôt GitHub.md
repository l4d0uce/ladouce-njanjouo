Procédure : créer un dépôt GitHub et le cloner en local

1. Installer Git

2. Télécharger Git depuis le site officiel
3. Installer Git en suivant les instructions.
4. Ouvrir un terminal et vérifier l’installation avec la commande :

git --version

2. Configurer son identité Git

3. Configurer son nom :

git config --global user.name "Mon Nom"

1. Configurer son adresse e-mail :

git config --global user.email "monmail@example.com"

1. Vérifier la configuration :

git config --global --list

3. Créer un dépôt GitHub

4. Se connecter sur [https://github.com/](https://github.com/)
5. Cliquer sur New repository.
6. Saisir le nom du dépôt.
7. Choisir sa visibilité : public
8. Cliquer sur Create repository.

9. Cloner le dépôt en local

10. Sur GitHub, ouvrir le dépôt créé.
11. Cliquer sur Code, puis copier l’URL HTTPS.
12. Ouvrir un terminal et se placer dans le dossier où enregistrer le projet.
13. Exécuter la commande suivante en remplaçant l’URL par celle du dépôt :

git clone

1. Entrer dans le dossier créé :

cd DEPOT

5. Vérifier le clonage

6. Vérifier le dépôt courant :

git status

1. Vérifier le lien avec GitHub :

git remote -v

1. Vérifier la branche active :

git branch

6. Faire une capture d’écran

7. Afficher les résultats des commandes dans le terminal.
8. Garder la date et l’heure visibles à l’écran.
9. Prendre une capture d’écran montrant les vérifications effectuées.