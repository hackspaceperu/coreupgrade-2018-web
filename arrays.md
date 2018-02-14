# Arrays y Objetos

En esta primera parte vamos a hablar un poco de los arreglos, objetos en javascript y luego pasaremos al uso del módulo yargs.

Un array es una colección de valores, donde cada valor tiene una posición dentro del array:

<p align="center">
<img src="https://www.javatpoint.com/images/core/array.gif">
</p>

Para crear un array podemos hacer:

```javascript
var arrayVacio = [];
var nrosPrimos = [2, 3, 5, 7, 11];

// Tambien pueden ser de diferentes tipos:
var mixedArray = [ 3.14, false, "Hackspace"];
// O un array de objetos
var alumnos = [
    {
        nombre: "Edward",
        apellido: "Elric",
        edad: 15
    },
    {
        nombre: "Riza",
        apellido: "Hawkeye",
        edad: 21
    },
    {
        nombre: "Roy",
        apellido: "Mustang",
        edad: 25
    }
]
```

Podemos extraer elementos de los arrays mediante el uso de sus índices, tambien podemos modificar los mismos:

```javascript

// Extraemos el segundo elemento
var alumna = alumnos[1];
console.log(alumna)
// {
//    nombre: "Riza",
//    apellido: "Hawkeye",
//    edad: 21
//}

// Modificamos el primer elemento del array

mixedArray[0] = { message: "Tuturuu" };
console.log(mixedArray);
// [ {message: "Tuturuu"} , false, "Hackspace"]

```

Los arrays poseen multiples métodos útiles como:

### Length
Nos devuelve el tamaño del array

```javascript
var sizeArray = alumnos.length // 3
```
### Push()
Añadimos un elemento al final del array

```javascript
mixedArray.push("CoreUpgrade2018");
console.log(mixedArray);
// [ {message: "Tuturuu"} , false, "Hackspace", "CoreUpgrade2018"]
```

### Pop()
Extraemos un elemento del final del array

```javascript
var element = mixedArray.pop();
console.log(element);
// "Coreupgrade"
```

### Slice()
Nos permite dividir un arreglo donde el primer elemento es el índice inicial y el segundo el indice final.

```javascript
var arr = ["I", "don't", "know", "anything"];
console.log(arr.slice(1,3)); // Se detiene en ultimo-1
// ["don't", "know"]
```

## Find()

Podemos realizar una busqueda en un arreglo haciendo uso del método `find()`;
```javascript
var users = [
  {id: 5123, name: "Josh"},
  {id: 1512, name: "Juliana"},
  {id: 1523, name: "Patricia"}
];

var result = users.find( function (user) {
        return user.id == 1512;
    }
);

console.log(result.name); // Juliana
```

## Recorriendo arrays

Podemos hacer uso de for para recorrer los elementos de un array
```javascript
var langs = ["C", "Python", "Javascript"];

for (var i = 0; i < langs.length; i++) {
    console.log(langs[i]);
}
// Tambien de este modo
for (var key in langs) {
    console.log(langs[key]);
}

// Nos da como resultado
// C
// Python
// Javascript
```

## Métodos especiales

En esta parte vamos a usar unos métodos especiales que nos facilitan mucho el manejo de arrays en javascript.

### Método filter

El método `filter()` crea un nuevo array con todos los elementos que pasan la prueba implementada por la función proporcionada.

En este ejemplo tenemos un array de animes y sus fechas de emisión y queremos filtrar a aquellos que se hayan estrenado luego del 2010:

```javascript
var animes = [
  {name: 'One Piece', year: 1999},
  {name: 'Samurai Champloo', year: 2004},
  {name: 'Steins Gate', year: 2011},
  {name: 'Fullmetal Alchemist: Brotherhood', year: 2009},
  {name: 'Hyouka', year: 2012},
];

// A filter le pasamos una función que filtre nuestra búsqueda
var animesFrom2010 = animes.filter( function( anime ){
    return anime.year > 2010;
});

console.log(animesFrom2010);
/*
[
    {name: 'Steins Gate', year: 2011},
    {name: 'Hyouka', year: 2012}
]
*/
```

### Método map

El método `map()` crea un nuevo array con los resultados de llamar a una función.


```javascript
var nombres = ["Juan", "Carlos", "Maria"];

// A map le pasamos una función que
// añadirá la cadena gonzales a los nombres
var familiaGonzales = nombres.map( function( nombre ){
    return nombre + " Gonzales";
});

console.log(familiaGonzales);
// ["Juan Gonzales", "Carlos Gonzales", "Maria Gonzales"]
```

### Método reduce

El método `reduce()` aplica una función a un acumulador y a cada valor de un array (de izquierda a derecha) para reducirlo a un único valor.

En este ejemplo vamos a sumar los elementos de un array

```javascript
var numbers = [12 , 21 , 32 , 81];

var resultado = numbers.reduce( function suma (acum, actual){
    return acum + actual;
});

console.log(resultado); // 146
```

En resumen estas 3 funciones hacen lo siguiente :D

<p align="center">
<img src="https://steemitimages.com/DQmc4oH8CBMuYwZZxvh8qQRkpNAMgxnS8vs3LT9QNXHh1Yn/image.png">
</p>

