# 03 - Variables en Python

## Introducción

Las variables permiten almacenar información para utilizarla posteriormente dentro de un programa.

En Python, una variable funciona como un contenedor que guarda un valor, el cual puede consultarse, modificarse o reemplazarse durante la ejecución del código.

---

# Objetivos de aprendizaje

Al finalizar este tema podrás:

- Comprender qué es una variable.
- Asignar valores a una variable.
- Reasignar valores a una variable existente.
- Identificar el tipo de dato almacenado en una variable.
- Comprender qué es un **TypeError**.

---

# ¿Qué es una variable?

Una variable es un contenedor que almacena datos.

Cada variable tiene un nombre que permite acceder al valor almacenado.

### Ejemplo

```python
username = "elarson"
```

En este ejemplo:

- `username` es el nombre de la variable.
- `"elarson"` es el valor almacenado.

---

# Asignación de variables

La asignación consiste en almacenar un valor utilizando el operador `=`.

### Ejemplos

```python
username = "bmoreno"

login_attempts = 3

login_status = True
```

Cada variable almacena un tipo de dato diferente.

---

# Reasignación de variables

Una variable puede cambiar de valor durante la ejecución del programa.

Esto se conoce como **reasignación**.

### Ejemplo

```python
login_attempts = 0

login_attempts = login_attempts + 1
```

Después de ejecutar la segunda línea, el valor de `login_attempts` será:

```python
1
```

La variable conserva el mismo nombre, pero ahora almacena un valor diferente.

---

# Variables y tipos de datos

Una variable puede almacenar cualquier tipo de dato.

### Ejemplos

```python
username = "tshah"
```

```python
login_attempts = 5
```

```python
login_status = False
```

```python
risk_score = 8.5
```

---

# Identificar el tipo de una variable

La función `type()` permite conocer el tipo de dato almacenado en una variable.

### Ejemplo

```python
login_attempts = 5

print(type(login_attempts))
```

Salida

```python
<class 'int'>
```

Otro ejemplo

```python
login_status = True

print(type(login_status))
```

Salida

```python
<class 'bool'>
```

---

# Error de tipo (TypeError)

Un **TypeError** ocurre cuando se utiliza un tipo de dato incompatible en una operación.

Este tipo de error indica que Python no puede realizar la operación solicitada debido al tipo de los datos involucrados.

Comprender el tipo de dato almacenado en cada variable ayuda a prevenir este tipo de errores.

---

# Buenas prácticas

Durante el módulo se utilizan nombres de variables que describen claramente la información almacenada.

Ejemplos:

```python
username
```

```python
device_id
```

```python
login_attempts
```

```python
login_status
```

Utilizar nombres descriptivos facilita la lectura y comprensión del código.

---

# Resumen

| Concepto | Descripción |
|----------|-------------|
| Variable | Contenedor que almacena datos. |
| Asignación | Almacenar un valor mediante el operador `=`. |
| Reasignación | Cambiar el valor almacenado en una variable. |
| `type()` | Función que identifica el tipo de dato almacenado. |
| TypeError | Error provocado por utilizar un tipo de dato incorrecto. |

---

# Puntos clave

- Las variables almacenan información para utilizarla posteriormente.
- La asignación se realiza con el operador `=`.
- Una variable puede cambiar de valor mediante una reasignación.
- Una variable puede almacenar distintos tipos de datos.
- La función `type()` permite conocer el tipo de dato almacenado.
- Un **TypeError** indica el uso incorrecto de un tipo de dato.

---

## Siguiente tema

➡️ **[04 - Funciones](04-funciones.md)**

⬅️ **[Volver al índice del módulo](README.md)**
