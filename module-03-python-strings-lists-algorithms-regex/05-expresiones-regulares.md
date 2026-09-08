# Expresiones regulares

## ¿Qué es una expresión regular?

Una expresión regular (`regex`) es una secuencia de caracteres que forma un patrón.

En Python, las expresiones regulares pueden utilizarse para buscar patrones complejos dentro de cadenas, como:

- Direcciones IP.
- Correos electrónicos.
- ID de dispositivos.
- Información dentro de registros.

## Módulo `re`

Para utilizar expresiones regulares y las funciones relacionadas se importa el módulo `re`:

```python
import re
```

Las expresiones regulares se almacenan en Python como cadenas. Estas cadenas se utilizan con las funciones del módulo `re`.

## `re.findall()`

`re.findall()` devuelve una lista con las coincidencias de una expresión regular.

Recibe dos parámetros:

1. La cadena que contiene el patrón de expresión regular.
2. La cadena en la que se realizará la búsqueda.

Ejemplo:

```python
import re

re.findall("a53", "a53-32c .E")
```

Resultado:

```text
["a53"]
```

## Símbolos para tipos de caracteres

### `\w`

Coincide con cualquier carácter alfanumérico y también con el guión bajo (`_`).

```python
re.findall("\w", "a53-32c .E")
```

Puede encontrar caracteres como letras, números y `_`.

### `\d`

Coincide con dígitos individuales de `0` a `9`.

```python
re.findall("\d", "a53-32c .E")
```

### `\s`

Coincide con caracteres de espacio en blanco, como espacios, tabulaciones y nuevas líneas.

```python
re.findall("\s", "a53-32c .E")
```

### `.`

Coincide con cualquier carácter, incluidos símbolos y espacios, excepto una nueva línea.

```python
re.findall(".", "a53-32c .E")
```

### `\.`

Coincide con el carácter punto literal (`.`).

La barra invertida se utiliza para escapar el significado especial del punto.

```python
re.findall("\.", "a53-32c .E")
```

## Símbolos para cuantificar ocurrencias

Los cuantificadores se colocan después de un carácter o símbolo que identifica el tipo de carácter.

### `+`

Representa una o más ocurrencias consecutivas.

```python
re.findall("\w+", "a53-32c .E")
```

El patrón `\w+` puede encontrar secuencias de uno o más caracteres alfanuméricos.

Por ejemplo:

```text
["a53", "32c", "E"]
```

El símbolo `+` trabaja con una secuencia de caracteres, no solamente con un carácter repetido.

### `*`

Representa cero, una o más ocurrencias.

```python
re.findall("\w*", "a53-32c .E")
```

Al permitir cero ocurrencias, puede producir también cadenas vacías en lugares donde no hay una coincidencia alfanumérica.

### `{n}`

Representa exactamente `n` ocurrencias.

```python
re.findall("\w{3}", "a53-32c .E")
```

El patrón `\w{3}` busca exactamente tres caracteres alfanuméricos consecutivos.

Resultado:

```text
["a53", "32c"]
```

También puede utilizarse con dígitos:

```text
\d{4}
```

Esto representa exactamente cuatro dígitos consecutivos.

### `{m,n}`

Permite especificar un mínimo y un máximo de ocurrencias.

```text
\d{1,3}
```

Coincide con entre uno y tres dígitos consecutivos.

Puede encontrar coincidencias de uno, dos o tres dígitos.

## Cómo Python compara una expresión regular

Python escanea las cadenas de izquierda a derecha.

Cuando encuentra una parte de la cadena que coincide con el primer elemento esperado del patrón, continúa comparando los caracteres siguientes.

Cuando el patrón está completo, comienza nuevamente en el carácter inmediatamente posterior a la coincidencia.

Por ejemplo, en una cadena que contiene `123`, el patrón `\d{2}` coincide con `12` y el proceso continúa desde `3`.

## Construcción de un patrón

Para construir una expresión regular, se divide el patrón buscado en componentes más pequeños y se representan mediante los símbolos disponibles.

Ejemplo de una cadena de registros de empleados:

```python
employee_logins_string = "1001 bmoreno: 12 Marketing 1002 tshah: 7 Human Resources 1003 sgilmore: 5 Finance"
```

La tarea es extraer el nombre de usuario y los intentos de inicio de sesión, sin el número de identificación del empleado ni el departamento.

Los componentes necesarios son:

- Número variable de caracteres del nombre de usuario → `\w+`
- Dos puntos → `:`
- Un espacio → `\s`
- Número variable de dígitos → `\d+`

El patrón se construye combinando esos componentes.

## Probar las expresiones regulares

Las expresiones regulares pueden devolver información innecesaria o excluir información que se desea obtener.

Por eso es útil probar las expresiones regulares antes de utilizarlas.

## Uso en ciberseguridad

Las expresiones regulares permiten buscar patrones en cadenas y registros sin conocer necesariamente los valores exactos.

Por ejemplo, pueden utilizarse para:

- Buscar determinados patrones de direcciones IP.
- Extraer correos electrónicos de registros.
- Buscar identificadores.
- Extraer información estructurada de cadenas.
