# Sintaxis y buenas prácticas en Python

## Introducción

Escribir código legible no solo facilita su comprensión, sino que también ayuda a evitar errores. La Guía de estilo PEP 8 proporciona recomendaciones para mejorar la organización del código y mantener una sintaxis correcta.

Esta lectura profundiza en tres aspectos principales:

- Comentarios.
- Indentación.
- Errores comunes de sintaxis.

---

# Comentarios

Un comentario es una nota que los programadores escriben para explicar la intención de su código.

Los comentarios ayudan tanto al autor como a otros programadores a comprender el funcionamiento del programa.

Se recomienda comenzar el código con un comentario que describa qué hace el programa y añadir comentarios adicionales cuando sea necesario para explicar secciones específicas.

---

## Comentarios de una línea

Los comentarios de una línea comienzan con el símbolo `#`.

Ejemplo:

```python
# Print elements of 'computer_assets' list

computer_assets = ["laptop1", "desktop20", "smartphone03"]

for asset in computer_assets:
    print(asset)
```

Según la guía PEP 8, es una buena práctica que las líneas no superen los **79 caracteres**, incluidos los comentarios.

El curso señala que los comentarios son especialmente útiles cuando el código contiene funciones, múltiples bucles o sentencias condicionales. En código muy sencillo, como una reasignación de variables, son opcionales.

---

## Comentarios multilínea

Cuando un comentario necesita más de una línea, existen dos formas comunes de escribirlo.

### Utilizando varias líneas con `#`

```python
# remaining_login_attempts() function takes two integer parameters,
# the maximum login attempts allowed and the total attempts made,
# and it returns an integer representing remaining login attempts
```

### Utilizando docstrings

Las **docstrings** son cadenas escritas entre comillas triples (`""" """`) que se utilizan para documentar código.

Ejemplo:

```python
"""
remaining_login_attempts() function takes two integer parameters,
the maximum login attempts allowed and the total attempts made,
and it returns an integer representing remaining login attempts
"""
```

---

# Indentación

La indentación es el espacio que se agrega al inicio de una línea de código.

En Python debe utilizarse en:

- Definiciones de funciones.
- Sentencias condicionales.
- Sentencias iterativas.

La indentación permite que Python interprete correctamente los bloques de código y también mejora su legibilidad.

PEP 8 recomienda utilizar **cuatro espacios** por cada nivel de indentación.

Cuando existen bloques dentro de otros bloques, la indentación aumenta un nivel adicional.

Ejemplo:

```python
count = 0
login_status = True

while login_status == True:
    print("Try again.")
    count = count + 1

    if count == 4:
        login_status = False
```

En este ejemplo:

- El cuerpo del `while` tiene una indentación de cuatro espacios.
- El cuerpo del `if`, que está dentro del `while`, tiene una indentación adicional.

---

# Mantener una sintaxis correcta

Los errores de sintaxis ocurren cuando el código no sigue las reglas del lenguaje Python.

Son uno de los errores más comunes al programar y normalmente impiden que el programa se ejecute.

El curso destaca dos fuentes frecuentes de errores:

- Tipos de datos.
- Encabezados de funciones, condicionales y bucles.

---

# Tipos de datos

Cada tipo de dato tiene una sintaxis específica.

## Cadenas

Las cadenas deben escribirse entre comillas.

```python
username = "bmoreno"
```

---

## Enteros, flotantes y booleanos

Estos tipos de datos **no** deben escribirse entre comillas.

Ejemplos:

```python
login_attempts = 5

percentage_successful = 0.8

login_status = True
```

---

## Listas

Las listas se escriben entre corchetes (`[]`) y sus elementos se separan mediante comas.

Ejemplo:

```python
username_list = ["bmoreno", "tshah"]
```

---

# Dos puntos en los encabezados

Las definiciones de funciones, las sentencias condicionales y las sentencias iterativas deben terminar con dos puntos (`:`).

Ejemplo:

```python
def remaining_login_attempts(maximum_attempts, total_attempts):
    return maximum_attempts - total_attempts
```

Si se omiten los dos puntos, Python genera un error de sintaxis.

---

# Ideas principales

- Los comentarios ayudan a explicar la intención del código.
- Los comentarios pueden ser de una línea o multilínea.
- Las docstrings se utilizan para documentar código mediante comillas triples.
- La indentación mejora la legibilidad y es necesaria para que Python interprete correctamente los bloques de código.
- PEP 8 recomienda utilizar cuatro espacios por nivel de indentación.
- Los errores de sintaxis suelen estar relacionados con los tipos de datos y con la estructura de funciones, condicionales y bucles.

---

# Conceptos clave

- Comentario
- Comentario de una línea
- Comentario multilínea
- Docstring
- Indentación
- Sintaxis
- Error de sintaxis
- PEP 8
