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