# Ville-3D-et-Minecraft
[<img width="250" alt="Minecraft" src="img/minecraft.jpg">](https://www.minecraft.net/fr-fr)

Il existe plusieurs possibilités pour importer des données 3d dans le jeu Minecraft (ou dans sa version libre [minetest](https://www.minetest.net/))

Nous allons ici en passer quelques unes en revue.

## Table des matières

Cliquer sur les liens ci-dessous pour accéder à la section

[Minecraft à la carte](#minecraft_carte)

[Worldpainter](#worldpainter)

[Tinkercad](#tinkercad)

[Voxélisation](#voxelisation)

[MCEdit](#mcedit)

[Informations Complémentaires](#EnPlus)

[Bibliographie](#bibliographie)

-----------------

## Minecraft à la carte <a name="minecraft_carte"></a>

### Site de l'IGN

[<img width="250" alt="Minecraft_site_internet" src="img/minecraft_a_la_carte.png">](https://minecraft.ign.fr/#) L'IGN propose un service qui permet de générer une carte lisible par le jeu Minecraft ou sa version gratuite Minetest à partir d'une emprise d'un maximum de 5km par 5km. 
Le site de l'IGN est accessible en cliquant sur l'image ci-contre ou avec ce [lien](https://minecraft.ign.fr/#).

La carte va être générée en fonction des données capitalisées par l'IGN et permet de retrouver la topographie du site ainsi que les bâtiments, cependant ceux-ci se ressemblent tous et il est nécessaire de prendre du recul pour bien reconnaître les lieux.

### Créer la carte

La première étape consiste à définir l'emprise de sélection des données : tout se passe dans l'onglet à gauche du site internet :

<img width="250" alt="minecraft_emprise" src="img/minecraft_emprise.png">

Il existe deux possibilités pour créer cette emprise, soit en renseignant une adresse, soit en utilisant l'option *par centrage* qui permet de positionner un axe xy sur la carte. Le centre de la carte étant défini, il faut maintenant rentrer les quelques options disponibles.

La première d'entre elle étant la plateforme sur laquelle se trouve le jeu (Windows 10, Linux, Mac ou encore Xbox...). Cette option sélectionnée ouvre la suivante, c'est à dire le format du jeu (c'est ici que l'on peut choisir le format minetest par exemple).

Ensuite des réglages avancés sont disponibles, c'est ici notamment que l'on peut régler la taille de l'emprise souhaitée.

<img width="250" alt="Minecraft_taille" src="img/minecraft_taille.png">

Il faut renseigner son mail, puis cliquer sur générer la carte, il y a un nombre limité de génération de cartes par jour pour l'ensemble des utilisateurs, si le compteur est à zéro, il faudra retenter sa chance le lendemain. De même, une seule carte par adresse mail par jour.

### Récupérer la carte et mettre le dossier au bon endroit

La carte est générée en plus en mois longtemps en fonction de l'emprise qui a été choisi. Elle est adressée par mail, il suffit de cliquer sur le lien pour télécharger le fichier zip (attention, le lien n'est valable que 72h).

L'étape suivante est assez simple il faut décompresser le fichier récupérer le dossier *_alac. C'est dans ce dossier que se trouve les fichiers qui vont permettrent de construire la carte.

Ce dossier doit simplement être déplacé au bon endroit en fonction du format choisi : 

* Dans le cas de Minecraft c'est par défaut dans le dossier : C: / Utilisateur / "Nom utilisateur" / AppData / Roaming / .minecraft / saves. 
C'est donc dans le répertoire *saves* qu'il faut copier le dossier *_alac

* Dans le cas de Minetest : C:\Program Files (x86)\minetest-*version*\worlds
C'est donc dans le répertoire *worlds* qu'il faut copier le dossier *_alac

### Jouer dans le monde créé avec minecraft à la carte

Enfin la dernière étape pour retrouver le monde créé, il suffit de lancer le jeu et de sélectionner le monde par exemple dans le cas de minetest :

<img width="500" alt="Minecraft_menu" src="img/minetest_menu.png">

Dans ce cas nous avons créé un monde en sélectionnant l'emprise du campus de Bron.

Nous pouvons constater sur la figure suivante que le monde généré ne correspond pas complètement à la réalité, sur l'image nous voyons le bâtiment E. L'IGN ne possède que l'emprise au sol des bâtiments, le résultat nous montre que les trois amphis avec leur forme circulaire et la partie nord du bâtiment.

<img width="500" alt="Minecraft_batE" src="img/minetest_batE.png">

Ceci étant dit, minecraft à la carte permet de générer facilement l'emprise d'un territoire existant et de s'en servir de base pour reproduire le plus fidèlement possible l'environnement. 

Démonstration sur Minecraft par Lubin avec une carte de Lyon.

<img width="500" alt="MC_ALAC_Lyon" src="img/MC_ALAC_Lyon.png">

-----------------

## Worldpainter <a name="worldpainter"></a>

World painter est un logiciel de génération de monde minecraft. Il se présente comme un outil permettant de "dessiner son monde" comme sur Paint.

A télécharger cliquant sur le lien suivant : [WorldPainter](https://www.worldpainter.net/)

<img width="500" alt="Interface_WorldPainter" src="img/Interface_WorldPainter.PNG">

World painter permet notamment d'importer des images laissant ainsi la possibilité d'importer des MNT (Modèle Numérique de Terrain) : menu "Edit" --> Import --> Height Map into current dimension

<img width="500" alt="ImportHeightMapWP" src="img/ImportHeightMapWP.PNG">

Une fois cette fenêtre ouverte, il faut ouvrir son MNT et paramétrer l'import dans World painter, en jouant sur l'échelle (Scale : à 100% par défaut ce qui signifie 1 pixel de l'image du MNT = 1 cube dans le jeu) et également sur le niveau de l'eau (Water Level)

<img width="500" alt="HeightMapLyon_WorldPainter" src="img/HeightMapLyon_WorldPainter.PNG">

Les paramètres d'import des MNT ne permettent pas de rendre le résultat correct, il faut alors utiliser les outils de "dessin" qu'offre World painter pour régler certains problème comme la gestion du niveau d'eau.

Une fois que le résultat est satisfaisant, il faut alors exporter le rendu
<img width="100" alt="ExportWP_Bouton" src="img/ExportWP_Bouton.PNG">

Pour paramétrer l'export, il faut d'abord lui donner un nom (Ce sera le nom du monde à ouvrir dans le jeu Minecraft). Il faut ensuite sélectionner les tuiles (Tiles) à exporter.

<img width="500" alt="ExportWP" src="img/ExportWP.PNG">

Il est important de ne pas modifier le chemin d'enregistrement de l'export, il est paramétré par défaut pour s'exporter au bon endroit.

Le résultat dans Minecraft :

<img width="500" alt="WorldPainterFourvière" src="img/WorldPainterFourvière.png">

-----------------

## Tinkercad <a name="tinkercad"></a>

Tinkercad est un logiciel en SAAS édité par Autodesk qui permet de créer gratuitement des objets en 3d pour de l'impression en 3D ou pour les exporter dans divers formats.

C'est un logiciel qui est assez simple d'utilisation, il existe plusieurs tutoriels sur internet pour le prendre en main. Le lien suivant est une vidéo youtube pour construire une maison : [tuto maison](https://www.youtube.com/watch?v=3LVAEuAWW_M).

Nous avons réalisé une forme de bâtiment très simple pour montrer le résultat : 

<img width ="500" alt="tinkercad_3D" src = "img/tinkercad_3d.png">

Tinkercad permet de visualiser le résultat de la modélisation transformé en bloc en cliquant sur l'icone suivante (à noter qu'il permet aussi la visualisation en briques légo) : 

<img width ="125" alt="tinkercad_bloc" src = "img/tinkercad_bloc.png">

Le résultat est le suivant : 

<img width ="500" alt="tinkercad_briques" src = "img/tinkercad_briques.png">

Il est possible de choisir le détail de la modélisation avec plus ou moins de bloc, donc plus ou moins de précision dans la représentation du bâtiment.

Une fois la construction du modèle 3d réalisé, il faut exporter le bâtiment au format voulu. Quand l'utilisateur est dans le mode conception 3d, il peut choisir plusieurs formats d'exports dont *.obj* et *.svg* ou choisir directement un modèle d'imprimante 3d.
Ce qui nous intéresse dans notre cas, c'est quand l'utilisateur est dans le mode bloc, quand il clique sur exporter le seul format d'export proposé est le *.schematic*, format que nous allons pouvoir exploiter avec Minecraft comme nous l'expliquons dans cette [section](#mcedit).

<img width ="250" alt="tinkercad_export" src = "img/tinkercad_export.png">

Cette solution permet de créer facilement des bâtiments et de les exporter dans un format qui est exploitable avec Minecraft, nous pouvons imaginer que combiné avec la création d'une carte depuis une emprise avec Minecraft à la carte, il peut être facile de reproduire l'environnement d'une ville avec ses bâtiments remarquables par exemple.

Ce n'est cependant pas la seule solution et nous allons voir dans la section suivante comment créer des fichiers schematic à partir de fichier *.obj*.

-----------------

## Voxélisation <a name="voxelisation"></a>

A partir d'un fichier .obj, il est assez facile de créer un fichier [schematic](https://www.minecraft-france.fr/tutoriel-les-schematics/) qui est un format d'échange de structure créé par la communauté de joueur minecraft. Ce type de format peut être chargé dans une carte grâce à MCedit que nous verrons plus [bas](#mcedit). Dans un premier temps, nous allons voir comment transformé un fichier .obj au format schematic.

### vox_package 

[vox_package](https://minecraft.gamepedia.com/Programs_and_editors/Binvox) est une archive qui comprend deux exécutables, un pour voxéliser (binvox) (passer un objet 3d texturé en cube) et l'autre pour visualiser (viewvox) le résultat de la voxélisation.

#### Installation des applications

Comme il s'agit d'une archive, il suffit de la télécharger puis de la dézippé à l'endroit souhaité. Pour utiliser au mieux les fonctions proposé par les deux exécutables, la ligne de commande est le plus simple, il faut donc pouvoir retrouver son dossier avec l'archive de la façon le plus simple possible. Dans l'exemple ci-dessous, le dossier se situe sur le bureau :

    cd C:/Users/"utilisateurs"/Desktop/vox_package

#### La voxélisation

L'exécutable binvox permet de voxéliser un fichier depuis plusieurs types de format : Wavefront OBJ, VRML 2.0, UG, OFF, DXF, XGL, POV, BREP, PLY, JOT. Dans la documentation, le format .obj semble le plus approprié pour cette opération.

En sortie, deux formats sont possibles : le .binvox qui peut être visualiser dans viewvox et schematic qui ne peut être visionné mais qui servira par la suite. 

Il est conseillé de faire une première sortie au format binvox afin de voir le résultat de la voxelisation. Ceci permet de régler les paramètres au fur et à mesure.

Pour lancer une voxélisation simple, la commande suivante doit être lancée depuis la ligne de commande dans le bon dossier (nous supposons ici que le fichier .obj se trouve dans le même dossier que l'exécutable).

    binvox {nom_fichier.obj}

La commande se lance, le fichier .obj est parcouru : 

<img width="400" alt="binvox" src="img/binvox.png">

En fonction de la taille, cela peut être plus ou moins long (plus de 25 min dans le cas du fichier Poleymieux terrain complet), dans le cas d'un petit fichier, à la fin du traitement nous apercevons furtivement le résultat du traitement :

<img width="250" alt="binvox" src="img/fin_binvox.png">

La commande a créé un fichier binvox qu'il est possible de voir avec viewvox en lançant la commande : 

    viewvox {nom_fichier.binvox}

La visionneuse se présente ainsi : 

<img width = "250" alt ="viewvox" src="img/viewvox.png">

Nous pouvons voir qu'elle est assez rudimentaire mais cependant suffisante pour voir le résultat. Les contrôles de zoom sont détaillés sur le [wiki](https://minecraft.gamepedia.com/Programs_and_editors/Binvox).

Ces deux opérations permettent d'affiner la voxélisation, en effet il y a plusieurs paramètres sur lesquels il est possible de jouer, notamment sur le nombre de cube générés ce qui déterminera la finesse de la figure finale. Ces paramètres sont détaillés dans le wiki cité ci-dessus.

Enfin lorsque la figure correspond au rendu souhaité, il est temps de créer le fichier .schematic avec la commande suivante :

    binvox {nom_fichier.obj} {parametre_1} {parametre_2} -t schematic

Les paramètres sont bien évidemment ceux déterminés lors des essais précéedents, le seul paramètre qui va changer cette fois et celui du format d'export, c'est le paramètre -t qui permet de préciser que le format sera du schematic.

Ainsi un fichier schematic est créé pour l'utiliser dans une carte minecraft il faut se reporter à la section [suivante](#mcedit)

-----------------------

## Import de fichiers schematic avec MCEdit <a name="mcedit"></a>

MC Edit est un éditeur pour monde minecraft : [MCEdit](http://www.mcedit.net/)

Il permet de modifier un monde déjà existant dans Minecraft

<img width="500" alt="MC_EditImportMonde" src="img/MC_EditImportMonde.PNG">

MC Edit permet notamment l'import de fichier au format ".schemactic" ce qui nous intéresse tout particulièrement pour importer les fichiers .obj voxelisé avec la méthode présenté dans la section précédente

<img width="500" alt="MC_EditImportSchematics" src="img/MC_EditImportSchematics.PNG">

Le résultat de l'import est souvent dans le mauvais sens, un ensemble d'outils permettent de régler ces soucis

<img width="500" alt="MC_EditImportSchematicsResult" src="img/MC_EditImportSchematicsResult.PNG">

<img width="500" alt="MC_EditChevalierSchematicsResult" src="img/MC_EditChevalierSchematicsResult.PNG">

Sur ces images, il ne s'agit pas d'une voxelisation d'un fichier .obj représentant un élément géographique. Pour obtenir un résultat satisfaisant, il faut que l'objet à importer soit suffisament détaillé.

Il est important de noter que Minecraft dispose d'un système de coordonnées ainsi les élements peuvent être déplacé en conséquence.

Pour importer réellement notre objet dans le monde minecraft choisi, il faut cliquer sur Confirm (en bas de l'image ci-dessus) puis sauvegarder.

Voici le résultat dans Minecraft :

<img width="500" alt="ChevalierImportMinecraft" src="img/ChevalierImportMinecraft.png">

## Informations Complémentaires <a name="EnPlus"></a>

* Minecraft est un jeu qui est limité en hauteur, la limite actuelle est fixé à 256 blocs, ce qui rend impossible la représentation à l'échelle 1:1 tout objet géographique dépassant 256 mètres de haut.
Comme nous pouvons le voir sur la dernière image de la section [Worldpainter](#worldpainter) où la hauteur de la colline de Fourvière est à l'échelle 1:1, cette dernière parait alors complétement disproportionnée. 
Pour allier l'ensemble des outils présenté dans ce tutoriel, dans l'objectif de représenter un bout de notre monde réel, il faut bien préparer les différents éléments en définissant le bon niveau de détails, la bonne échelle, les bonnes coordonnées relatives au jeu.

* Le projet Minecraft à la carte de l'IGN a donné lieu à un concours porté par le ministère de la cohésion des territoires et des relations avec les collectivités territoriales : [Concours Minecraft ALAC](http://www.cohesion-territoires.gouv.fr/jeu-concours-minecraft-cree-ta-ville-et-ton-territoire-de-demain)

* Il existe un projet qui a commencé en 2020 avec comme objectif de recréer la Terre entière à l'échelle 1:1 : [Projet BuildTheEarth](https://buildtheearth.net/)

## Bibliographie <a name="bibliographie"></a>

[minecraft à la carte](https://minecraft.ign.fr/#)

Pour pouvoir utiliser minecraft à la carte il faut bien faire attention à la version que ce soit pour minecraft ou minetest.
La version supportée de minetest est disponible ici : [minetest_04.16](https://github.com/minetest/minetest/releases/tag/0.4.16)

Une autre possibilité semble exister pour minetest : [cartOSM](https://framagit.org/marpa/cartosm-ign)

Tutoriel d'utilisation de minecraft à la carte : [tutoriel](https://www.wikidebrouillard.org/wiki/Ma_ville_bloc_par_bloc_-_reconstruire_sa_ville_avec_Minecraft_ou_Minetest)

[Génération de carte Minecraft avec WorldPainter](https://www.minecraftforum.net/forums/archive/tutorials/930401-mapping-using-real-world-terrain-data)

Générer des bâtiments 3d avec [tinkercad](https://square.banq.qc.ca/projets/tutoriel-transfert-dun-modele-3d-vers-minecraft/)
