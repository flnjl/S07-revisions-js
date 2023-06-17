# Révisions JS

## Variables

### Déclaration

Créer les variables suivantes :

- `nombrePages` qui contient la valeur `354`
- `titre` qui contient la valeur `JavaScript pour les Nuls`
- `prix` qui contient la valeur `24.95`
- `formatNumerique` qui contient la valeur `faux`

Correction

```js
let nombrePages = 354;
let titre = "JavaScript pour les Nuls";
let prix = 24.95;
let formatNumerique = false;
```

Quels sont les types de chaque variable ?

Correction :

- number
- string
- number
- boolean

### Opérations

Sur les variables précédentes :

- incrémenter `nombrePages`
- décrémenter `nombrePages`
- inverser la valeur de `formatNumerique`
- créer une chaîne de caractères `infosLivre` qui contient `Le livre "JavaScript pour les Nuls" contient 354 pages, au prix de 24.95 €. Existe au format numérique : vrai`.

Correction

```js

nombrePages++;
nombrePages--;
formatNumerique = !formatNumerique;
let infosLivre = 'Le livre "' + titre + '" contient ' + nombrePages + ' pages, au prix de ' + prix + ' €. Existe au format numérique : vrai';
```

### Tableaux

- Stocker les informations (dans l'ordre de création des variables) dans un tableau indexé
- Créer une chaine de caractères `infosLivre2` qui contient la même valeur que `infoLivre` mais à partir du tableau
- Afficher la longueur du tableau

- Stocker les informations (dans l'ordre de création des variables) dans un tableau associatif (en clé le nom de la variable)
- Créer une chaine de caractères `infosLivre3` qui contient la même valeur que `infoLivre` mais à partir du tableau


### Constante

- Comment déclare-t-on une constante ?
- Peut-on modifier une constante ?

### Divers

```js

let x = 1;
let y = "2";
let z = x + y; // que vaut z, quel est son type ?

// comment inverser les valeurs de x et y ?
z = x;
x = y;
y = z;

// est-ce que 42 est divisible par 3 ?
console.log(42 % 3 === 0);

// est-ce que 306 est divisble par 3 ?
console.log(306 % 3 === 0);

```

## Conditionnelles

### min

Déclarer deux variables :

- `a` qui contient 56
- `b` qui contient 27

Écrire une condition qui affiche "a plus grand que b" si `a` est plus grand que `b` et qui affiche "b plus grand que a" dans le cas inverse.

Correction

```js
let a = 56;
let b = 27;

if (a > b) {
  console.log("a plus grand que b");
} else {
  console.log("b plus grand que a");
}
```

Modifier la condition pour afficher "a et b sont égaux" s'ils sont égaux.

```js
let a = 56;
let b = 27;

if (a > b) {
  console.log("a plus grand que b");
} else if (a < b)
  console.log("b plus grand que a");
} else {
  console.log("a et b sont égaux");
}
```

Modifier le code pour tirer `a` et `b` de façon aléatoire et faire plusieurs essais :

```js
let a = Math.floor(Math.random() * 150);
let b = Math.floor(Math.random() * 150);
```

