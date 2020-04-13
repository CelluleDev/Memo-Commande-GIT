# Il s'agit d'un modèle de fichier .gitignore pour les projets WordPress gérés par git.
# Fait: vous ne voulez pas de fichiers de base WordPress ou de votre serveur
# fichiers de configuration, etc., dans le référentiel de votre projet. Ce n'est tout simplement pas le cas.
#
# Solution: collez ce fichier dans la racine de votre référentiel (qu'il suppose être
# également le répertoire racine WordPress) et ajouter des exceptions pour tous les plugins,
# thèmes et autres répertoires devant être sous contrôle de version.
#
# Voir les commentaires ci-dessous pour plus d'informations sur la façon d'ajouter des exceptions pour votre
# contenu. Ou consultez la documentation de git pour plus d'informations sur les fichiers .gitignore:
# http://kernel.org/pub/software/scm/git/docs/gitignore.html

# Ignorez tout à la racine sauf le répertoire "wp-content".
/ *
! .gitignore
! wp-content /

# Ignore tout dans le répertoire "wp-content", sauf les "plugins"
# et répertoires "thèmes".
wp-content / *
! wp-content / plugins /
! wp-content / thèmes /

# Ignorez tout dans le répertoire "plugins", à l'exception des plugins que vous
# spécifier (voir les exemples commentés pour des conseils sur la façon de procéder.)
wp-content / plugins / *
# ! wp-content / plugins / my-single-file-plugin.php
# ! wp-content / plugins / mon-répertoire-plugin /

# Ignorez tout dans le répertoire "thèmes", à l'exception des thèmes que vous
# spécifier (voir l'exemple commenté pour une astuce sur la façon de procéder.)
wp-content / thèmes / *
# ! wp-content / themes / mon-theme /
