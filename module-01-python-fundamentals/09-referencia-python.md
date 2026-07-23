# 09 - Guía de referencia de Python

## Introducción

Esta guía reúne la sintaxis y las estructuras principales presentadas durante el Módulo 1. Está diseñada como material de consulta rápida para recordar la forma correcta de utilizar comentarios, funciones, sentencias condicionales y bucles.

---

# Comentarios

Los comentarios permiten añadir notas dentro del código para explicar su propósito. Python ignora estas líneas durante la ejecución.

## Sintaxis

```python
# Este es un comentario
```

## Ejemplo

```python
# Print approved usernames
```

---

# Funciones

## `print()`

Muestra información en la pantalla.

### Sintaxis

```python
print(objeto)
```

### Ejemplos

```python
print("Login success")
```

```python
print(9 < 7)
```

---

## `type()`

Devuelve el tipo de dato de un valor o una variable.

### Sintaxis

```python
type(objeto)
```

### Ejemplos

```python
print(type(51.1))
```

```python
print(type(True))
```

---

## `range()`

Genera una secuencia de números.

### Sintaxis completa

```python
range(inicio, fin, incremento)
```

### Ejemplo

```python
range(0, 5, 1)
```

Genera:

```text
0
1
2
3
4
```

### Forma abreviada

```python
range(5)
```

---

# Sentencias condicionales

## `if`

Inicia una condición.

```python
if device_id != "la858zn":
    print("Unknown device")
```

---

## `elif`

Evalúa una condición adicional cuando la anterior fue falsa.

```python
if status == 200:
    print("Success")
elif status == 500:
    print("Server error")
```

---

## `else`

Se ejecuta cuando ninguna condición anterior es verdadera.

```python
if login_status:
    print("Access granted")
else:
    print("Access denied")
```

---

# Operadores de comparación

| Operador | Significado |
|----------|-------------|
| `==` | Igual a |
| `!=` | Distinto de |
| `<` | Menor que |
| `>` | Mayor que |
| `<=` | Menor o igual que |
| `>=` | Mayor o igual que |

---

# Operadores lógicos

## `and`

```python
if username == "bmoreno" and login_attempts < 5:
```

Ambas condiciones deben ser verdaderas.

---

## `or`

```python
if status == 100 or status == 102:
```

Basta con que una condición sea verdadera.

---

## `not`

```python
if not account_status == "removed":
```

Invierte el valor lógico de una condición.

---

## `in`

Comprueba si un elemento pertenece a una secuencia.

```python
if user in approved_list:
```

---

# Bucles

## `for`

Recorre una secuencia.

```python
for username in ["bmoreno", "tshah", "elarson"]:
    print(username)
```

---

## `for` con `range()`

```python
for i in range(10):
    print(i)
```

---

## `while`

Repite instrucciones mientras una condición sea verdadera.

```python
while login_attempts < 5:
    print(login_attempts)
```

---

## `break`

Finaliza inmediatamente un bucle.

```python
for asset in computer_assets:

    if asset == "desktop20":
        break

    print(asset)
```

---

## `continue`

Omite la iteración actual y continúa con la siguiente.

```python
for asset in computer_assets:

    if asset == "desktop20":
        continue

    print(asset)
```

---

# Resumen de funciones

| Función | Propósito |
|----------|-----------|
| `print()` | Mostrar información en pantalla. |
| `type()` | Obtener el tipo de un dato. |
| `range()` | Generar secuencias numéricas. |

---

# Resumen de palabras clave

| Palabra clave | Uso |
|---------------|-----|
| `if` | Inicia una condición. |
| `elif` | Evalúa otra condición. |
| `else` | Ejecuta el bloque alternativo. |
| `for` | Recorre una secuencia. |
| `while` | Repite mientras una condición sea verdadera. |
| `break` | Finaliza un bucle. |
| `continue` | Omite la iteración actual. |
| `and` | Todas las condiciones deben cumplirse. |
| `or` | Basta con una condición verdadera. |
| `not` | Niega una condición. |
| `in` | Comprueba pertenencia a una secuencia. |

---

# Contenido cubierto en el Módulo 1

- Comentarios
- Variables
- Tipos de datos
- Funciones
- Sentencias condicionales
- Operadores de comparación
- Operadores lógicos
- Bucles `for`
- Bucles `while`
- `break`
- `continue`
- Automatización
- Glosario

---

⬅️ **[Volver al índice del módulo](README.md)**

⬆️ **[Volver al repositorio principal](../README.md)**
