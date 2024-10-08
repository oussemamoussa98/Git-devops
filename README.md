# Mon Projet
**Comment vérifier la configuration actuelle de Git sur votre machine, notamment le nom
d’utilisateur et l’adresse e-mail ?**
git config --list


**Comment modifier votre adresse e-mail si vous l'avez mal configurée lors de l'installation
de Git ?**
git config --global user.email "mohamedamine.benfredj@polytechnicien.tn"
touch README.md
echo "# Mon Projet" > README.md
git add README.md
git commit -m "Ajout du README.md"


**Si vous avez oublié de créer un fichier README.md lors de l'initalisation du projet,
comment pouvez-vous l'ajouter après coup et commiter les changements ?**
git remote add origin git@github.com:votre-utilisateur/mon-projet.git


**Comment annuler les modifications locales d'un fichier avant de les ajouter à l'index ?**
git checkout -- <fichier>

**Comment visualiser les fichiers qui sont prêts à être commités dans Git (staging) ?**
 git status


**Comment suivre (track) un dépôt distant et récupérer toutes les branches de ce dépôt ?**
git fetch --all

 **Comment supprimer une branche locale après l'avoir fusionnée dans master ?**
 git branch -d ma-fonctionnalite
 
**Comment interrompre un rebase en cours si vous avez commis une erreur ?**
git rebase --abort

**Comment lister les commits qui vont être rebasés avant de lancer un rebase ?**
git log ma-fonctionnalite ^master

**Comment afficher la liste des branches ac�ves et en cours de développement dans
Gi�low ?**
git flow feature list

**Comment annuler une branche de correc�f (ho�ix) avant de la finaliser si vous constatez
une erreur ?**
git flow hotfix finish mon-correctif
git branch -d mon-correctif
