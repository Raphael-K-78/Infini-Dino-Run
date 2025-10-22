# Infini Dino Run - Chrome Dino sans fin !

Ce petit script JavaScript permet de **rendre le jeu Chrome Dino infini**   
Le dinosaure ne meurt plus, et tu peux courir éternellement sans "Game Over" 

---

## Fonctionnement
Le jeu Chrome Dino repose sur un objet JavaScript interne appelé `Runner`.  
Ce script **désactive temporairement** les fonctions internes `gameOver()` et `stop()` pour empêcher la fin du jeu, puis les rétablit ensuite si tu veux rejouer normalement.

---

## Code utiliser
### Empecher le GameOver
```js
GameOver = Runner.prototype.gameOver;
Pause = Runner.prototype.stop;

// Désactivation des fonctions de fin / pause
Runner.prototype.gameOver = function(){};
Runner.prototype.stop = function(){};
```
### Réactiver le GameOver
```js
Runner.prototype.gameOver = GameOver;
Runner.prototype.stop = Pause;
```

---

## Comment utiliser
### 1 - Ouvrir le jeu Dino
- Tape `chrome://dino` dans ta barre d’adresse (ou déconnecte ton Wi-Fi et ouvre n’importe quelle page)

### 2 - Ouvrir la console développeur
- Raccourci:
    - `Ctrl + Shift + I` (Windows / Linux)
    - `Cmd + Option + I` (Mac)
- Va dans l’onglet Console

### 3 - Colle le code
- Copie/colle le code ci-dessus dans la console
- Appuie sur Entrée


### 4 - Lance le jeu
Appuie sur la barre d’espace pour commencer

🎉 Le jeu devient maintenant infini ! Le dinosaure ne mourra plus.

---

## Remmetre par défault
### 1 - Ouvrir la console développeur
- Raccourci:
    - `Ctrl + Shift + I` (Windows / Linux)
    - `Cmd + Option + I` (Mac)
- Va dans l’onglet Console

### 2 - Colle le code
- Copie/colle le code ci-dessus dans la console
- Appuie sur Entrée

---

## Remarques
- Ce script ne modifie rien de permanent : il agit seulement en mémoire pendant que la page est ouverte.
- Si tu rafraîchis la page, le comportement normal revient automatiquement.
- C’est un hack basique, qui as seulement pour but de s'amuser

---

## Auteur
Created by [Raphaël K.](https://github.com/Raphael-K-78)

---

## Licence
Ce projet est distribué sous licence MIT.
Libre à toi de le modifier et le réutiliser.