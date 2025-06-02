
# Jeudi: Meta SDK

## Matin – C’est quoi le Meta Blocks SDK ?

Aujourd’hui, nous allons nous familiariser avec le Meta Blocks SDK.  
Le cours sera ajusté en fonction de ce que vous avez déjà vu avec Arnaud sur OpenXR.  
Tutorial : https://youtu.be/X9bGkqK8zbw

### Étapes :

* Installer **Meta Blocks**
* Ajouter les blocs suivants :
  * Le bloc pour le **passthrough**
  * Le bloc pour les **mains**
  * Le bloc pour les **manettes**
  * Le bloc pour les **espaces scannés**
  * Le bloc pour le **mesh 3D**

## Midi – Créons notre ChTK (Charleroi Toolkit)

**"Isoler pour mieux régner."**  
Voici une liste de propositions pour créer une boîte à outils qui n’utilise que des **transforms** et des **meshes**.  
**Pas besoin d’OpenXR ni de Meta SDK pour cet exercice.**    

### Objectif :

Créer entre **7 et 20 boîtes à outils** séparées, puis les rassembler dans un **Charleroi Toolkit**, votre boîte à outils de groupe.
Voir: https://github.com/EloiStree/HelloUnityPackage/wiki  

Dans la liste suivante, choisissez une idée selon votre niveau. Chaque élève prend un sujet différent.

- [ ] Créer un script C# capable de détecter si ce sont les **mains** ou les **manettes** qui sont utilisées.
- [ ]  Détecter si la main est **plate** et orientée vers la **tête du joueur**.
- [ ]  Créer une boîte à outils permettant de déclencher des actions quand vos **doigts touchent votre pouce** :
  - [ ]  Détecter la distance entre deux points pour créer un **pinch**.
Créer un **curseur contextuel** pour les meshes de la pièce :
- [ ]  Voir : [Raycast – HelloUnityKeywordForJunior #70](https://github.com/EloiStree/HelloUnityKeywordForJunior/issues/70)
- [ ]  Faire apparaître :
  - [ ]  des **plantes** sur le plafond
  - [ ]  des **objets** sur les murs
  - [ ]  des **meubles** sur le sol
  - [ ]  des **ustensiles** sur les tables


Voici une version corrigée et améliorée de ton texte en gardant le ton informel et pédagogique :

---

###  Vendredi

Pour placer des objets dans un espace 3D, il faut savoir **trianguler**.
Mon objectif est de vous transmettre ce savoir que j’ai mis plusieurs semaines à explorer,
afin que vous puissiez l’utiliser ensuite en VR et en AR, avec l’aide des caméras.

---

###  Mardi

Je vais passer le week-end à rattraper mon retard sur le **Camera API**.
Je vous proposerai donc un cours sur ce que j’aurai appris durant ces trois jours.
Nous en profiterons pour voir — ou revoir — ce qu’est une **Texture2D** dans Unity3D.

---

###  Mercredi

Vous pouvez travailler sur l’image captée par la caméra du casque,
soit avec **OpenCV**, soit avec **Sentry**.
Mais il serait préférable d’exécuter ce traitement sur un serveur local ou en ligne.

Explorons ensemble comment **exporter l’image depuis le Camera API du Quest**
vers un **serveur WebSocket ou FTP**, pour la traiter avec des bibliothèques Python
et des outils de type **LM Studio**.


---------------

https://github.com/alvr-org/ALVR








---

### Tâches de fond à ne pas oublier :

* Maintenir un **Git** propre et présentable.
* Tenir à jour un **profil LinkedIn** professionnel.
* Définir **quatre mots** qui résument votre carrière dans les deux années à venir.
* Approfondir votre connaissance de **C# un peu chaque jour** :
  * [Suivre ce tableau d'exercices](https://docs.google.com/spreadsheets/d/15BQ1OqLn9omeHH6yPuqSO0Ip6XeQ0CktMDebbJCkarU/edit?gid=111671064#gid=111671064)
* Bonus :
  * [QwertyWar](https://www.qwertywar.com)
  * [Speed Typing Online](https://www.speedtypingonline.com/typing-test)



------------
- https://github.com/alvr-org/ALVR
  - https://youtu.be/oY_S5ok6keo?t=154
- https://github.com/oculus-samples/Unity-PassthroughCameraApiSamples/
- https://github.com/oculus-samples/Unity-DepthAPI.git?path=/Packages/com.meta.xr.depthapi.urp

===========================
- https://docs.google.com/spreadsheets/d/15BQ1OqLn9omeHH6yPuqSO0Ip6XeQ0CktMDebbJCkarU/edit?gid=111671064#gid=111671064
- Exercice C# Wow Level Up:
  - https://github.com/EloiStree/2025_02_03_MonsLevelUpInGroup
- Char in C# https://github.com/EloiStree/HelloSharpForUnity3D/issues/557
