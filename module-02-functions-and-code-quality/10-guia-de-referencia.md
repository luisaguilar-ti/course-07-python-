# Guía de referencia - Conceptos de Python (Módulo 2)

## Definición de funciones

```python
def nombre_funcion():
    print("Hola")
```

Define una función llamada `nombre_funcion`.

---

## Llamar una función

```python
nombre_funcion()
```

Ejecuta la función previamente definida.

---

## Parámetros

Los parámetros son variables que se declaran en la definición de una función.

```python
def greet_employee(name):
    print("Welcome", name)
```

`name` es un parámetro.

---

## Argumentos

Los argumentos son los datos que se envían cuando se llama a una función.

```python
greet_employee("Luis")
```

`"Luis"` es el argumento.

---

## Sentencia `return`

Devuelve información desde una función.

```python
def remaining_attempts(maximum_attempts, total_attempts):
    return maximum_attempts - total_attempts
```

---

## Almacenar el valor devuelto

```python
remaining = remaining_attempts(5, 2)

print(remaining)
```

Permite utilizar posteriormente el resultado de una función.

---

# Variables globales

Se crean fuera de las funciones y pueden utilizarse en cualquier parte del programa.

```python
username = "elarson"
```

---

# Variables locales

Se crean dentro de una función y solo existen mientras la función se ejecuta.

```python
def greet():
    message = "Welcome"
```

`message` es una variable local.

---

# Funciones integradas

## print()

Muestra información en pantalla.

```python
print("Login successful")
```

---

## type()

Devuelve el tipo de dato.

```python
print(type(True))
```

---

## max()

Devuelve el valor mayor.

```python
numbers = [5, 9, 2]

print(max(numbers))
```

---

## min()

Devuelve el valor menor.

```python
numbers = [5, 9, 2]

print(min(numbers))
```

---

## sorted()

Ordena un iterable en orden ascendente.

```python
numbers = [5, 9, 2]

print(sorted(numbers))
```

---

# Importar módulos

## Importar un módulo completo

```python
import statistics
```

Llamar una función:

```python
statistics.mean(numbers)
```

---

## Importar funciones específicas

```python
from statistics import mean, median
```

Uso:

```python
mean(numbers)

median(numbers)
```

---

# Módulos vistos en el curso

| Módulo | Uso |
|---------|-----|
| `statistics` | Media y mediana |
| `re` | Expresiones regulares |
| `csv` | Archivos CSV |
| `os` | Sistema operativo |
| `glob` | Buscar archivos |
| `time` | Tiempo |
| `datetime` | Fechas y horas |

---

# Bibliotecas externas mencionadas

| Biblioteca | Uso |
|------------|-----|
| Beautiful Soup (`bs4`) | Analizar HTML |
| NumPy (`numpy`) | Matemáticas y matrices |

---

# Instalar una biblioteca

```python
%pip install numpy
```

---

# Comentarios

## Una línea

```python
# Este es un comentario
```

## Multilínea (docstring)

```python
"""
Comentario
de varias
líneas
"""
```

---

# Indentación

PEP 8 recomienda utilizar **4 espacios** por cada nivel de indentación.

Ejemplo:

```python
if login_success:
    print("Access granted")
```

---

# PEP 8

La guía de estilo PEP 8 recomienda escribir código:

- Claro.
- Consistente.
- Fácil de leer.
- Fácil de mantener.

---

# Recordatorios

- Definir una función **no la ejecuta**.
- Una función se ejecuta únicamente cuando es llamada.
- Los parámetros se definen.
- Los argumentos se envían.
- `return` devuelve información.
- Las variables locales solo existen dentro de la función.
- Las variables globales pueden utilizarse en todo el programa.
- `import` importa módulos completos.
- `from ... import ...` importa funciones específicas.
