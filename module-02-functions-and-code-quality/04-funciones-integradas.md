# Funciones integradas (Built-in Functions)

## Introducción

Las funciones integradas son funciones que vienen incluidas en Python. No necesitan ser creadas por el programador y pueden utilizarse inmediatamente.

Estas funciones permiten realizar tareas comunes de forma sencilla y eficiente.

En este módulo se estudiaron las siguientes funciones:

- `print()`
- `type()`
- `max()`
- `min()`
- `sorted()`

---

# print()

La función `print()` muestra información en la pantalla.

Es la función más utilizada al comenzar a programar en Python.

## Sintaxis

```python
print(objeto)
```

## Ejemplo

```python
print("Login successful")
```

Salida

```
Login successful
```

También puede imprimir varios elementos separados por comas.

```python
month = "September"

print("Investigate failed login attempts during", month)
```

Salida

```
Investigate failed login attempts during September
```

---

# type()

La función `type()` devuelve el tipo de dato de un objeto.

Es muy útil para verificar qué tipo de información contiene una variable.

## Sintaxis

```python
type(objeto)
```

## Ejemplo

```python
print(type("security"))
```

Salida

```
<class 'str'>
```

Otro ejemplo

```python
print(type(True))
```

Salida

```
<class 'bool'>
```

---

# Pasar una función dentro de otra

Una función puede utilizar el resultado de otra función.

Ejemplo:

```python
print(type("Python"))
```

Python ejecuta primero:

```python
type("Python")
```

y después pasa ese resultado a:

```python
print()
```

---

# max()

Devuelve el valor más grande de una colección de datos.

## Ejemplo

```python
numbers = [12, 2, 32, 19, 57, 22, 14]

print(max(numbers))
```

Salida

```
57
```

### Uso en ciberseguridad

Puede utilizarse para encontrar:

- Mayor cantidad de intentos de inicio de sesión.
- Sesión más larga.
- Archivo más grande.
- Tiempo máximo de respuesta.

---

# min()

Devuelve el valor más pequeño de una colección.

## Ejemplo

```python
numbers = [12, 2, 32, 19, 57, 22, 14]

print(min(numbers))
```

Salida

```
2
```

### Uso en ciberseguridad

Puede utilizarse para encontrar:

- Menor tiempo de conexión.
- Menor número de intentos.
- Sesión más corta.

---

# sorted()

Ordena los elementos de un iterable.

Por defecto, los organiza en orden ascendente.

## Ejemplo

```python
numbers = [12, 2, 32, 19, 57, 22, 14]

print(sorted(numbers))
```

Salida

```
[2, 12, 14, 19, 22, 32, 57]
```

---

## sorted() no modifica la lista original

```python
numbers = [12, 2, 32]

print(sorted(numbers))

print(numbers)
```

Salida

```
[2, 12, 32]

[12, 2, 32]
```

La función devuelve una nueva lista ordenada, pero la lista original permanece igual.

---

## Restricción de sorted()

Todos los elementos deben ser del mismo tipo de dato.

Correcto:

```python
[3, 8, 1]
```

Correcto:

```python
["juan", "pedro", "ana"]
```

Incorrecto:

```python
[1, "juan", True]
```

Python producirá un error porque intenta ordenar distintos tipos de datos.

---

# Aplicación en ciberseguridad

Estas funciones permiten automatizar muchas tareas, por ejemplo:

- Mostrar información durante la ejecución (`print()`).
- Verificar tipos de datos (`type()`).
- Obtener el mayor número de intentos fallidos (`max()`).
- Obtener el menor tiempo de sesión (`min()`).
- Ordenar registros, usuarios o eventos (`sorted()`).

---

# Buenas prácticas

- Utilizar `print()` para depuración y pruebas.
- Utilizar `type()` cuando exista duda sobre el tipo de dato.
- Utilizar `max()` y `min()` para evitar recorrer manualmente listas.
- Utilizar `sorted()` cuando se necesite una copia ordenada sin modificar la lista original.

---

# Conceptos clave

- Función integrada
- `print()`
- `type()`
- `max()`
- `min()`
- `sorted()`
- Tipo de dato
- Lista
- Iterable
- Ordenamiento
