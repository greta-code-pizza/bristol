[:arrow_backward:](../README.md)

Ce Bristol permet d'avoir un accès rapide aux informations les plus courantes, mais n'est en aucun cas un tour complet de JQuery. Pour aller plus loin n'hésitez pas à faire un tour sur [la documentation de JQuery](https://api.jquery.com/).

# Sommaire

- [JQuery](#jquery)
  - [Guide d'installation](INSTALL.md)
- [Les Sélecteurs](#les-selecteurs)
  - [Basiques](#basiques)
  - [Avancés](#avances)
- [Les filtres](#les-filtres)
- [Les méthodes](#les-methodes)
  - [Manipulation](#manipulation)
  - [Animation](#animation)
  - [Taille et position](#taille-et-position)


## Les Sélecteurs

JQuery vous permet d'utiliser une syntaxe proche de celle de CSS pour sélectionner un élément du DOM.

### Basiques

```js
// En Javascript
document.getElementById('id')
document.querySelectorAll('.class')
document.querySelectorAll('li')

// En JQuery
$('#id') // ou JQuery('#id')
$('.class') // ou JQuery('.class')
$('li') // ou JQuery('li')
```

À noter que par la même occasion, JQuery transforme notre sélecteur en objet JQuery sur lequel on pourra appliquer des méthodes.

### Avancés

```js
// Tous les liens dans l'id #id
$('#id a')

// Limite les liens au enfants direct
$('#id > a')

// Lien ayant le même parent
$('#id ~ a')

// Liens ayant l'attribut spécifié
$("a[href='http://www.google.fr']")
```

## Les filtres

Afin de sélectionner plus facilement un ou plusieurs éléments, vous pouvez utiliser les filtres.

```js
// le premier élément de liste
$('li:first')

// le dernier élément de liste
$('li:last')

// élément avec l'index numéro 2
$('.slide:eq(2)')

// éléments ayant un index supérieur à 2
// gt = greater than
$('.slide:gt(2)')

// éléments ayant un index inférieur à 2
// lt = lower than
$('.slide:lt(2)')

// Le lien contenant "Accueil"
$('a:contains(Accueil)')
```

## Les méthodes