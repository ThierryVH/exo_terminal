# Défis Terminal

### Défi n°1
- Ouvrez le terminal (ctrl + t)
- Affichez le répertoire (ou dossier) de travail actuel. Cela permet de visualiser son chemin.
- Listez les éléments du dossier
- Créez un dossier *sites/*
- Listez les éléments du dossier
- Déplacez-vous dans le dossier *sites/*
- Une fois dans le dossier *sites/*, créez les dossiers *lab/* et *prod/*
- Listez les éléments du dossier
- Revenez dans le dossier *home/votre_utilisateur*

Cette architecture vous permettra d'organiser votre travail. Les projets en cours seront à placer dans le dossier *lab/*, et une fois terminés, vous les déplacerez dans le dossier *prod/*.

### Défi n°2
- Déplacez-vous à la racine de votre machine */*
- Listez les éléments du dossier
- Listez les éléments du dossier en affichant les dossiers et fichiers cachés, avec les détails (permissions d'accès, le nombre de liens physiques, le nom du propriétaire et du groupe, la taille en octets, et l'horodatage)
- Listez les éléments du dossier en affichant les dossiers et fichiers cachés, triés par ordre décroissant de modification
- Revenez dans le dossier *home/votre_utilisateur*

### Défi n°3
- Déplacez-vous dans le dossier *sites/lab/*
- Créez un dossier *prairie/*
- Déplacez-vous dans le dossier *prairie/*
- Créez un dossier *exo_terminal/*
- Listez le contenu du dossier *prairie/*
- Déplacez-vous dans le dossier *exo_terminal/*
- Créez 3 fichiers *Fichier1* - *Fichier2* - *Fichier3*
- Listez le contenu du dossier
- Supprimez le fichier *Fichier2*
- Listez le contenu du dossier pour vous assurer qu'il a bien été supprimé
- Renommer le fichier *Fichier3* en *Fichier2*
- Listez le contenu du dossier pour vous assurer qu'il a bien été renommé
- Revenez dans le dossier *home/votre_utilisateur*

### Défi n°4
- Depuis le dossier *home/votre_utilisateur*, listez le contenu du dossier *sites/lab/prairie/exo_terminal/*
- Créez un fichier *monFichier*
- Sans vous déplacer du dossier *home/votre_utilisateur*, copiez le fichier *monFichier* dans le répertoire *sites/lab/prairie/exo_terminal/*
- Depuis le dossier *home/votre_utilisateur*, listez le contenu du dossier *sites/lab/prairie/exo_terminal/* pour vous assurer qu'il a bien été copié
- Copiez à nouveau le fichier *monFichier* dans le répertoire *sites/lab/prairie/exo_terminal/*, mais cette fois en le renommant *monFichierRenomme* (Attention, dans le dossier *home/votre_utilisateur*, le fichier doit rester *monFichier* !)
- Listez à nouveau le contenu du dossier *sites/lab/prairie/exo_terminal/*
- Toujours depuis le dossier *home/votre_utilisateur*, créez un dossier *sites/lab/prairie/exo_terminal/dossier_a_supprimer/*
- Déplacez-vous dans le dossier *sites/lab/prairie/exo_terminal/dossier_a_supprimer/*
- Affichez le répertoire de travail actuel
- Listez le contenu du répertoire précédent (dossier "parent" qui n'est autre que *exo_terminal/*)
- Déplacez le fichier *monFichierRenomme* du répertoire *exo_terminal/* dans le répertoire *dossier_a_supprimer/*
- Listez le contenu du dossier *dossier_a_supprimer/*
- Déplacez-vous dans le dossier "parent" (Ce qui revient à revenir en arrière)
- Supprimez le dossier *dossier_a_supprimer/*
- Revenez dans le dossier *home/votre_utilisateur*

### Défi n°5
- Déplacez-vous dans le dossier *Desktop/* (ou *Bureau/*)
- Créez un raccourci (un lien symbolique et non un lien physique) qui pointe vers le dossier *exo_terminal/*
- Listez le contenu du dossier *Desktop/* (ou *Bureau/*) en affichant les détails. Remarquez que le chemin où pointe le raccourci est indiqué
- Déplacez-vous dans le dossier raccourci *exo_terminal/*
- Créez un dossier *test_lien_symbolique/*
- Déplacez-vous dans le répertoire *sites/lab/prairie/exo_terminal/*
- Listez le contenu du répertoire. On s'aperçoit que le dossier *test_lien_symbolique/* a bien été créé.
- Revenez dans le dossier *home/votre_utilisateur*

### Défi n°6
- Déplacez-vous dans le dossier *sites/lab/prairie/*
- Supprimez le dossier *exo_terminal/* ainsi que son contenu
- Listez le contenu du dossier courant pour s'assurer que la suppression s'est effectuée
- Créez un répertoire *exo_permissions/* et se déplacer dedans
- Créez un fichier *Fichier1*
- Créez un fichier *Fichier_sudo* en mode sudo
- Listez le contenu du répertoire. Quelle différence observez-vous?
- Changer le propriétaire du fichier *Fichier_sudo* pour qu'il vous appartienne (votre nom d'utilisateur)... Un problème? ;)

### Défi n°7
- Vous vous trouvez dans le dossier *sites/lab/prairie/exo_permissions/*
- Listez le contenu du dossier en détails et attardez vous sur le propriétaire et le Groupe
- Si le défi n°6 a bien été réalisé, le fichier *Fichier_sudo* devrait vous appartenir, mais appartient toujours au groupe *root*
- Modifier le groupe du fichier *Fichier_sudo* pour qu'il appartienne à votre groupe (votre nom d'utilisateur)
ex : -rw-r--r-- 1 thierry thierry 0 mai 22 11:21 Fichier_sudo
- Listez le contenu pour vous assurer des changements
- Supprimez le fichier *Fichier_sudo* et créez le à nouveau en mode sudo
- Modifier à nouveau le groupe du fichier *Fichier_sudo* pour qu'il appartienne à votre groupe. Qu'est ce qui a changé?
- Créez un fichier *blablabla* en mode sudo
- À vous de trouver la commande pour changer le propriétaire ET le groupe du fichier pour qu'il vous appartienne, tout ça en une seule commande !

### Défi n°8
- Vous vous trouvez dans le dossier *sites/lab/prairie/exo_permissions/*
- Listez le contenu du dossier en détails et attardez vous sur les permissions (ex: -rw-r--r--)
- Changez les permissions du fichier *Fichier1* pour lui donner les droits suivants:
		- Propriétaire : lecture, écriture et exécution
		- Groupe : lecture, exécution
		- Autres : lecture
- Changez les permissions du fichier *Fichier_sudo* pour lui donner les droits suivants:
		- Propriétaire : lecture, écriture et exécution
		- Groupe : exécution
		- Autres : lecture, exécution
- Listez le contenu du dossier en détails et attardez vous sur les permissions pour observer les changements
- Changer le propriétaire du fichier *Fichier_sudo* pour qu'il appartienne à *root*
- Déplacez-vous dans le dossier "parent"
- Changez les permissions du dossier *exo_permissions/* ainsi que son contenu (de façon récursive) pour lui donner les droits suivants:
		- Propriétaire & Groupe & Autres : lecture, écriture et exécution
