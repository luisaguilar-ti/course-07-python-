# Guía de referencia — Python: conceptos del Módulo 3

## Funciones integradas

### `str()`

Convierte el objeto de entrada en una cadena.

```python
str(10)
```

Convierte el entero `10` en la cadena `"10"`.

### `len()`

Devuelve el número de elementos de un objeto.

```python
print(len("security"))
```

Devuelve y muestra `8`, el número de caracteres de `"security"`.

## Métodos de cadenas

### `.upper()`

Devuelve una copia de la cadena con todas las letras en mayúsculas.

```python
print("Security".upper())
```

### `.lower()`

Devuelve una copia de la cadena con todas las letras en minúsculas.

```python
print("Security".lower())
```

### `.index()`

Encuentra la primera aparición de la entrada en una cadena y devuelve su posición.

```python
print("Security".index("c"))
```

Resultado: `2`.

## Métodos de listas

### `.insert()`

Añade un elemento en una posición específica de la lista.

### `.remove()`

Elimina la primera aparición de un elemento específico.

### `.append()`

Añade una entrada al final de una lista.

### `.index()`

Encuentra la primera aparición de un elemento en una lista y devuelve su índice.

## Sintaxis adicional

### `+` — concatenación

Combina dos cadenas o dos listas.

```python
device_id = "IT" + "nwp12"

users = ["elarson", "bmoreno"] + ["tshah", "btang"]
```

### `[]` — notación entre corchetes

Utiliza índices para extraer partes de una cadena o lista.

```python
print("h32rb17"[0])
print("h32rb17"[0:3])

username_list = ["elarson", "fgarcia", "tshah"]
print(username_list[2])
```

## Expresiones regulares

### `re.findall()`

Devuelve una lista de coincidencias con una expresión regular.

```python
import re

re.findall("a53", "a53-32c .E")
```

### `\w`

Coincide con cualquier carácter alfanumérico y también con `_`.

### `.`

Coincide con todos los caracteres, incluidos símbolos.

### `\d`

Coincide con dígitos individuales.

### `\s`

Coincide con espacios.

### `\.`

Coincide con el carácter punto.

### `+`

Representa una o más ocurrencias de un carácter específico.

### `*`

Representa cero, una o más ocurrencias de un carácter específico.

### `{n}`

Representa un número especificado de ocurrencias.

Ejemplo:

```text
\w{3}
```

Coincide con exactamente tres caracteres alfanuméricos consecutivos.
