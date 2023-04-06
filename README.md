## Notas

- **JSX** significa **JavaScript Syntax Extension**. Parece JS pero muestra código HTML, es básicamente un lenguaje de template que muestra el HTML pero tiene todas las funciones de JavaScript.

- Una vez compilado el **JavaScript Sintax Extension JSX** todos esos pasan a ser archivos **.JS** con funciones y objetos normales.

- **Reglas al escribir JSX**

- Si una etiqueta HTML tiene apertura es indispensable agregar el cierre.

- Existen algunas que son de solo apertura `<link> <img>` o `<input>` Estas deberán finalizar con />

- Cada componente debe de tener un return

- Debe haber máximo 1 solo elemento en el nivel más alto en ese return. En caso de tener varios, estos deben englobarse en uno solo para que react los pueda procesar. Para evitar que existan muchos divs, en React se puede retornar lo que es un fragment y dejar únicamente   `<> </>`

- Los componentes se van a dividir en dos partes, antes del return y después del return.

- Antes del return: Codigo JS como lo conocemos, funciones, ifs, variaciones

- Después del return: No se deben definir funciones, es lo que se va a ver en pantalla, no se deben poner ifs. Se ponen **expresiones** regularmente.

- Si queremos que lo que está escrito después del return sea tratado como código **js**, debe encerrarse entre corchetes, ej `{1 + 1}`

- Para ejecutar el código se deben utilizar operadores ternarios. No se deben declarar variables. ej: `{edad >= 18 ? 'Eres mayor de edad' : 'No eres mayor de edad' }` - No va a recibir un if.

- Si quiero aplicar un método de Javascript después del return, debo encerrarlo entre las comillas para que funcione, ej. `<h1>{'Hola Mundo'.toLowerCase()}</h1>`

- Si quiero imprimir una variable ej `{edad}`

- Los componentes deben ser nombrados con la primera letra en mayúscula. Tanto el archivo como el nombre del componente.

- Todos los componentes son *funciones*, todos requieren un *return* y todos requieren un *export default*. Para llamar a los componentes desde la app se puede escribir ej `<Header />`

## Formas de escribir código CSS en React

- **CSS Plano** 
- **Framework CSS**, en el HTML es posible poner un enlace hacia un CDN de algún framework de css, tailwind, bootstrap..
- **Módulos de CSS**
- **Componentes**, algunas librerias tienen componentes de React.
- **SASS**
- **Styled Components**

- **Tailwind CSS** Framework popupar por paleta de colores definida, fuentes que se ven muy bien, muy bien documentado.

- El nombre de las clases es parecido al de las propiedades de CSS.

- Las directrices de Tailwind empiezan con @tailwind. Este trabaja con clases. Si queremos añadir estilos a un elemento, le asignamos esa clase de tailwind y el estilo se aplicará al elemento html.


## React Hooks

- Son la base de React. Esta cuenta con una API muy sencilla que nos permite crear todo tipo de aplicaciones por medio de algo llamado hooks. Al final, los hooks también son funciones

- Están disponibles desde la versión 16.8. Antes de esto, era necesario crear clases para crear y modificar el state. Con los Hooks no es necesario.

- Se dividen en **Básicos** y **Adicionales**

- Las categorías más conocidas son: `useState` - Pieza central de react, es el "estado" que es una variable con información relevante en nuestra aplicación de React, algunas veces el state pertenece a un componente en específico o algunas veces deseas compartirlo a lo largo de diferentes componentes. `useEffect` `useContext`

- Es posible crear tus propios Hooks, así es posible separar el código en funciones reutilizables y sacar todo el beneficio de lo que React ofrece.

## React State

- Es básicamente eso, cuál es el estado de nuestra aplicación, en qué se encuentra la app. Ej, si tengo un carrito de compras, ¿tiene o no tiene productos el carrito? si descargué un listado de clientes.. ¿ya llegó o está vacío, qué pasó con esa descarga?

- Es una variable con información relevante en nuestra aplicación de react. **A veces el state pertenece a un componente en específico o se desea compartir a lo largo de diferentes componentes.**

- `ìmport {useState} from "react" const [cliente, setCliente]= useState({});` -> 1. **cliente** es la variable que contiene el valor del estado, 2. **setCliente** es el modificador, es la función que va a modificar la variable cliente, no puede modificar otros estados, únicamente a ese cliente y 3. **useState({})** Tiene las llaves, lo que quiere decir que es el valor inicial. Por lo tanto este cliente inicia como un objeto vacío. El objeto se irá llenando pero ese es su valor inicial. Se pueden tener múltiples useState por componente. `const [total, setTotal] = useState(0);`

