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

| #  | Concepto                     | Descripción                                                   | Ejemplo                                       | Caso de Uso                                   |
|----|------------------------------|---------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------|
| 1  | JSX                          | Sintaxis que permite escribir HTML en JavaScript.             | `<div>Hello, world!</div>`                    | Facilita la creación de UIs en React.         |
| 2  | Componentes                  | Bloques de construcción independientes en React.              | `function Welcome() { return <h1>Hello!</h1> }`| Permiten reutilizar y organizar código.       |
| 3  | Props                        | Propiedades que se pasan a los componentes.                   | `<UserProfile name="John" />`                 | Pasar datos y configuraciones a componentes.  |
| 4  | Estado (State)               | Almacenamiento local mutable en componentes.                  | `useState(0)`                                 | Mantener y gestionar datos dinámicos.         |
| 5  | Eventos                      | Manejo de eventos del usuario.                                | `<button onClick={handleClick}>Click me</button>`| Responder a interacciones del usuario.      |
| 6  | Renderizado Condicional      | Renderizar UIs basadas en condiciones.                       | `{isLoggedIn ? <LogoutButton /> : <LoginButton />}`| Mostrar diferentes UIs basadas en estado.  |
| 7  | Listas y Keys                | Renderizar listas de elementos en React.                     | `<ul>{listItems}</ul>`                         | Mostrar colecciones de datos.                |
| 8  | Componentes Funcionales      | Componentes definidos como funciones.                        | `const Button = () => <button>Click</button>` | Crear componentes sin estado.                |
| 9  | Componentes de Clase         | Componentes definidos como clases ES6.                       | `class Button extends React.Component { ... }` | Crear componentes con métodos de ciclo de vida.|
| 10 | Hooks                        | Funciones que permiten usar estado y otras características en componentes funcionales. | `useState`, `useEffect`                    | Usar características de React sin clases.     |
| 11 | useEffect                    | Hook para manejar efectos secundarios en componentes funcionales. | `useEffect(() => { document.title = name; });` | Ejecutar efectos secundarios en el componente.|
| 12 | useRef                       | Hook para acceder a las referencias DOM en componentes funcionales. | `const myRef = useRef(null);`             | Acceder y manipular nodos DOM directamente.   |
| 13 | Custom Hooks                 | Hooks personalizados creados para reutilizar lógica de estado. | `function useCustomCounter() { ... }`          | Reutilizar lógica de estado entre componentes.|
| 14 | Context API                  | Proporcionar un medio para pasar datos a través del árbol de componentes sin tener que pasar props manualmente a cada nivel. | `React.createContext`                    | Gestionar estados globales como tema o datos de usuario.|
| 15 | Render Props                 | Técnica para compartir código entre componentes usando una prop cuyo valor es una función. | `<DataProvider render={data => (<Component data={data} />)} />`| Reutilizar lógica de renderizado.         |
| 16 | Higher Order Components (HOC)| Componentes que toman otro componente y retornan un nuevo componente mejorado. | `const EnhancedComponent = higherOrderComponent(WrappedComponent);`| Reutilizar lógica de componente.         |
| 17 | Fragmentos                   | Agrupar una lista de hijos sin nodos DOM adicionales.          | `<React.Fragment>{children}</React.Fragment>` | Agrupar elementos sin añadir nodos al DOM.    |
| 18 | Portales                     | Renderizar componentes en un nodo DOM que existe fuera de la jerarquía del DOM de React. | `ReactDOM.createPortal(child, container)` | Manejar UI en diferentes partes del DOM.      |
| 19 | Suspense                     | Suspender la renderización mientras los componentes esperan algo, como datos o scripts. | `<Suspense fallback={<Spinner />}>{component}</Suspense>`| Manejar el estado de carga de componentes.|
| 20 | Lazy Loading                 | Técnica para cargar componentes bajo demanda.                 | `const OtherComponent = React.lazy(() => import('./OtherComponent'));`| Mejorar el rendimiento cargando componentes sólo cuando se necesiten. |
| 21 | Memoización                  | Optimizar el rendimiento memorizando resultados costosos.     | `React.memo(Component)`                        | Prevenir renderizados innecesarios.           |
| 22 | Callbacks                    | Usar funciones que se pasan a otros componentes o hooks para ejecutar acciones. | `useCallback(() => { ... }, [deps]);`         | Evitar recreaciones innecesarias de funciones.|
| 23 | Refs                         | Referencias a elementos DOM o componentes en React.           | `const node = useRef();`                       | Acceso directo a elementos DOM para gestión de enfoque o animaciones. |
| 24 | Lifting State Up             | Técnica para mover el estado a componentes ancestros comunes. | `function handleInputChange(e) { ... }`        | Compartir estado entre componentes hermanos.  |
| 25 | Prop Drilling                | Pasar props a través de múltiples niveles de componentes.     | `<Component prop={data} />`                    | Pasar datos a componentes profundos en el árbol de componentes. |
| 26 | Control de Formularios       | Manejar entradas de formularios con estado de React.          | `<input value={value} onChange={handleChange} />` | Crear formularios controlados con validaciones.|
| 27 | Validación de Props          | Verificar que los props que recibe un componente son válidos. | `UserProfile.propTypes = { name: PropTypes.string };` | Asegurar que los componentes reciban datos correctos. |
| 28 | Children prop                | Acceder a los hijos de un componente desde dentro.            | `function Wrapper({ children }) { return <div>{children}</div>; }` | Composición de componentes.                  |
| 29 | React Router                 | Manejar rutas en aplicaciones web.                            | `<Router><Route path="/" component={Home} /></Router>` | Navegación entre vistas en aplicaciones SPA.|
| 30 | Server-Side Rendering (SSR)  | Generar HTML en el servidor y enviarlo al navegador.          | `ReactDOMServer.renderToString(<App />)`        | Mejorar SEO y tiempo de carga inicial.        |
| 31 | Static Site Generation (SSG) | Generar páginas estáticas en tiempo de compilación.           | Usar Next.js para generar páginas estáticas.    | Optimizar el rendimiento y el SEO.            |
| 32 | Dynamic Import               | Importar módulos de forma dinámica en el código.              | `import('./module.js').then(module => { ... });`| Cargar módulos sólo cuando se necesiten.      |
| 33 | React DevTools               | Herramientas para depurar aplicaciones React.                 | Instalar React DevTools en el navegador.        | Inspeccionar y modificar el estado y props en tiempo de desarrollo. |
| 34 | PropTypes                    | Verificar tipos de props en tiempo de ejecución.              | `Component.propTypes = { name: PropTypes.string.isRequired };` | Asegurar integridad de datos en componentes. |
| 35 | Error Boundaries             | Componentes que capturan errores en la jerarquía de componentes. | `<ErrorBoundary><Component /></ErrorBoundary>`| Gestionar errores de UI para prevenir colapsos completos de la app.|
| 36 | React Patterns               | Patrones comunes para resolver problemas comunes en React.    | Usar patrones como Provider, Container/Presenter. | Establecer soluciones estandarizadas para problemas recurrentes. |
| 37 | Optimización de Rendimiento  | Técnicas para hacer que React funcione más rápido.            | Uso de `React.memo`, `useMemo`.                 | Mejorar la experiencia de usuario reduciendo tiempos de carga y respuesta. |
| 38 | Reconciliation               | Algoritmo de React para sincronizar el DOM con los estados de los componentes. | Entender cómo funciona el diffing de React.    | Optimizar actualizaciones del DOM para mejorar el rendimiento. |
| 39 | Forward Ref                  | Pasar refs a través de componentes.                           | `React.forwardRef((props, ref) => (<div ref={ref} {...props} />));` | Permitir a los componentes hijos interactuar con refs. |
| 40 | Controlled Components        | Componentes que controlan sus propios estados.                | `<input type="text" value={value} onChange={handleInput} />` | Crear formularios con validaciones y control de estado detallado. |
| 41 | Uncontrolled Components      | Componentes que almacenan su propio estado internamente.      | `<input type="text" ref={inputRef} />`          | Simplificar componentes de formulario usando refs. |
| 42 | Webpack                      | Herramienta para compilar JavaScript y recursos asociados.    | Configurar Webpack para bundle de React app.    | Optimizar la carga y el rendimiento de aplicaciones React. |
| 43 | Babel                        | Compilador para escribir JavaScript moderno compatible con navegadores antiguos. | Configurar Babel con presets de React.         | Asegurar que el JSX y ES6+ sean compatibles con todos los navegadores. |
| 44 | Redux                        | Biblioteca para manejar el estado de la aplicación de manera global. | `<Provider store={store}><App /></Provider>` | Gestionar estado complejo en aplicaciones grandes. |
| 45 | Middleware                   | Capa intermedia para manejar acciones antes de que lleguen al reducer en Redux. | Usar `redux-thunk` para acciones asíncronas.   | Permitir lógica asíncrona en la manipulación de estado. |
| 46 | Thunk                        | Funciones que envuelven expresiones para retrasar su ejecución. | Usar `redux-thunk` para aplazar envío de acciones. | Manejar acciones asíncronas en Redux. |
| 47 | Saga                         | Librería para manejar efectos secundarios en aplicaciones Redux. | Usar `redux-saga` para operaciones complejas.  | Organizar y manejar efectos secundarios en aplicaciones React/Redux. |
| 48 | Virtual DOM                  | Representación ligera del DOM que permite a React hacer cambios de manera eficiente. | Entender cómo React actualiza el DOM.          | Permitir que React gestione grandes cantidades de datos de manera eficiente. |
| 49 | Flux                         | Patrón arquitectónico para construir interfaces de usuario coherentes. | Implementar arquitectura Flux en React.        | Mantener datos unidireccionales para consistencia en UI. |
| 50 | React Native                 | Framework para desarrollar aplicaciones móviles nativas usando React. | Crear una app con React Native.                | Desarrollar aplicaciones móviles con habilidades de React. |



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


Concepto | Descripción | Ejemplos | Caso de Uso
-- | -- | -- | --
JSX | Extensión de la sintaxis de JavaScript que permite escribir HTML dentro del código JavaScript. | <div>Hola Mundo</div> | Simplifica la creación de elementos de la interfaz de usuario.
Componentes | Bloques de construcción reutilizables de la interfaz de usuario. | Button, Navbar, Card | Modularizan la UI y facilitan la gestión del código.
Props | Argumentos que se pasan a los componentes para configurarlos. | color="rojo", size="grande" | Permiten personalizar el comportamiento y apariencia de los componentes.
Estado (State) | Datos internos de un componente que pueden cambiar a lo largo del tiempo. | count, isOpen, isLoading | Gestionan la interactividad y la lógica de la aplicación.
Ciclo de Vida | Diferentes etapas por las que pasa un componente, desde su creación hasta su destrucción. | componentDidMount, componentDidUpdate, componentWillUnmount | Permiten ejecutar código en momentos específicos del ciclo de vida del componente.
Hooks | Funciones que permiten usar el estado y otras características de React en componentes funcionales. | useState, useEffect, useContext | Simplifican la gestión del estado y del ciclo de vida en componentes funcionales.
Hooks Personalizados | Funciones que encapsulan lógica reutilizable para compartir entre componentes. | useFetch, useLocalStorage | Extraen lógica común para evitar la repetición de código.
Renderizado Condicional | Mostrar u ocultar elementos de la UI según ciertas condiciones. | if, else, operadores ternarios | Adaptan la interfaz a diferentes estados o datos.
Listas y Keys | Renderizar listas de elementos de manera eficiente. | map, key | Muestran colecciones de datos de forma dinámica.
Eventos | Interacciones del usuario con la interfaz, como clics o pulsaciones de teclas. | onClick, onChange, onSubmit | Permiten reaccionar a las acciones del usuario.
Formularios | Elementos de la UI que permiten recopilar datos del usuario. | input, textarea, select | Capturan información para su posterior procesamiento.
Refs | Permiten acceder directamente a los elementos del DOM. | useRef | Manipulan elementos del DOM de forma imperativa.
React Router | Biblioteca para gestionar la navegación en aplicaciones de una sola página (SPA). | BrowserRouter, Route, Link | Crea rutas y maneja la navegación entre diferentes secciones de la aplicación.
Redux | Biblioteca para la gestión del estado global de la aplicación. | store, actions, reducers | Centraliza el estado y facilita su acceso desde cualquier componente.
Context API | Mecanismo para compartir datos entre componentes sin necesidad de pasar props explícitamente. | createContext, Provider, Consumer | Evita el "prop drilling" al compartir datos globales.
React.memo | Optimiza el rendimiento al evitar renderizados innecesarios de componentes. | React.memo(MyComponent) | Mejora la eficiencia al memorizar el resultado del renderizado.
React.lazy | Carga componentes de forma asíncrona para mejorar el rendimiento inicial. | React.lazy(() => import('./MyComponent')) | Reduce el tamaño del paquete inicial de la aplicación.
Suspense | Permite mostrar contenido de carga mientras se espera que un componente se cargue de forma asíncrona. | <Suspense fallback={<Loading />}> | Mejora la experiencia del usuario al evitar pantallas en blanco durante la carga.
Componentes de Clase | Forma anterior de definir componentes que utilizan clases de JavaScript. | class MyComponent extends React.Component | Permiten usar el estado y el ciclo de vida de una manera más tradicional.
PropTypes | Validación de tipos de las props para asegurar la consistencia del código. | MyComponent.propTypes = { name: PropTypes.string } | Detectan errores en las props durante el desarrollo.
Estilos | Diferentes maneras de aplicar estilos a los componentes de React. | CSS en línea, archivos CSS, CSS-in-JS | Personalizan la apariencia de la interfaz.
React DevTools | Extensión del navegador que facilita la depuración y la inspección de aplicaciones React. | Inspeccionar el árbol de componentes, ver el estado y las props, analizar el rendimiento | Herramienta esencial para el desarrollo con React.
Pruebas | Aseguran la calidad y el correcto funcionamiento de la aplicación. | Jest, React Testing Library | Permiten escribir pruebas unitarias y de integración para los componentes.
Componentes de Orden Superior (HOC) | Funciones que reciben un componente como argumento y devuelven un nuevo componente con funcionalidades añadidas. | withRouter, withStyles | Reutilizan lógica y comportamiento entre componentes.
Render Props | Patrón de diseño que permite compartir lógica entre componentes mediante una función como prop. | <Mouse render={(mouse) => ( /* ... */ )}/> | Proporcionan mayor flexibilidad en la reutilización de la lógica.
Portales | Permiten renderizar un componente en un nodo del DOM que está fuera de la jerarquía del componente padre. | ReactDOM.createPortal | Se utilizan para modales, tooltips y otros elementos que necesitan estar posicionados de forma específica.
Error Boundaries | Componentes que capturan errores de JavaScript en su subárbol y muestran una interfaz de usuario alternativa. | componentDidCatch | Mejoran la experiencia del usuario al evitar que la aplicación se rompa por completo ante errores.
React.StrictMode | Herramienta para identificar posibles problemas en el código de la aplicación. | <React.StrictMode> | Ayuda a detectar código antipatrón y problemas de rendimiento.
Concurrencia (Experimental) | Nuevas características que permiten a React pausar y reanudar el renderizado para mejorar la experiencia del usuario. | startTransition, useDeferredValue | Optimizan el rendimiento y la capacidad de respuesta de la aplicación.
Server-Side Rendering (SSR) | Renderizado de la aplicación en el servidor para mejorar el rendimiento y el SEO. | Next.js, Gatsby | Permiten que el contenido se cargue más rápido y sea indexado por los motores de búsqueda.
Static Site Generation (SSG) | Generación de sitios web estáticos en el momento de la compilación para mejorar el rendimiento y la seguridad. | Next.js, Gatsby | Crea sitios web estáticos que se sirven desde un CDN.
React Native | Framework para construir aplicaciones móviles nativas utilizando React. | Expo, React Native CLI | Permite crear aplicaciones móviles para iOS y Android con el mismo código base.
React 360 | Framework para crear experiencias de realidad virtual con React. | React 360 CLI | Permite desarrollar experiencias inmersivas para la web y dispositivos móviles.
