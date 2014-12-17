LOG
==========

# Définition
Script Shell sous Linux pour informer :
  - Affichage dans la console
  - Ecriture dans les logs
 
Lancement du script :
 ```shell
 ./printMassage.sh
```
# Pré-requis
La librairie des fonctions est requise
```shell
 #CHEMIN RACINE
 PATHROOT="$PWD"
 # RECUPERATION DES FONCTIONS
 . $PATHROOT/../lib/functions.sh
```
Le fichier de config est requis
```shell
 #RECUPERATION DES PROPERTIES
 . $PATHROOT/../config/config.sh
```
Il contient la définition de `$PATHDEST_FICLOG` (nom et chemin de fichier de log)

 


# Contenu
### J'affiche uniquement sur l'écran
Syntaxe  :
```shell
printMessageToUser "Message à afficher"
```

### J'affiche avec un style de formattage uniquement sur l'écran
Syntaxe  :
```shell
printFormatMessageToUser "Message à afficher"
```

### J'affiche uniquement dans le fichier de log $PATHDEST_FICLOG
Syntaxe  :
```shell
printMessageToLog "Message à afficher" "$PATHDEST_FICLOG"
```

### J'affiche avec un style de formattage uniquement dans le fichier de log  $PATHDEST_FICLOG
Syntaxe  :
```shell
printFormatMessageToLog "Message à afficher" "$PATHDEST_FICLOG"
```

### J'affiche à l'écran et dans le fichier de log $PATHDEST_FICLOG
Syntaxe  :
```shell
printMessageToLogAndUser "Message à afficher" "$PATHDEST_FICLOG"
```

### J'affiche avec un style de formattage à l'écran et dans le fichier de log  $PATHDEST_FICLOG
Syntaxe  :
```shell 
printFormatMessageToLogAndUser "Message à afficher" "$PATHDEST_FICLOG"
```