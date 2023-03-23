## Notas

- **JSX** significa **JavaScript Syntax Extension**. Parece JS pero muestra código HTML, es básicamente un lenguaje de template que muestra el HTML pero tiene todas las funciones de JavaScript.

- Una vez compilado el **JavaScript Sintax Extension JSX** todos esos pasan a ser archivos **.JS** con funciones y objetos normales.

- **Reglas al escribir JSX**

-- Si una etiqueta HTML tiene apertura es indispensable agregar el cierre.
-- Existen algunas que son de solo apertura ´<link>´ ´<img>´ o ´<input>´ Estas deberán finalizar con />
-- Cada componente debe de tener un return
-- Debe haber máximo 1 solo elemento en el nivel más alto en ese return. En caso de tener varios, estos deben englobarse en uno solo para que react los pueda procesar. Para evitar que existan muchos divs, en React se puede retornar lo que es un fragment y dejar únicamente   ´<> y </>.´