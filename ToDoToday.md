- [ ] https://github.com/EloiStree/2025_06_05_TwoPointsQuadLoader
- [ ] https://github.com/EloiStree/2020_06_06_GizmoTools
- [ ] https://github.com/EloiStree/2025_06_05_DebugDrawUtility

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






==========================

========================

# Triangulation

Mon exemple le plus simple : essayer de voir si la main d'un joueur est à gauche, à droite ou au-dessus de la tête du joueur.

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

- GetCrossProductAtMiddle
- GetCentroid
- GetClosestPoint
- GetFarestPoint


   public interface I_ThreePointsGet
   {
       public void GetPoints(out Vector3[] arrayOf3);
       public void GetPoint(ThreePointCorner corner, out Vector3 point);
       public void GetThreePoints(out Vector3 start, out Vector3 middle, out Vector3 end);
   }
  
    public enum ThreePointCorner { Start, Middle, End }








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

## 
 


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




-----------------

https://github.com/EloiStree/HelloUnityKeywordForJunior/issues/176





---------------
[![image](https://github.com/user-attachments/assets/bf1592af-738e-43a7-abce-24e7fd723ed9)](https://youtu.be/bYWZ_lQKzb8)
https://youtu.be/bYWZ_lQKzb8  
[![image](https://github.com/user-attachments/assets/8d657fd4-e1d1-4057-a685-a955f492668c)](https://www.linkedin.com/posts/christoph-spinger-280621190_ballee-gameon-metaquest3-ugcPost-7335641936856281088-Adyq?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAbZXakBIv3dUUeyXBKfnq58XyNESFvicZo)  



Make your toolboxes but dont make it too big. Split it.
```
  Eloi.E_DrawingUtility.DrawLines(dt, pointsLineToGround, middle, flatMiddle);
  Eloi.E_DrawingUtility.DrawLines(dt, pointsLineToGround, end, flatEnd);
```

------------

[![image](https://github.com/user-attachments/assets/6e25d9d5-096a-48cf-8234-6adbe5cae58a)](https://img-9gag-fun.9cache.com/photo/apRAYP8_460svav1.mp4)
https://img-9gag-fun.9cache.com/photo/apRAYP8_460svav1.mp4
https://img-9gag-fun.9cache.com/photo/apRAYP8_460svav1.mp4
