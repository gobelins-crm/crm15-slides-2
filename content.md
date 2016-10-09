class: center, middle, inverse
# Workshop Mobile Java/Android
## CRM15 - 2ème année
---

class: center, middle, inverse
# Modalités
---

.left-column[
## Modalités
### - Rendu
]

.right-column[
# .center[Dimanche 23 octobre 2016 à 11h59]
]
---

.left-column[
## Modalités
### - Rendu
### - Rendu intermédiaire
]

.right-column[
# .center[Jeudi 13 octobre 2016 à 16h29]
]
---

.left-column[
## Modalités
### - Rendu
### - Rendu intermédiaire
### - Présentation orale
]

.right-column[
# .center[Vendredi 14 octobre 2016 à 14h00]
]
---

.left-column[
## Modalités
### - Rendu
### - Livrables
]

.right-column[
### Claroline
- Zip des sources
- Apk de l'appli
- Vidéos / captures d'écrans
- README.md / Document d'info sur votre projet
  - Lien vers le dépôt Git

### Dépôt Git
- Projet complet versionné depuis la première ligne de code
- Historique des commits reflétant tout votre travail
- README.md _le document d'info complet_

### Présentation
- ~2 slides
- 5 minutes de présentation
- 10 minutes de questions et discussion
]
---

.left-column[
## Modalités
### - Rendu
### - Livrables
### - Barême
]

.right-column[
# Oral

## Ce qui rentre dans les critères d’évaluation :
- Présentation claire et concise       : __4 points__
- Argumentation des choix techniques   : __4 points__
- Argumentation des choix fonctionnels : __4 points__
- Pertinence des réponses              : __4 points__
- Attitude pendant le workshop         : __4 points__

## Ce qui ne rentre pas dans les critères d’évaluation :
- design des slides
]
---

.left-column[
## Modalités
### - Rendu
### - Livrables
### - Barême
]

.right-column[
# Écrit

## Ce qui rentre dans les critères d’évaluation :
- Projet complet et fonctionnel : __5 points__
- Qualité du travail :            __5 points__
- Maîtrise des concepts Java :    __3 points__
- Maîtrise des concepts Android : __3 points__
- Ergonomie :                     __2 points__
- Qualité du code source :        __1 point__
- Gestion du projet :             __1 point__

## Ce qui ne rentre pas dans les critères d’évaluation :
- le graphisme
- les bugs mineurs
]
---

.left-column[
## Modalités
### - Rendu
### - Livrables
### - Barême
### - Planning
]

.right-column[
## Lundi
- Android 7.0 et Android Studio 2.2
- Rappel des patterns Android
- Rappel Firebase
- Java et annotations
- Architecture d'un projet

## Mardi
- Cryptographie

## Jeudi
- Rendu intermédiaire

## Vendredi
- Présentation
]
---

class: center, middle, inverse
# [Mr. Robot](http://www.whoismrrobot.com)
<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/Oc-AsN7d1wg" frameborder="0" allowfullscreen></iframe>
---

class: center, middle, inverse
# Android Nougat

[Android 7.0 for Developers](https://developer.android.com/about/versions/nougat/android-7.0.html)
---

.left-column[
## Android N
### - Multi-Window
]

.right-column[
## Multi-Window support
![img](https://developer.android.com/images/android-7.0/mw-splitscreen.png)

```
android:resizeableActivity=["true" | "false"]
```
```java
startDragAndDrop(ClipData, DragShadowBuilder,
    Object, DRAG_FLAG_GLOBAL)
```
]
---

.left-column[
## Android N
### - Multi-Window
### - Notifications
]
.right-column[
## Inline reply, grouping,
![img](https://developer.android.com/images/android-7.0/inline-type-reply.png)
## Grouping
![img](https://developer.android.com/images/android-7.0/inline-type-reply.png)

]
---

.left-column[
## Android N
### - Multi-Window
### - Notifications
### - Power saving
]
.right-column[
## Doze mode updated
![tiny_img](https://developer.android.com/images/android-7.0/doze-diagram-1.png)
![tiny_img](https://developer.android.com/images/android-7.0/doze-diagram-2.png)
]
---

.left-column[
## Android M
### - Multi-Window
### - Notifications
### - Power saving
### - Data saving
]
.right-column[
```java
ConnectivityManager connMgr = (ConnectivityManager)
        getSystemService(Context.CONNECTIVITY_SERVICE);
if (connMgr.isActiveNetworkMetered()) {
  // Checks user’s Data Saver settings.
  switch (connMgr.getRestrictBackgroundStatus()) {
    case RESTRICT_BACKGROUND_STATUS_ENABLED:
    // Background data usage is blocked for this app.

    case RESTRICT_BACKGROUND_STATUS_WHITELISTED:
    // The app is whitelisted.

    case RESTRICT_BACKGROUND_STATUS_DISABLED:
    // Data Saver is disabled.
  }
} else {
  // The device is not on a metered network.
}
```
]
---

.left-column[
## Android M
### - Multi-Window
### - Notifications
### - Power saving
### - Data saving
### - Direct Boot
]
.right-column[
```java
<receiver
  android:directBootAware="true" >
  ...
  <intent-filter>
    <action android:name="android.intent.action.ACTION_LOCKED_BOOT_COMPLETED" />
  </intent-filter>
</receiver>
```
]
---

.left-column[
## Android Studio 2.2
### - OpenJDK 8
### - Layout Editor
### - Improved emulator
### - Instant run that works
]
.right-column[
![img](https://developer.android.com/studio/images/hero_image_studio_2-2.png)
]
