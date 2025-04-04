# js-arreglos-bucles

## RETO1 
```javascript
function sumaElementos(arreglo) {
  return arreglo.reduce((acc, num) => acc + num, 0);
}
```

## RETO2
```javascript
function numeroMayor(arreglo) {
  return Math.max(...arreglo);
}
```

## RETO3
```javascript
function filtrarPares(arreglo) {
  return arreglo.filter(num => num % 2 === 0);
}
```

## RETO04
```javascript
function contarVocales(palabra) {
  const vocales = 'aeiouAEIOU';
  return [...palabra].filter(letra => vocales.includes(letra)).length;
}
```

## RETO5
```javascript
function invertirArreglo(arreglo) {
  let resultado = [];
  for (let i = arreglo.length - 1; i >= 0; i--) {
    resultado.push(arreglo[i]);
  }
  return resultado;
}
```

## RETO6
```javascript
function promedioNotas(arreglo) {
  const suma = arreglo.reduce((acc, nota) => acc + nota, 0);
  return suma / arreglo.length;
}
```

## RETO7
```javascript
function contarLetras(palabra, letra) {
  return [...palabra].filter(caracter => caracter === letra).length;
}
```

## RETO08
```javascript
function elementosUnicos(arreglo) {
  return [...new Set(arreglo)];
}
```

## RETO9
```javascript
function esPalindromo(palabra) {
  const palabraInvertida = palabra.split('').reverse().join('');
  return palabra === palabraInvertida;
}
```

## CHALLENGE
```javascript
function adivinaElNumero() {
  const numeroAleatorio = Math.floor(Math.random() * 100) + 1;
  let intentos = 0;
  let adivinanza;
  
  while (adivinanza !== numeroAleatorio) {
    adivinanza = parseInt(prompt("Adivina el número entre 1 y 100:"));
    intentos++;
    
    if (adivinanza > numeroAleatorio) {
      alert("El número es menor.");
    } else if (adivinanza < numeroAleatorio) {
      alert("El número es mayor.");
    } else {
      alert(`¡Adivinaste! El número era ${numeroAleatorio}. Intentos: ${intentos}`);
    }
  }
}
```
