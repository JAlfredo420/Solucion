# Solucion
Encontrar la edad mayor y edad menor con su respectivo nombre
---
```
(()=>{
const nombres: string[] = ['Julian', 'Holga', 'Luis', 'Lucio', 'Hector'];
const edad: number[] = [48, 100, 18, 43, 67];

let menorNombre = nombres[0];
let menorEdad = edad[0];

let mayorNombre = nombres[0];
let mayorEdad = edad[0];

const comparar = (edad: number, nombre: string): void => {
  if (edad < menorEdad) {
    menorEdad = edad;
    menorNombre = nombre;
  }
  if (edad > mayorEdad) {
    mayorEdad = edad;
    mayorNombre = nombre;
  }
};

// comparar la edad dada la posicion del array
comparar(edad[0], nombres[0]);
comparar(edad[1], nombres[1]);
comparar(edad[2], nombres[2]);
comparar(edad[3], nombres[3]);
comparar(edad[4], nombres[4]);

console.log(`${menorNombre} es el menor con ${menorEdad} años.`);
console.log(`${mayorNombre} es el mayor con ${mayorEdad} años.`);

})()
```
