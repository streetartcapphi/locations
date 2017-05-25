# Locations
Entrepot pour les données affichées dans le site [https://streetartcapphi.github.io/map/](https://streetartcapphi.github.io/map/)

pour modifier les données, vous devez être commiteur sur le projet, ou proposer une pull request pour validation.

## Workflow

Les posts sont inscrits dans le répertoire input, 

des robots créé des vues, dans le répertoire views


## Structures de données

les fichiers input sont des geojson, 
deux attributs pilotent la publication :
- validated : savoir si une entrée a été validées
- mustbepublished : savoir si une entrée doit être publiée

l'entité est publiée uniquement si les deux attributs sont "vrais"

# Modifier les éléments non validés 


c'est ici : , on click sur l'entité, on est redirigé sur geojson.io, 

[https://streetartcapphi.github.io/map/?view=views/unvalidated/content.geojson&linkattribute=editURL](https://streetartcapphi.github.io/map/?view=views/unvalidated/content.geojson&linkattribute=editURL)

pour tout ceux qui n'ont pas été validés ce dernier mois glissant :



[https://streetartcapphi.github.io/map/?view=views/unvalidatebydate/0months/content.geojson&linkattribute=editURL](https://streetartcapphi.github.io/map/?view=views/unvalidatebydate/0months/content.geojson&linkattribute=editURL)



pour tout ceux qui n'ont pas été validés la semaine courante :
[https://streetartcapphi.github.io/map/?view=views/unvalidatebydate/0weeks/content.geojson&linkattribute=editURL](
https://streetartcapphi.github.io/map/?view=views/unvalidatebydate/0weeks/content.geojson&linkattribute=editURL)

il faut les droits d'écriture



## Editer les données bruts en tant que contributeur

Aller sur le site [http://geojson.io](http://geojson.io/#id=github:streetartcapphi/locations/blob/master/capphi.geojson&map=14/45.7535/4.8463)

puis loggez vous avec votre compte github, vous pouvez alors modifier le fichier geojson en utilisant la commande "open"/"github", 

L'éditeur vous permet de positionner les points, ajouter les attributs nécessaires

deux attributs sont strictement nécessaires : 

- imageURL : url de l'image affichée
- originURL : url du post pour être redirigé dessus

##Vues existantes

  - views/bydate/[XX]months/content.geojson  : posts du mois M - XX
  - views/bydate/[XX]weeks/content.geojson  : posts de la semaine S - XX
  - views/unvalidated/content.geojson : posts non validés encore (validated = false)  





