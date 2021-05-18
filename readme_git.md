## Initialisation d'un repositery :

Repository : dépot git, il garde en mémoire les changements appliqués à un projet.

Pour initialiser `git init` dans un un invité de commande, dans l'espace souhaité de travail.

## ajouter des fichiers au commit

Commit : Checkpoint dans l'avancé du projet (un point de sauvegarde), il retiet qui a fait le commit, quad, quand, et quels fichiers sont concerné par le commit. On lui donne un message qui sert a informer les autres utilisateurs.

Pour ajouter des fichiers au prochain commit, on passe par la commande `git add monFichier.truc`. Si on veux ajouter tous les fichiers qui ont été modifiés : `git add.`

##verifions le status de git (avant de faire des betises) :

On peut verifier l'état de git avec la commade `git status`
Elle nous donnera les infos  :
- La branche sur laquelle on est
- Les fichiers qui ont été modifiés
    - tracké (pret à l'envoi en commit)
    - non tracké

## Effectuer un commit

Pour envoyer le commit à git (faire un checkpoint): `git commit -m "mon message de commit"`

Il existe plusieurs conventions pour les messages de commit, celle d'angular est la plus propre : `git commit -m "Feature/Connexion(fichiers modifiés): ce qui a été fait sur ce commit"` 

## ajouter un repository distant (remote)

Il faut créer un repo sur l'hebergeur Git de votre choix (Github, gitlab, Bitbucket, etc).

Il faut ensuite renseigner le repository distant au repo local : 
`git remote add origin url-du-remote`.

> origin fait référence à une variable locale, vous avez le choix de son nom.

###Envoyer les commits

Pour que le repository distant récupère les modifications(commits), il faut lui envoyer.
`git push branche-distante branche-locale`
Exemple : `git push origin main`
