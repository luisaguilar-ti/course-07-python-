# 04 - Funciones básicas en Python

## Introducción

Una función es un bloque de código diseñado para realizar una tarea específica. Python incluye numerosas funciones integradas (*built-in functions*) que permiten ejecutar acciones comunes sin necesidad de escribirlas desde cero.

Durante este módulo se introducen tres funciones fundamentales:

- `print()`
- `type()`
- `range()`

Estas funciones son utilizadas constantemente en los ejemplos y ejercicios del curso.

---

# Objetivos de aprendizaje

Al finalizar este tema podrás:

- Comprender qué es una función.
- Utilizar la función `print()` para mostrar información.
- Utilizar `type()` para identificar el tipo de un dato.
- Utilizar `range()` para generar secuencias numéricas en bucles.

---

# ¿Qué es una función?

Una función es un conjunto de instrucciones que realiza una tarea específica cuando es llamada.

Las funciones ayudan a simplificar el código y permiten reutilizar operaciones frecuentes.

---

# La función `print()`

La función `print()` muestra información en la pantalla.

Es una de las funciones más utilizadas para visualizar resultados durante la ejecución de un programa.

## Sintaxis

```python
print(objeto)
```

## Ejemplo

```python
print("Login success")
```

**Salida**

```text
Login success
```

También puede mostrar el resultado de una expresión.

```python
print(9 < 7)
```

**Salida**

```text
False
```

En este caso, primero se evalúa la comparación y posteriormente se imprime el resultado.

---

# La función `type()`

La función `type()` devuelve el tipo de dato de un valor o de una variable.

## Sintaxis

```python
type(objeto)
```

## Ejemplo

```python
print(type(51.1))
```

**Salida**

```text
<class 'float'>
```

Otro ejemplo:

```python
print(type(True))
```

**Salida**

```text
<class 'bool'>
```

Esta función es útil para verificar qué tipo de dato está siendo utilizado dentro de un programa.

---

# La función `range()`

La función `range()` genera una secuencia de números.

Se utiliza principalmente junto con los bucles `for`.

## Sintaxis general

```python
range(inicio, fin, incremento)
```

Donde:

- **inicio**: primer valor de la secuencia.
- **fin**: valor donde termina la secuencia (no se incluye).
- **incremento**: cantidad que aumenta entre cada número.

---

## Ejemplo completo

```python
range(0, 5, 1)
```

La secuencia generada es:

```text
0
1
2
3
4
```

El valor **5** no forma parte de la secuencia porque el punto final es exclusivo.

---

## Forma abreviada

Si el inicio es `0` y el incremento es `1`, ambos pueden omitirse.

```python
range(5)
```

Produce exactamente la misma secuencia:

```text
0
1
2
3
4
```

---

# Uso de `range()` en un bucle

```python
for i in range(5):
    print(i)
```

**Salida**

```text
0
1
2
3
4
```

En este ejemplo:

- `range()` genera la secuencia.
- El bucle `for` recorre cada número.
- `print()` muestra el valor actual.

---

# Resumen de funciones

| Función | Propósito |
|----------|-----------|
| `print()` | Mostrar información en pantalla. |
| `type()` | Identificar el tipo de dato de un valor. |
| `range()` | Generar secuencias numéricas. |

---

# Puntos clave

- Las funciones permiten ejecutar tareas específicas.
- `print()` muestra información en la pantalla.
- `type()` devuelve el tipo de un dato o una variable.
- `range()` genera secuencias de números.
- El valor inicial de `range()` es inclusivo.
- El valor final de `range()` es exclusivo.
- `range()` se utiliza con frecuencia en los bucles `for`.

---

## Siguiente tema

➡️ **[05 - Sentencias condicionales](05-condicionales.md)**

⬅️ **[Volver al índice del módulo](README.md)**
