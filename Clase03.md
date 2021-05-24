# **TERCERA CLASE 😎**

Tercera Clase de [Coderhood](https://www.coderhood.dev/)

## 1. Hacer una función que reciba un numero y que retorne verdadero si es par o falso en caso contrario.

```
function esPar(numero) {
  if (numero % 2 === 0) {
    return true;
  } else {
    return false;
  }
}

console.log(esPar(2)); //True
console.log(esPar(3)); //False
console.log(esPar(222)); //True
console.log(esPar(333)); //False

```

## 2. Hacer una función que reciba una serie de palabras separadas por espacios y que imprima la misma frase pero en orden inverso.

**Ejemplo 1:**

 > La sentencia sentencia for...of ejecuta un bloque de código para cada elemento de un objeto iterable, como lo son: String, Array,

```

function palabraReversa(cadena) {
  let espacio = " ";
  for (let letra of cadena) {
    espacio = letra + espacio;
  }
  return espacio;
}

console.log(palabraReversa("Hola")); // aloH

```

**Ejemplo 2:**

>texto.split() - separa con un espacio cada caracter "Hola" -> "H","o","l","a".
>texto.reverse() - invierte el orden de cada caracter, el ultimo sera el primero.
>texto.join(") - Juntar todos los caracteres y quitar las comas.


```

function stringInvertido(texto) {
  return texto.split("").reverse().join("");
}

console.log(stringInvertido("Hola que tal JS")); // SJ lat euq aloH 

```


## 3. Hacer una función que reciba como parámetro tres números enteros y que lo ordene de mayor a menor.

```
console.clear();


function obtenerMaxyMin(num1, num2, num3) {
  let numMayor = 0;
  let numMedio = 0;
  let numMenor = 0;
  if (num1 > num2 && num1 > num3) {
    numMayor = num1;
  } else if (num2 > num1 && num2 > num3) {
    numMayor = num2;
  } else if (num3 > num1 && num3 > num2) {
    numMayor = num3;
  }
  if (num1 < num2 && num1 < num3) {
    numMenor = num1;
  } else if (num2 < num1 && num2 < num3) {
    numMenor = num2;
  } else if (num3 < num1 && num3 < num2) {
    numMenor = num3;
  }
  if (
    (numMayor === num2 || numMenor === num2) &&
    (numMayor === num3 || numMenor === num3)
  ) {
    numMedio = num1;
  } else if (
    (numMayor === num1 || numMenor === num1) &&
    (numMayor === num3 || numMenor === num3)
  ) {
    numMedio = num2;
  } else if (
    (numMayor === num1 || numMenor === num1) &&
    (numMayor === num2 || numMenor === num2)
  ) {
    numMedio = num3;
  }
  console.log("Numero menor: ", numMenor);
  console.log("Numero medio: ", numMedio);
  console.log("Numero mayor: ", numMayor);
}

console.log(obtenerMaxyMin(3, 25, 1));

// Numero menor: 1
// Numero medio: 3
// Numero mayor: 25

```

