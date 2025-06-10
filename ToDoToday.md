
# To Do Today

Dans l'atelier, et dans votre futur emploi XR, vous allez devoir charger des murs invisibles pour le bâtiment et/ou charger des exercices localisés. Je ne serai plus là demain. Trouvez avec votre niveau un moyen de charger du contenu dans le bâtiment Technocité.

Permet de charger un prefab depuis une distance ou de relocaliser un niveau :
- [ ] [2025_06_05_TwoPointsQuadLoader](https://github.com/EloiStree/2025_06_05_TwoPointsQuadLoader.git)

Mesure faite avec Open Brush du bâtiment en groupe :
- [ ] [2025_05_20_MeasureOfTechnociteWithQuest3](https://github.com/EloiStree/2025_05_20_MeasureOfTechnociteWithQuest3.git)
  - [ ] Utiliser ROOT_CHARLEROI_STREE_ELOI pour créer votre niveau.

Utile :
- [ ] [2025_06_05_DebugDrawUtility](https://github.com/EloiStree/2025_06_05_DebugDrawUtility)
- [ ] [2024_10_19_RelocationRotation](https://github.com/EloiStree/2024_10_19_RelocationRotation)

Exercice pour junior :
- Invoquer un prefab horizontal et vertical.

Exercice pour médior :
- Relocaliser un niveau dans la pièce avec des "tags de distance".

Exercice pour senior :
- Trouver une manière de relocaliser votre niveau dans la pièce par vous-même 😅😜😁


-------------------------------


# To Do Today 2025 06 11

Comme dit vendredi, mon but est de vous faire pratiquer durant une journée les rotations et translations avec des Vector3, Euler et Quaternion.

Vous trouverez plus bas une liste de sujets à éliminer.
Vous ne les ferez pas tous en une journée.

Vous aurez probablement besoin de ceci pour vous en sortir :
- [ ] https://github.com/EloiStree/2020_06_06_GizmoTools
- [ ] https://github.com/EloiStree/2025_06_05_DebugDrawUtility
- [ ] https://github.com/EloiStree/2024_10_19_RelocationRotation

Mercredi, c'est aussi une journée de pratique mais sur le positionnement d'objets dans le bâtiment avec le code de vendredi : https://github.com/EloiStree/2025_06_05_TwoPointsQuadLoader

--------------------

Dans le but de vous donner des exemples de rotation, j'ai passé le week-end à faire une vidéo sur comment créer le grab de Open Brush appliqué à un mouvement de drone.
J'y ai ajouté un canon pour refaire en vidéo l'exercice de vendredi.
![image](https://github.com/user-attachments/assets/dfa63691-e155-4eb5-af22-ea93c1388684)

Un total de 8H... Beaucoup trop de matière pour une journée.
Deux vidéos faciles à pratiquer si vous ne faites pas l'exercice au complet :
- Calculer le roll avec des cross product pour faire un volant de voiture
  - https://www.youtube.com/watch?v=ZLGrYFqCeGs
- Faire un canon de tank
  - https://youtu.be/XxiZXgC7NDk?t=3811

Le step by step total pour pratiquer les rotations, `Pinch Joystick` :
- Introduction à l'exercice
  - https://youtu.be/jXE9EZmj6RQ?t=7
- Calcul du roll à un volant de voiture
  - https://www.youtube.com/watch?v=ZLGrYFqCeGs
- D'une direction locale à un drone qui bouge en pourcentage
  - https://youtu.be/8j7TjPTHQE8?t=4808
- Sauver une position start, stay et exit de deux points
  - https://youtu.be/QjNqzI2x7CA?t=286
- Utiliser le start et exit pour calculer le yaw, roll et autre info
  - https://youtu.be/KYeEUsV14WY?t=5047
- Lier la position de la main, le grab, de l'index et du pouce à notre code
  - https://youtu.be/yGx6T766WZQ?t=3
- Utiliser le Pinch Joystick pour bouger notre drone
  - https://youtu.be/AErE_1inpZI?t=2
- Ajoutons un canon pour s'entraîner à relocaliser de local à world
  - https://youtu.be/XxiZXgC7NDk?t=3770

Vidéo de Quad Loader qui utilise quelques rotations et cross product, A4 :
https://github.com/EloiStree/2025_06_05_TwoPointsQuadLoader
- https://www.youtube.com/watch?v=XPQT77vDt4w Introduction à l'exercice
- https://www.youtube.com/watch?v=bXiPIEok_10&t=5s Réflexion sur le sujet
- https://www.youtube.com/watch?v=1lBkZXi4XUQ De l'idée au code


Must watch avant de commencer, Euler et gimbal lock:
[![image](https://github.com/user-attachments/assets/6ab57c71-3272-4c18-8078-12c033b9019f)](https://youtu.be/zc8b2Jo7mno?t=81)  
https://youtu.be/zc8b2Jo7mno?t=81    


Liste des sujets utilisés dans les vidéos :

- Vector3.up et Vector3.Cross en image [https://youtu.be/jXE9EZmj6RQ?t=57](https://youtu.be/jXE9EZmj6RQ?t=57)
- Plan cartésien X Y Z Unity [https://youtu.be/jXE9EZmj6RQ?t=79](https://youtu.be/jXE9EZmj6RQ?t=79)
- Ajouter DebugDrawUtility à un assembly [https://youtu.be/ZLGrYFqCeGs?t=246](https://youtu.be/ZLGrYFqCeGs?t=246)
- Direction = Destination - origine [https://youtu.be/ZLGrYFqCeGs?t=608](https://youtu.be/ZLGrYFqCeGs?t=608)
- Vector3.Cross(axis, direction) [https://youtu.be/ZLGrYFqCeGs?t=669](https://youtu.be/ZLGrYFqCeGs?t=669)
- Milieu de deux points [https://youtu.be/ZLGrYFqCeGs?t=691](https://youtu.be/ZLGrYFqCeGs?t=691)
- Up, Forward, Right depuis deux points [https://youtu.be/ZLGrYFqCeGs?t=786](https://youtu.be/ZLGrYFqCeGs?t=786)
- Dessinez un plan cartésien [https://youtu.be/ZLGrYFqCeGs?t=893](https://youtu.be/ZLGrYFqCeGs?t=893)
- [ExecuteInEditor] [https://youtu.be/ZLGrYFqCeGs?t=945](https://youtu.be/ZLGrYFqCeGs?t=945)
- .Normalize() [https://youtu.be/ZLGrYFqCeGs?t=1102](https://youtu.be/ZLGrYFqCeGs?t=1102)
- Direction * float [https://youtu.be/ZLGrYFqCeGs?t=1152](https://youtu.be/ZLGrYFqCeGs?t=1152)
- Vector3.SignedAngle(dir, dir, axis) [https://youtu.be/ZLGrYFqCeGs?t=1263](https://youtu.be/ZLGrYFqCeGs?t=1263)
- OnChange UnityEvent [https://youtu.be/ZLGrYFqCeGs?t=1468](https://youtu.be/ZLGrYFqCeGs?t=1468)
- D'un angle à un pourcentage [https://youtu.be/ZLGrYFqCeGs?t=1998](https://youtu.be/ZLGrYFqCeGs?t=1998)
- Mathf.Clamp() Mathf.Clamp01() [https://youtu.be/ZLGrYFqCeGs?t=2000](https://youtu.be/ZLGrYFqCeGs?t=2000)
- Un pourcentage à une rotation d'un volant [https://youtu.be/ZLGrYFqCeGs?t=2592](https://youtu.be/ZLGrYFqCeGs?t=2592)
- Quaternion et Transform.rotation [https://youtu.be/ZLGrYFqCeGs?t=2631](https://youtu.be/ZLGrYFqCeGs?t=2631)
- Quaternion.Euler(x, y, z) [https://youtu.be/ZLGrYFqCeGs?t=2638](https://youtu.be/ZLGrYFqCeGs?t=2638)
- WorldQuaternion * Q.Euler() [https://youtu.be/ZLGrYFqCeGs?t=2638](https://youtu.be/ZLGrYFqCeGs?t=2638)
- Vector3/distance = Vector3 as Percent [https://youtu.be/8j7TjPTHQE8?t=1051](https://youtu.be/8j7TjPTHQE8?t=1051)
- Yaw à un Quaternion par Euler [https://youtu.be/8j7TjPTHQE8?t=1873](https://youtu.be/8j7TjPTHQE8?t=1873)
- `Qa * Qb != Qb * Qa` [https://youtu.be/8j7TjPTHQE8?t=2241](https://youtu.be/8j7TjPTHQE8?t=2241)
- Dessiner un point et son plan cartésien entre deux points [https://youtu.be/8j7TjPTHQE8?t=4196](https://youtu.be/8j7TjPTHQE8?t=4196)
- Bouger localement : Position + Q(Rotation) * (direction locale) [https://youtu.be/8j7TjPTHQE8?t=4933](https://youtu.be/8j7TjPTHQE8?t=4933)
- Transform.Translate(direction, Space.Self) [https://youtu.be/8j7TjPTHQE8?t=5101](https://youtu.be/8j7TjPTHQE8?t=5101)
- Transform.Rotate(euler, Space.World) [https://youtu.be/8j7TjPTHQE8?t=5101](https://youtu.be/8j7TjPTHQE8?t=5101)
- [Transform.InverseTransformPoint](https://docs.unity3d.com/6000.1/Documentation/ScriptReference/Transform.InverseTransformPoint.html) World to Local
- [Transform.TransformPoint](https://docs.unity3d.com/6000.1/Documentation/ScriptReference/Transform.TransformPoint.html) Local to World
- Enter Stay Exit de deux points explication [https://youtu.be/QjNqzI2x7CA?t=170](https://youtu.be/QjNqzI2x7CA?t=170)
  - `public struct` [https://youtu.be/QjNqzI2x7CA?t=887](https://youtu.be/QjNqzI2x7CA?t=887)
  - Struct comme variable et événement [https://youtu.be/QjNqzI2x7CA?t=980](https://youtu.be/QjNqzI2x7CA?t=980)
- Up Right Forward to Matrix4 to Quaternion [https://youtu.be/QjNqzI2x7CA?t=1278](https://youtu.be/QjNqzI2x7CA?t=1278)
  - Alternative : Quaternion.LookAt(V3, V3)
- `Nested Class` for UnityEvent [https://youtu.be/QjNqzI2x7CA?t=1846](https://youtu.be/QjNqzI2x7CA?t=1846)
- V3 direction = Q rotation * Vector3.forward [https://youtu.be/QjNqzI2x7CA?t=4059](https://youtu.be/QjNqzI2x7CA?t=4059)
- Quaternion.FromToRotation(from, to) [https://youtu.be/QjNqzI2x7CA?t=4079](https://youtu.be/QjNqzI2x7CA?t=4079)
- Roll et Cross dans une méthode statique [https://youtu.be/QjNqzI2x7CA?t=4450](https://youtu.be/QjNqzI2x7CA?t=4450)
- -Vector3 et Quaternion.Inverse() [https://youtu.be/KYeEUsV14WY?t=840](https://youtu.be/KYeEUsV14WY?t=840)
- Relocaliser un World à un espace local [https://youtu.be/KYeEUsV14WY?t=1011](https://youtu.be/KYeEUsV14WY?t=1011)
- Flat XZ Yaw [https://youtu.be/KYeEUsV14WY?t=2509](https://youtu.be/KYeEUsV14WY?t=2509)
- Vector3.Distance [https://youtu.be/KYeEUsV14WY?t=2822](https://youtu.be/KYeEUsV14WY?t=2822)
- Vector3.magnitude
- Delta de deux angles [https://youtu.be/KYeEUsV14WY?t=3732](https://youtu.be/KYeEUsV14WY?t=3732)
- Quaternion.Euler(0, 0, 40) * Vector.right (et non forward) [https://youtu.be/KYeEUsV14WY?t=4338](https://youtu.be/KYeEUsV14WY?t=4338)
- Clamp Vector3 [https://youtu.be/KYeEUsV14WY?t=4838](https://youtu.be/KYeEUsV14WY?t=4838)
- QuickFollowIt [https://youtu.be/yGx6T766WZQ?t=157](https://youtu.be/yGx6T766WZQ?t=157)
- LateUpdate [https://youtu.be/yGx6T766WZQ?t=177](https://youtu.be/yGx6T766WZQ?t=177)
- Démo du code jusqu'ici avec Meta SDK [https://youtu.be/yGx6T766WZQ?t=1142](https://youtu.be/yGx6T766WZQ?t=1142)
- Écouter à deux inputs avec des booléens [https://youtu.be/yGx6T766WZQ?t=1830](https://youtu.be/yGx6T766WZQ?t=1830)
- OnValidate [https://youtu.be/yGx6T766WZQ?t=1939](https://youtu.be/yGx6T766WZQ?t=1939)
- InputActionReference (hors sujet) [https://youtu.be/yGx6T766WZQ?t=2272](https://youtu.be/yGx6T766WZQ?t=2272)
  - action.Enable()
  - performed started et canceled
  - ReadValue<float>
- Détecter un pinch de doigts [https://youtu.be/yGx6T766WZQ?t=3934](https://youtu.be/yGx6T766WZQ?t=3934)
  - Vector3.Distance et threshold [https://youtu.be/yGx6T766WZQ?t=4060](https://youtu.be/yGx6T766WZQ?t=4060)
  - Mathf.Abs [https://youtu.be/yGx6T766WZQ?t=4467](https://youtu.be/yGx6T766WZQ?t=4467)
- Quaternion.identity [https://youtu.be/yGx6T766WZQ?t=4635](https://youtu.be/yGx6T766WZQ?t=4635)
- Explication des infos nécessaires pour faire un Grab à la Open Brush
  - Yaw Roll Scale Direction et Joystick3D
  - [https://youtu.be/AErE_1inpZI](https://youtu.be/AErE_1inpZI)
- Observer et relayer par des UnityEvent [https://youtu.be/AErE_1inpZI?t=658](https://youtu.be/AErE_1inpZI?t=658)
- LET'S CREATE A CANNON [https://youtu.be/XxiZXgC7NDk?t=19](https://youtu.be/XxiZXgC7NDk?t=19)
- Q canon local = Q horizontal * Q vertical [https://youtu.be/XxiZXgC7NDk?t=1171](https://youtu.be/XxiZXgC7NDk?t=1171)
- Point local à un point global [https://youtu.be/XxiZXgC7NDk?t=1779](https://youtu.be/XxiZXgC7NDk?t=1779)
  - V3 World = (Q rotation * V3 localPoint) + V3 destination [https://youtu.be/XxiZXgC7NDk?t=1808](https://youtu.be/XxiZXgC7NDk?t=1808)
  - Q tourelle = Q tank * Q.Euler(rotation locale) [https://youtu.be/XxiZXgC7NDk?t=2598](https://youtu.be/XxiZXgC7NDk?t=2598)
- Bouger la tourelle sur le temps avec un pourcentage [https://youtu.be/XxiZXgC7NDk?t=3530](https://youtu.be/XxiZXgC7NDk?t=3530)


Note: https://github.com/EloiStree/2025_06_07_PinchJoysticks.git
- ExPinchMono_LocalComputeForCartesianTwoPoints
- ExPinchMono_RelayBasicFromLocalComputeCTP

Autre:
- https://github.com/EloiStree/HelloUnityKeywordForJunior/blob/main/Guide/Relocation.md
- Une perle https://github.com/EloiStree/HelloUnityKeywordForJunior/issues/240
- Attribute de Unity https://github.com/EloiStree/HelloSharpForUnity3D/issues/429
==================

======================

# Brouillons de l autre jour

==================


--------------------


Ce cours est chiant et difficile. Si vous n'avez pas mal à la tête vendredi soir, vous ne l'avez pas pratiqué. Mais il est une garantie d'emploi pour l'année 2025/2026.

**Objectif** : Recalibrer un espace virtuel sur un espace réel en utilisant la caméra du Quest 3 ! Si vous savez faire ça, vous avez un pied dans l'industrie.

# Relocalisation

Mon professeur de mathématiques m'avait enseigné une idée que j'utilise depuis mes 10 ans dans le jeu. C'est plus facile de faire des maths dans un espace choisi.

Je vais donc vous apprendre à relocaliser un espace en zéro zéro : [2024_10_19_RelocationRotation](https://github.com/EloiStree/2024_10_19_RelocationRotation).

L'exercice est simple : la main droite du joueur est-elle à gauche et au-dessus de sa tête en VR ?

Autres exemples :
- La main du joueur est-elle à plat au-dessus d'une surface ?
- Les deux manettes sont-elles en position d'inversion ?
- Le joueur est-il en train de montrer un gros poisson ?
- Le joueur regarde-t-il en l'air ?
- Le joueur regarde-t-il dans la direction d'un monstre ?
- Le joueur a-t-il les mains en l'air ?
- Le joueur a-t-il les mains sur la table ?
- Les points du cube sont ils dans la vue de la camera ?
- Le joueur est-il en [position de guillotine](https://youtu.be/N8zkbl6mKXE?t=4) ?
- Signe de mains
  - L index et le pouce de la main forme, ils un trianble
  - Les pouces et les indexes forment ils une ligne
  - Les pouces et les indexes forment ils une un cube
  

Exercice d'hier :
- [ ] https://youtu.be/1lBkZXi4XUQ

Exercice d'aujourd'hui:
- [ ] Pratiquer et comprendre l exercice d hier
  - [ ] Sauver les projets Git
  - [ ] Charger une feuille A4 avec un asset de SketchFab
  - [ ] Charger un niveau sur une table
  - [ ] Challenge:
    - [ ] Charger un niveau dans la salle commune
    - [ ] Charger un niveau sur l'ecran
- [ ] Pratiquer la relocalisation
  - [ ] Local To World: Creeons un canon.
  - [ ] World To Local: Creons un joystick avec nos doights

==========================

========================

Je dois voir avec vous :
- [ ] Euler vs Quaternion
  - [ ] Pitch, Yaw, Roll
- [ ] Produit vectoriel (Cross Product)
- [ ] Quaternion * Vector.Forward
- [ ] Qa * Qb n'est pas égal à Qb * Qa
- [ ] Aplatir une donnée sur un plan 2D relocalisé
- [ ] DrawLine
- [ ] Raycast
  - [ ] Détecter un plafond
  - [ ] Détecter un mur
  - [ ] Détecter une table
  - [ ] Détecter un sol
- [ ] Angle et Distance
  - [ ] Le doigt touche-t-il ?
  - [ ] Montre-t-il un gros poisson ?
- [ ] Relocalisation
  - [ ] Un objet est-il à droite d'un autre ?
  - [ ] Les mains du joueur sont-elles en l'air ?
  - [ ] Les mains du joueur sont-elles devant ?
  - [ ] Un joueur est-il en train de ramper ?








--------------

Pour le fun, regardons a ce que j ai utiliser pour replacer des objets.
https://github.com/EloiStree?tab=repositories&q=2024_10_17_ThreePoints&type=&language=&sort=
https://github.com/EloiStree/2024_10_17_ThreePointsTag
https://github.com/EloiStree/2024_10_17_ThreePointsTag/blob/main/Runtime/ThreePointsMono_Transform3.cs

-------------------------------------

-------------------------------------

# Jeudi: Meta SDK

## Matin – C’est quoi le Meta Blocks SDK ?

Aujourd’hui, nous allons nous familiariser avec le Meta Blocks SDK.  
Le cours sera ajusté en fonction de ce que vous avez déjà vu avec Arnaud sur OpenXR.  
Installer Meta XR : https://youtu.be/X9bGkqK8zbw

### Étapes :

* Installer **Meta Blocks**
* Ajouter les blocs suivants :
  * Le bloc pour le **passthrough**
  * Le bloc pour les **mains**
  * Le bloc pour les **manettes**
  * Le bloc pour les **espaces scannés**
  * Le bloc pour le **mesh 3D**


---

###  Vendredi

- Placer des objets dans un espace 3D via une "feuille de papier".
- Apprendre a relocaliser des points dans l espace.

---

###  Mardi

Je vais passer le week-end à rattraper mon retard sur le **Camera API**.
Je vous proposerai donc un cours sur ce que j’aurai appris durant ces trois jours.
Nous en profiterons pour voir — ou revoir — ce qu’est une **Texture2D** dans Unity3D.

---

###  Mercredi

Vous pouvez travailler sur l’image captée par la caméra du casque,
soit avec **OpenCV**, soit avec **Sentry**, soit avec **Shader Graph**.
Mais il serait préférable d’exécuter ce traitement sur un serveur local ou en ligne.

Explorons ensemble comment **exporter l’image depuis le Camera API du Quest**
vers un **serveur WebSocket ou FTP**, pour la traiter avec des bibliothèques Python
et des outils de type **LM Studio**.





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




-----------------

https://github.com/EloiStree/HelloUnityKeywordForJunior/issues/176


---------------
[![image](https://github.com/user-attachments/assets/bf1592af-738e-43a7-abce-24e7fd723ed9)](https://youtu.be/bYWZ_lQKzb8)
https://youtu.be/bYWZ_lQKzb8  
[![image](https://github.com/user-attachments/assets/8d657fd4-e1d1-4057-a685-a955f492668c)](https://www.linkedin.com/posts/christoph-spinger-280621190_ballee-gameon-metaquest3-ugcPost-7335641936856281088-Adyq?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAbZXakBIv3dUUeyXBKfnq58XyNESFvicZo)  




------------

[![image](https://github.com/user-attachments/assets/6e25d9d5-096a-48cf-8234-6adbe5cae58a)](https://img-9gag-fun.9cache.com/photo/apRAYP8_460svav1.mp4)
https://img-9gag-fun.9cache.com/photo/apRAYP8_460svav1.mp4
https://img-9gag-fun.9cache.com/photo/apRAYP8_460svav1.mp4


-----------------------
-----------------------------

## Autre – Créons notre ChTK (Charleroi Toolkit)

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
