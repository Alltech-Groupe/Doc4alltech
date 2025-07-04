# 🚀 PepITs Starter Pack – Alltech Consulting

_Bienvenue sur le dépôt du **Starter Pack PepITs**, une plateforme web simple, modulaire et responsive conçue pour organiser des ressources techniques par thématiques._

https://alltech-groupe.github.io/Doc4alltech/

---

## 📐 Structure générale

Le projet repose sur une structure HTML/CSS simple et responsive.  
La page principale contient :

- Un **header fixe** avec le titre du projet.
- Une **grille de catégories**, chaque catégorie représentant une thématique (ex : Front, Back, Testing…).
- À l’intérieur de chaque catégorie, une **grille de sous-catégories**, affichées sous forme de cartes cliquables.
- Un **footer** contenant des liens utiles.

### 🗂️ Catégorie

Chaque catégorie est définie par un bloc `<section class="category-container">`. Il contient :

```html
<section class="category-container">
  <div class="category-header">
    <div class="icon-circle">
      <i class="material-icons">engineering</i>
    </div>
    <span class="category-title">Nom de la catégorie</span>
  </div>
  <div class="item-grid">
    <div class="sub-grid">
      <!-- Sous-catégories ici -->
    </div>
  </div>
</section>
```
Composants principaux :
- category-container : le bloc global de la catégorie
- category-header : le bandeau contenant le badge icône et le titre
- icon-circle : un badge rond contenant une icône Material Icons
- category-title : le titre de la catégorie
- item-grid : la grille contenant les sous-catégories
- sub-grid : le cellule contenant la sous-catégorie qui seront dispersés dans la grille

### 🔸 Sous-catégorie
Chaque sous-catégorie est une carte cliquable composée d’un lien, d’une image illustrative et d’un titre :

```html
<a href="./categories/front/angular.html" class="item">
  <div class="card">
    <img src="./ressources/images/angular-icon.png" alt="sous-cetegorie">
    <span>Sous-Categorie</span>
  </div>
</a>
```
Composants principaux :
- a.item : lien vers la page de la sous-catégorie
- .card : la carte visuelle contenant :
  - une image (img)
  - un titre (span)

Chaque carte est responsive et peut inclure un effet de survol.

## ➕ Contribuer
### Ajouter une catégorie

Les catégories sont structurées sous forme de sections HTML comme ci-dessous :

```html
<section class="category-container">
  <div class="category-header">
    <div class="icon-circle">
      <i class="material-icons">engineering</i>
    </div>
    <span class="category-title">Nom de la catégorie</span>
  </div>
  <div class="item-grid">
    <div class="sub-grid">
      <!-- Sous-catégories ici -->
    </div>
  </div>
</section>
```

Pour ajouter une catégorie :

- Copier une section existante.

- Changer l’icône Material (voir plus bas).

- Modifier le titre.

- Ajouter des sous-catégories dans la item-grid.

### Ajouter une sous-catégorie
Les sous-catégories sont représentées par des cartes avec une image et un nom :

```html
<a href="./categories/front/angular.html" class="item">
  <div class="card">
    <img src="./ressources/images/angular-icon.png" alt="Angular">
    <span>Angular</span>
  </div>
</a>
```
Il suffit d’ajouter ce type de bloc dans la sub-grid correspondante.

## 🎨 Utilisation de Material Icons
Les icônes Material de Google sont utilisées pour illustrer chaque catégorie.
Elles sont intégrées via ce lien dans le <head> :

```html
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
```
Et appelées ainsi :

```html
<i class="material-icons">palette</i>
```
🔗 Icônes disponibles ici : https://fonts.google.com/icons

## 📁 Arborescence recommandée
```css
.
├── index.html
├── index.css
├── ressources/
│   ├── images/
│   │   ├── angular-icon.png
│   │   └── ...
│   └── polices/
│       └── Quicksand-Regular.ttf
└── categories/
    ├── front/
    │   └── angular.html
    ├── back/
    └── ...
```

## 📎 Structure des Pages Secondaires

Les pages secondaires sont des webpages dédiées au contenu de chaque carte utilisant le format style "GIT CHEAT SHEET".

Chaque page contient :

- Un **header fixe** avec le titre de la sous-catégorie, sous-titre de la catégorie et un lien "home" pour le retour à page d'accueil.
- 2 columns dans lequelles contienent des box qui répresentent les principales caractéristiques pour mieux comprendre le sujet (ex : Définition, Caractéristiques, Bonnes Pratiques d'utilisation, tips, etc).
- Un **footer** contenant des liens utiles.

### Utilisation des Schémas, Tables, Images
Des tables, schémas et images sont bienvenus.
_ _Tables__
```html
<table>
  <thead>
      <tr>
        <th>header1</th>
        <th>header2</th>                   
      </tr>
  </thead>
  <tbody>
      <tr>
        <td>row1-content X</td>
        <td>row1-content Y</td>
      </tr>
      <tr>
        <td>row2-content X</td>
        <td>row2-content Y</td>
      </tr>
  </tbody>
</table>
```
_ _Schémas/Images__
```html
<div class="sketch">
  <img  src="../../../ressources\images\scketch.png">
</div>
```

## 🤝 Contribuer
Les contributions sont bienvenues !

Vous pouvez :
- Ajouter des catégories ou sous-catégories.
- Améliorer le design ou le code CSS/HTML.
- Corriger des erreurs ou proposer des idées.

Pour contribuer :
- Forkez ce dépôt
- Créez une branche (git checkout -b nouvelle-fonctionnalite)
- Commitez (git commit -m "Ajout nouvelle catégorie")
- Poussez (git push origin nouvelle-fonctionnalite)
- Créez une Pull Request

Merci pour votre contribution au projet PepITs ! 🙌
