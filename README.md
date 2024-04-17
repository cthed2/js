# Pildoras

Java -> Proposito general
JavaScript -> Proposito concreto, el cual es ejecutarse en un navegador. Orientado a la web.

## Javascript

    - Se ejecuta en local (no cuenta con servidor)
    - Es interpretado
    - Respuesta innmediata
    - Agrega interactividad a los sitios web
    - Proporciona efectos visuales dinámicos

## JQuery

Librería de JS, open source.
    - Puedes obtener un efecto vistoso de JQuery.
    - Permite agregar funcionalidades avanzadas

## ¿Como lo agregamos ?

Puede ir dentro del codigo html o también en archivos externos archivo.js

## Sintaxis

Las funciones tiene siempre un parentesis:
    - alert();

### Tipos de datos

    - Numeros: 50
    - Strings: "abc" | 'abc'
    - Boleans: TRUE - FALSE


### Variables
Espacio en la memoria del ordenador (RAM), podemos almacenar datos.

    - var puntuacion; -> DECLARAS
    - puntuacion=0; -> Asginas

### Concatenar variables

    - alert("El importe total es: " + total + "Euros");
    - camisetas="5";
    - total=Number(camisetas) + 5;

### Operadores incremento-decremento
    - +=  (Record+=10)    10+10: 20
    - -=  (Record-=7)     10-7: 3 
    - *=
    - /=
    - ++ Incrementa en 1 el valor de la variable
    - -- Decrementa en 1 el valor de una variable
### Prompt

Para entrada de datos, a diferencia de alert que es la salida de datos.
    - var nombre = prompt("Cual es tu nombres: ");


### Arrays | Arreglos Matrices

Puedes almacenar varias variables. Como una lista.
    - var aticulos=new Array("abc", "xyz", "123");
    - var articulos["zapatillas", "pantalon", "abc"];
    - posición [0], [1],[2]
    - alet(articulos[1])

### Propiedades de Arrays
    - articulos.length=4;
    


### Metodos de Arrays
    - Push, agrega la final - articulos.push("balon")
    - unshift agrega al inicio - artuculos.unshift("balon")
    - pop - elimina el ultimo
    - shift - elimina el primero


### P.O.O.

 Caracteristicas(**Tener**) + Capacidades(**poder hacer**)

 Un objeto puede ser un boton. 

 Nomenclatura del PUNTO
```
 NOMBRE_COCHE.COLOR="AZUL";
 NOMBRE_COCHE.ANCHO="2000";

 NOMBRE_COCHE.ACELERA();  // Con parentesis se dice la acción lo que puede hacer.
```
 Ejemplo Boton:

```
 boton.style.width="500px";
```

### Control de Flujo
```
if(condicion && condition){

}

else if(condicion && condition){

}
else{

}

parseInt(var_string) -> numeric
```

### Bucle Do - while
```
Do{

}while(condicion){

}
```
### For
```
for(var i=o; i < 10; i++){

}
```
### Funciones
Crea:
```
function nombre_funcion(){
    // Codigo a ejecutar
}
```
Ejecuta:
```
nombre_funcion()
```
Con Parametros:
```
function nombre_funcion(a,b,c){

}
```
### Introducción a Eventos
Eventos más funciones, optinen su máxima potencialidad.

Eventos: Desencadenantes de la accción. Permite interactuar con la pagina web.

Eventos: onblur, onchange, onclick, ondblclick, onfocus, onkeydown, onkeypress, onkeyup
onload, onmousedown, onmousemove, onmouseout, onmouseover, onmouseup, onreset, onresize


Ejemplo:
```
function aviso(){
    alert("aviso...");
}

<img src= "..." onClick="aviso()">
```
Dentro de la etiqueta de la imagen agrego el evneto onclick.



### JQuery

Librería que nos ayuda en la creación de tareas frecuentes ala hora de programar.

Estoy en el 68 js


### Ajax
Asincrono
JAvascript
Xml

Esta tecnologia dota del comportamiento tipico de una aplicacion de escritorio.

Puedes hacer varias peticiones en paralelo al servidor.

Enviar petición por XMLHttpRequest:
```
var mi_var=new XLMHttpRequest();
```
Se comunica al servidor mediante peticiones tipo ulr, con los parametros indicados, luego el servidor lanza un respuesta y el cliente en este caso js modifica el DOM, en especifico que parte del DOM será modificado con la informaciónq ue envio el servidor.

La respuesta viene en formato: xml, json, etc.

#

# Cosas de Js para React

## ChatGPT

Por supuesto, aquí tienes la información organizada en una tabla de Markdown, incluyendo los conceptos de JavaScript necesarios para React y algunos ejemplos prácticos o casos de uso:

| Concepto                        | Descripción y Caso de Uso                                                                                                                                                                             |
|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ES6 y más allá**              | - **Let y Const**: Usar `let` en bucles para limitar el alcance de una variable. Usar `const` para declarar constantes.<br>- **Arrow Functions**: Simplificar la sintaxis y manejar el contexto de `this` en componentes funcionales de React.<br>- **Template Literals**: Crear strings de HTML o direcciones URL dinámicas más legibles.<br>- **Destructuring**: Extraer propiedades de objetos props en componentes React de forma más limpia.<br>- **Import/Export**: Organizar el código en módulos, importar y exportar componentes o utilidades. |
| **Programación Asincrónica**    | - **Promesas y Async/Await**: Gestionar llamadas a APIs, como obtener datos de un servidor en componentes React.                                                                                       |
| **Manejo de Errores**           | - **Try/Catch**: Usar en funciones asincrónicas para capturar errores que podrían surgir durante las llamadas a APIs.                                                                                 |
| **Funciones de Orden Superior** | - Usar funciones como `.map()` para renderizar listas de componentes en React.                                                                                                                         |
| **Callbacks y Promesas**        | - **Callbacks**: Usar en métodos `.then()` de promesas para manejar respuestas asincrónicas.<br>- **Promesas**: Usar para manejar la asincronía más limpiamente con `.then()` y `.catch()`.            |
| **Programación Funcional**      | - **Map, Reduce, Filter**: Usar `map` para transformar arrays de datos en elementos JSX en React.<br>- **Funciones Puras**: Crear funciones que no modifiquen el estado externo para evitar side effects en React.  |
| **Manejo de Estado y Efectos**  | - **Closures y Hooks (useState, useEffect)**: Utilizar `useState` para manejar el estado local en un componente, `useEffect` para manejar efectos secundarios como subscripciones o fetch de datos.     |
| **Manejo de Eventos**           | - Entender y utilizar la propagación de eventos (bubbling y capturing) para manejar eventos en componentes de forma eficiente.                                                                         |
| **Prototipos y Herencia**       | - Comprender cómo se utilizan los prototipos para implementar técnicas de herencia en JavaScript, aunque en React se prefiere la composición sobre la herencia.                                         |
| **ESLint y Formato de Código**  | - Utilizar ESLint para asegurar que el código siga las buenas prácticas y estándares, especialmente útil en equipos grandes.                                                                           |
| **Immutable Data**              | - Uso de estructuras de datos inmutables para gestionar el estado en Redux, ayudando a prevenir mutaciones no deseadas y facilitar el seguimiento de cambios.                                           |
| **Testing de JavaScript**       | - Usar Jest para escribir pruebas unitarias para componentes React, asegurando que cada componente funcione correctamente de forma aislada.                                                            |

Esta tabla proporciona una visión clara de los conceptos intermedios y avanzados de JavaScript que son fundamentales para entender y trabajar eficientemente con React. Estos fundamentos son esenciales para manejar el estado, los efectos secundarios, y la estructura del proyecto en aplicaciones React.

## Gemini 1.5

| Concepto                        | Descripción                                                                                                                | Ejemplo                                                                                                   | Importancia en React                                                                                   |
|---------------------------------|----------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|
| **Programación Funcional**      | Enfoque que enfatiza funciones puras, inmutabilidad y funciones de orden superior para construir software.                 | `const sumar = (a, b) => a + b;`                                                                          | Fundamental para la gestión del estado y la composición de componentes en React.                       |
| **Funciones Puras**             | Funciones que, dados los mismos argumentos, siempre devuelven el mismo resultado y no tienen efectos secundarios.          | `const cuadrado = x => x * x;`                                                                            | Facilitan el razonamiento sobre el código y las pruebas.                                                |
| **Inmutabilidad**               | El estado del programa no se modifica directamente, sino que se crean nuevas versiones con los cambios.                    | `const nuevoArreglo = [...arreglo, elemento];`                                                            | Ayuda a mantener la previsibilidad del código y facilita la depuración.                                |
| **Funciones de Orden Superior** | Funciones que toman otras funciones como argumentos o las devuelven.                                                       | `arreglo.map(x => x * 2);`                                                                                | Permiten abstraer la lógica y escribir código más conciso y reutilizable.                              |
| **Closures**                    | Funciones que "recuerdan" el entorno léxico en el que fueron creadas, incluso después de que la función externa haya terminado de ejecutarse. | `function crearContador() { let contador = 0; return () => contador++; }` | Útiles para encapsular el estado y crear componentes con estado en React.                              |
| **Currying**                    | Técnica para transformar una función que toma múltiples argumentos en una secuencia de funciones que toman un solo argumento. | `const sumar = a => b => a + b; const sumar5 = sumar(5); sumar5(3); // 8`                                  | Puede simplificar la composición de funciones y mejorar la legibilidad del código.                     |
| **Manejo de this**              | `this` se refiere al objeto que llama a la función actual, pero su comportamiento puede ser complejo.                        | Usar `bind`, funciones flecha o clases para controlar el contexto de `this`.                              | Importante para trabajar con eventos y métodos de ciclo de vida en componentes React.                   |
| **Prototipos y Herencia**       | Mecanismos para crear objetos que heredan propiedades y métodos de otros objetos.                                           | `function Persona(nombre) { this.nombre = nombre; } Persona.prototype.saludar = function() { console.log(\`Hola, soy ${this.nombre}\`); }` | Conocerlos ayuda a entender la estructura de clases y componentes en React.                            |
| **Expresiones Regulares**       | Patrones que se utilizan para buscar y manipular cadenas de texto.                                                         | `const regex = /^[a-z]+$/i;`                                                                              | Útiles para la validación de formularios y el procesamiento de datos de texto.                         |
| **Promesas**                    | Objetos que representan el resultado eventual de una operación asíncrona.                                                  | `fetch('https://api.example.com/data').then(response => response.json()).then(data => console.log(data)).catch(error => console.error(error));` | Esenciales para trabajar con APIs y realizar operaciones asíncronas en React.                          |
| **Async/Await**                 | Sintaxis que simplifica el trabajo con promesas.                                                                           | `async function obtenerDatos() { const response = await fetch('https://api.example.com/data'); const data = await response.json(); console.log(data); }` | Permite escribir código asíncrono de forma más legible y estructurada.                                 |
| **Módulos (ES Modules)**        | Sistema para organizar y compartir código JavaScript.                                                                      | `import { Component } from 'react';`                                                                      | Fundamentales para estructurar aplicaciones React y reutilizar código.                                 |
| **Gestión de Paquetes (npm/yarn)** | Herramientas para instalar y administrar dependencias de terceros.                                                         | `npm install react react-dom`                                                                             | Necesarias para incorporar bibliotecas y frameworks a tu proyecto React.                               |
