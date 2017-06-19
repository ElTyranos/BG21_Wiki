---
layout: default
---

# Welcome to Mission Maker Wiki

*Cette première page vous guidera à travers l'installation du framework selon que vous souhaitiez GM en PvP ou en CooP.*

Choisissez votre type de mission :
* [CooP](#préparer-lenvironnement-coop)
* [PvP](#préparer-lenvironnement-pvp)

<hr />

## Préparer l'environnement CooP
Rendez vous sur [](https://github.com/ElTyranos/BG21_Sandbox.altis) et enregistrez le template sur votre ordinateur.
![cliquez sur "clone or download > download zip"](http://i.imgur.com/zNMBhVI.jpg)

### Editer le nom du dossier
Extrayez le .zip dans le dossier _C:\Users\Username\Documents\Arma 3\mpmissions_. 
Pour changer la carte, il suffit de changer le suffixe du nom du dossier de **.altis** à **.nomdelacarte**.
Une fois cette étape effectuée, vous pouvez ouvrir la mission dans EDEN et passer à l'étape suivante.

### Préparer les slots et les loadouts
#### Réorganisation  
La mission étant préparée sur altis, il se peut que tout ce qui est préalablement placé (modules & unités) soit sous terre, hors carte ou dans les airs. Cela est du au système de géolocalisation des cartes et au réglage des coordonnées. Bref, recentrez tout au milieu, placez les unités au sol, placez les modules dans un coin hors de la carte pour éviter de les supprimer par inadvertance, lorsque vous serez en zeus, en voulant nettoyer une zone.

_Concernant les respawns, attendez l'étape suivante_

#### Slots    
Par défaut, la mission permet de jouer les 4 camps. Selon la mission que vous souhaitez faire, vous pouvez retirer des faction, supprimer des slots, en créer, changer leur équipement ou leurs attributs. On peut ainsi limiter les rôles selon le briefing que l'on a prévu.  
  
#### Joueurs pré-équipés  
Il existe plusieurs possibilités :  
* Forcer l'équipement en faisant _clic droit > edit loadout_. Cela ouvre le virtual arsenal et on peut équiper le joueur comme on le souhaite. Cette méthode est longue à réaliser mais est utile pour un départ immédiat en mission après le briefing au lobby.
* Créer un loadout vide contenant seulement l'uniforme, l'attribuer à tous les slots et remplir un arsenal virtuel limité sur une caisse de munition. Les joueurs s'équipent mais leur matériel est limité.

### Respawn
#### Possibilités
* Vous voulez que vos joueurs apparaissent dans une zone, vous pouvez ajouter un respawn dans l'éditeur. Attention, il faudra faire un "add to zeus" pour le modifier une fois en jeu.
* Vous voulez que vos joueurs commencent à un endroit précis (éparpillés, séparés, dans un bâtiment), ne mettez pas de respawn dans l'éditeur, ajoutez le au commencement de la mission.
* Véhicule sur lequel est attaché un respawn - placez un respawn dans EDEN, configurez le puis faites _clic droit > sync to_, cliquez le  véhicule et voilà, fini.

#### Important
Il est idéal de prendre l'habitude de toujours avoir un respawn pour chaque camp. En effet, si vous oubliez de mettre un spawn BLUFOR et que vous mourrez, vous n'aurez pas la possibilité, même en étant GameMaster, d'en replacer un nouveau. Vous n'aurez plus qu'à remballer.

<hr />

## Préparer l'environnement PvP
Rendez vous sur [](https://github.com/ElTyranos/BG21_PvP) et enregistrez le template sur votre ordinateur.
![cliquez sur "clone or download > download zip"](http://i.imgur.com/Zp2sHXa.jpg)

Allez dans EDEN, faites Fichier > Nouveau et choisissez la carte que vous souhaitez utiliser.  
_Ex : je choisi takistan_

Une fois sur la carte, enregistrez votre mission, ici j'enregistre ma mission dans "_MPMissions_" sous le nom de `BG21_PvP_Tuto`.

Dans _\Mes Documents\ArmA3\MPMissions_ je retrouve donc le dossier de ma mission `BG21_PvP_Tuto.takistan`

### __Attributs__
Attributes > General :  
* **Remplissez  vos infos :** nom de mission, auteur, etc.  
* _Changez l'allégeance des indépendants si nécessaire_.  
  
Attribues > Multiplayer :
* **Game Type :** Sandbox  
* **Enable AI :** désactivées par défaut dans le fichier _description.ext_
* **Respawn :** Tout est fixé dans le fichier _description.ext_ (temps de respawn réglé sur 2 heures)

### __Modules__
#### Module Radio  
Pensez à placer les modules Task Force ou ACRE2 selon ce que vous souhaitez.  
  
#### Module Game Master  
**Owner :** #adminLogged  
**Default addons :** All addons (including unofficial ones)  

#### Modules WMT  
Ils permettent de régler les paramètres de jeu, se référer à la suite du wiki.


[back](./)
