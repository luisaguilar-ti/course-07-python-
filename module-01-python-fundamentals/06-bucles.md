# 06 - Bucles en Python

## Introducción

Los bucles son estructuras de control que permiten ejecutar un bloque de código de forma repetitiva. En lugar de escribir las mismas instrucciones varias veces, un bucle repite automáticamente las acciones según una condición o una secuencia de elementos.

En Python existen dos tipos principales de bucles:

- `for`
- `while`

Además, pueden controlarse mediante las palabras clave `break` y `continue`.

---

# Objetivos de aprendizaje

Al finalizar este tema podrás:

- Comprender qué es una sentencia iterativa.
- Utilizar bucles `for` para recorrer secuencias.
- Utilizar `range()` para generar secuencias numéricas.
- Utilizar bucles `while` basados en condiciones.
- Controlar la ejecución de un bucle con `break` y `continue`.
- Comprender qué es un bucle infinito.

---

# ¿Qué es una sentencia iterativa?

Una **sentencia iterativa** es un bloque de código que ejecuta repetidamente un conjunto de instrucciones.

Dependiendo de la condición o de la secuencia utilizada, el bloque puede ejecutarse cero, una o varias veces.

---

# Bucle `for`

El bucle `for` se utiliza para recorrer una secuencia de elementos.

## Sintaxis

```python
for variable in secuencia:
    instrucciones
```

La variable de bucle toma el valor de cada elemento de la secuencia durante cada iteración.

---

## Ejemplo

```python
for i in ["elarson", "bmoreno", "tshah", "sgilmore"]:
    print(i)
```

**Salida**

```text
elarson
bmoreno
tshah
sgilmore
```

---

# Recorrer una lista

Las listas son una de las estructuras más comunes utilizadas con los bucles `for`.

```python
computer_assets = [
    "laptop1",
    "desktop20",
    "smartphone03"
]

for asset in computer_assets:
    print(asset)
```

Cada iteración procesa un elemento diferente de la lista.

---

# Recorrer una cadena

También es posible recorrer una cadena de texto carácter por carácter.

```python
string = "security"

for character in string:
    print(character)
```

Cada iteración devuelve un carácter diferente.

---

# La función `range()`

`range()` genera una secuencia de números que suele utilizarse con un bucle `for`.

## Sintaxis

```python
range(inicio, fin, incremento)
```

Ejemplo:

```python
for i in range(0,5,1):
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

El punto inicial es **inclusivo** y el punto final es **exclusivo**.

---

## Forma abreviada

Cuando el inicio es `0` y el incremento es `1`, ambos pueden omitirse.

```python
for i in range(5):
    print(i)
```

Produce exactamente la misma secuencia.

---

# Bucle `while`

El bucle `while` ejecuta instrucciones mientras una condición sea verdadera.

## Sintaxis

```python
while condicion:
    instrucciones
```

---

## Ejemplo

```python
i = 1

while i < 5:
    print(i)
    i = i + 1
```

**Salida**

```text
1
2
3
4
```

En cada iteración la variable cambia de valor hasta que la condición deja de cumplirse.

---

# Condiciones con enteros

Es común utilizar un contador para controlar el número de iteraciones.

```python
login_attempts = 0

while login_attempts < 5:
    print(login_attempts)
    login_attempts = login_attempts + 1
```

---

# Condiciones booleanas

Un bucle también puede depender de una variable booleana.

```python
count = 0
login_status = True

while login_status == True:
    print("Try again.")
    count = count + 1

    if count == 4:
        login_status = False
```

Cuando `login_status` cambia a `False`, el bucle finaliza.

---

# La palabra clave `break`

`break` finaliza inmediatamente un bucle cuando se cumple una condición.

```python
computer_assets = [
    "laptop1",
    "desktop20",
    "smartphone03"
]

for asset in computer_assets:

    if asset == "desktop20":
        break

    print(asset)
```

**Salida**

```text
laptop1
```

Al encontrar `"desktop20"` el bucle termina y no continúa con los elementos restantes.

---

# La palabra clave `continue`

`continue` omite únicamente la iteración actual y continúa con la siguiente.

```python
computer_assets = [
    "laptop1",
    "desktop20",
    "smartphone03"
]

for asset in computer_assets:

    if asset == "desktop20":
        continue

    print(asset)
```

**Salida**

```text
laptop1
smartphone03
```

En este caso `"desktop20"` no se imprime, pero el bucle continúa con el siguiente elemento.

---

# Bucle infinito

Un **bucle infinito** ocurre cuando la condición del bucle nunca llega a ser falsa.

En estos casos, el programa continuará ejecutándose indefinidamente hasta que sea detenido manualmente.

Durante el curso se menciona que puede detenerse utilizando:

- `CTRL + C`
- `CTRL + Z`

según el entorno donde se esté ejecutando el programa.

---

# Resumen

| Concepto | Descripción |
|----------|-------------|
| `for` | Recorre una secuencia de elementos. |
| `while` | Repite instrucciones mientras una condición sea verdadera. |
| Variable de bucle | Controla cada iteración del bucle. |
| `range()` | Genera secuencias numéricas. |
| `break` | Finaliza inmediatamente un bucle. |
| `continue` | Omite la iteración actual y continúa con la siguiente. |
| Bucle infinito | Bucle cuya condición nunca deja de ser verdadera. |

---

# Puntos clave

- Los bucles permiten automatizar tareas repetitivas.
- `for` recorre secuencias como listas, cadenas y rangos numéricos.
- `while` depende de una condición booleana.
- `range()` genera secuencias de números.
- `break` termina un bucle antes de tiempo.
- `continue` omite únicamente la iteración actual.
- Un bucle infinito nunca finaliza hasta que es detenido manualmente.

---

## Siguiente tema

➡️ **[07 - Automatización con Python](07-automatizacion.md)**

⬅️ **[Volver al índice del módulo](README.md)**
