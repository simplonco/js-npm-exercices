# js-npm-jeux
Apprendre à utiliser npm. Apprendre à choisir et utiliser des librairies

## npm, c'est quoi ?

<svg viewBox="0 0 18 7">
	<path fill="#CB3837" d="M0,0v6h5v1h4v-1h9v-6"></path>
	<path fill="#FFF" d="M1,1v4h2v-3h1v3h1v-4h1v5h2v-4h1v2h-1v1h2v-4h1v4h2v-3h1v3h1v-3h1v3h1v-4"></path>
</svg>

> #### Acronyme de :

> Node Package Manager => **Gestionnaire de package pour Node**

> #### Traduction :

> Il y a des gestionnaires de package pour, à peu près, tous les languages : Gem pour Ruby, Composer pour PHP, etc...

> Node, c'est du javascript : Donc NPM est le gestionnaire de package pour javascript. Et nous allons l'utiliser tous les jours.

> Avec npm, vous allez pouvoir ajouter en une seconde, toutes les librairies dont vous avez besoin.

> Mais pas que...

> #### Plus d'infos :
* [what is npm ? ](https://docs.npmjs.com/getting-started/what-is-npm)
* [openclassrooms](https://openclassrooms.com/courses/des-applications-ultra-rapides-avec-node-js/les-modules-node-js-et-npm])
* [ sitepoint.com](https://www.sitepoint.com/beginners-guide-node-package-manager/)
* [awesome list](https://github.com/sindresorhus/awesome-npm)
* [awesome micro-npm-packages](https://github.com/parro-it/awesome-micro-npm-packages)

## npm, c'est aussi un annuaire

> npm liste tous les packages que les gens ont publiés.

> Il y a des librairies pour tout ou presque...

> Faisons quelques recherche pour tester ça.

> Il faut savoir choisir une librairie :
> * Vous en avez besoin
> * nombre d'étoile sur github
> * dernier commit
> * nombre de version taggées
> * npm trends

> [ex. npm trends 1](http://www.npmtrends.com/react-vs-angular)

> [ex npm trends 2](http://www.npmtrends.com/react-vs-angular-vs-jquery-vs-express-vs-glob-vs-rimraf)

> [ex npm trends 3](http://npmjs.ir/)

> [ex npm trends 4](http://npmsearch.com/)

## npm dans votre terminal

![command line](https://www.npmjs.com/static/images/saas-features/do-more-faster.svg)

#### Quelques commandes essentielles :
* npm list
* npm list -g --depth=0
* npm outdated
* npm config list
* npm install (quand vous forkez ou vous clonez un projet avec un package.json, c'est la premiere chose à faire)
* npm install --save
* npm install --save-dev
* npm install --global

## npm dans votre projet

* créer votre projet sur github OU bitbucket
  * avec un README.md
  * avec un .gitignore => nodejs

* créer votre dossier

    **```git clone https://...```**

* accéder à votre projet sur votre machine

    **```cd votredossier```**


* génèrer un fichier package.json et un dossier node_modules

    **```npm init```**

* installer vos librairies

  **```npm install --save blabla```** ou

  **```npm i -s blabla```** (raccourci)

* les librairies sont installées dans le dossier **node_modules**

## Utiliser les librairies

* avec nodejs

  **```var blabla = require('blabla');```**

* avec un navigateur

  **```<script src="node_modules/blabla/blabla.js"></script>```**

* avec un navigateur et webpack (que nous verrons plus tard)
*
  **```var blabla = require('blabla');```**

## Atom utiles

  https://atom.io/packages/npm

## exercices Browser (à executer dans le navigateur)

But :
Faire une page avec 3 liens vers 3 affichages differents.

Regles :
Utiliser npm.

Les elements à afficher :

1. generateur de nom de super-heros :
  * avec https://github.com/sindresorhus/superheroes (nodejs / browser)
  * Un bouton => superheroes.random() => Affichage d'un nom de superhero en dessous du bouton
  
  
2. generateur de mots dit par un lapin :
  * https://github.com/ryanbahniuk/sign-bunny (nodejs / browser avec un peu de boulot)
  * chalk (pour coloriser vos resultats en **nodejs**)
  * 1 input text + 1 bouton => quand on clique sur le bouton => le lapin affiche le contenu de l'input text
  
  
3. Generateur de camelCase, kebab-case, snake_case (nodejs / browser) avec 
	* https://github.com/ianstormtaylor/to-camel-case
	* https://github.com/joakimbeng/kebab-case
	* https://github.com/ianstormtaylor/to-snake-case
	* https://github.com/ianstormtaylor/to-space-case
	
	* 1 input text + 1 bouton + 4 radio buttons (camel-case, snake-case, kebab-case, space-case)
	* l'utilisateur saisi un texte
	* l'utilisateur clique sur un des 4 boutons radio
	* l'utilisateur sur le bouton
	* => le texte saisi dans l'input text va s'afficher en dessous du bouton sous la forme choisie par l'utilisateur (cf. bouton radios)
	
	
	

## exercice nodejs

https://github.com/simplonco/js-node-project-boilerplate
	
	
4. Générateur de favicon avec https://github.com/haydenbleasel/favicons (nodejs only)
5. generateur de qrcode avec https://github.com/soldair/node-qrcode (nodejs / browser)
6. lecteur de exif avec https://github.com/gomfunkel/node-exif ou https://github.com/hMatoba/piexifjs ou https://github.com/devongovett/exif-reader (nodejs / broser pas sî)
6. lecteur de exif avec https://github.com/gomfunkel/node-exif ou https://github.com/hMatoba/piexifjs ou https://github.com/devongovett/exif-reader (nodejs / browser pas sûr)
6. lecteur de exif avec https://github.com/gomfunkel/node-exif ou https://github.com/hMatoba/piexifjs ou https://github.com/devongovett/exif-reader (nodejs / broser pas s)
