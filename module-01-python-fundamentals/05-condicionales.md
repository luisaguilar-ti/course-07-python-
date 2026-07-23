# 05 - Sentencias condicionales

## Introducción

Las sentencias condicionales permiten que un programa tome decisiones en función de si una condición se evalúa como **True** o **False**.

En lugar de ejecutar siempre las mismas instrucciones, un programa puede seguir diferentes caminos dependiendo del resultado de una comparación.

---

# Objetivos de aprendizaje

Al finalizar este tema podrás:

- Comprender el funcionamiento de las sentencias condicionales.
- Utilizar `if`, `elif` y `else`.
- Aplicar operadores de comparación.
- Utilizar operadores lógicos para combinar condiciones.
- Emplear el operador `in` para comprobar la pertenencia a una secuencia.

---

# ¿Qué es una sentencia condicional?

Una sentencia condicional evalúa una condición antes de ejecutar un bloque de código.

Si la condición es **True**, Python ejecuta las instrucciones correspondientes.

Si la condición es **False**, el programa continúa con la siguiente condición o con el bloque `else`, si existe.

---

# La sentencia `if`

La palabra clave `if` inicia una sentencia condicional.

## Sintaxis

```python
if condicion:
    instrucciones
```

## Ejemplo

```python
if device_id != "la858zn":
    print("Unknown device")
```

En este ejemplo, el mensaje se mostrará únicamente cuando el valor almacenado en `device_id` sea diferente de `"la858zn"`.

---

# Operadores de comparación

Las condiciones suelen construirse mediante operadores de comparación.

| Operador | Significado |
|----------|-------------|
| `==` | Igual a |
| `!=` | Distinto de |
| `<` | Menor que |
| `>` | Mayor que |
| `<=` | Menor o igual que |
| `>=` | Mayor o igual que |

## Ejemplo

```python
if login_attempts < 5:
    print("Login allowed")
```

---

# El operador `in`

El operador `in` permite comprobar si un elemento pertenece a una secuencia.

## Ejemplo

```python
if user in approved_list:
    print("User approved")
```

Si el valor de `user` se encuentra dentro de `approved_list`, la condición será **True**.

---

# La sentencia `elif`

`elif` permite evaluar una nueva condición cuando la condición anterior fue **False**.

## Sintaxis

```python
if condicion:
    instrucciones

elif otra_condicion:
    instrucciones
```

## Ejemplo

```python
if status == 200:
    print("Success")

elif status == 500:
    print("Server error")
```

La condición del `elif` solamente se evalúa cuando la condición del `if` resulta falsa.

---

# La sentencia `else`

`else` se ejecuta cuando ninguna de las condiciones anteriores es verdadera.

## Sintaxis

```python
if condicion:
    instrucciones

else:
    instrucciones
```

## Ejemplo

```python
if login_status == True:
    print("Access granted")

else:
    print("Access denied")
```

---

# Operadores lógicos

Los operadores lógicos permiten combinar varias condiciones.

---

## Operador `and`

Todas las condiciones deben ser verdaderas.

```python
if username == "bmoreno" and login_attempts < 5:
    print("Access granted")
```

La condición completa será verdadera únicamente cuando ambas expresiones sean verdaderas.

---

## Operador `or`

Basta con que una de las condiciones sea verdadera.

```python
if status == 100 or status == 102:
    print("Processing")
```

Si cualquiera de las dos condiciones se cumple, el resultado será **True**.

---

## Operador `not`

Niega una condición.

Si una condición es **True**, `not` la convierte en **False**.

Si una condición es **False**, `not` la convierte en **True**.

## Ejemplo

```python
if not account_status == "removed":
    print("Account active")
```

En este ejemplo, el código se ejecutará siempre que `account_status` sea distinto de `"removed"`.

---

# Flujo de evaluación

Python evalúa una sentencia condicional siguiendo este orden:

1. Evalúa la condición del `if`.
2. Si es **True**, ejecuta ese bloque y finaliza la sentencia condicional.
3. Si es **False**, evalúa el primer `elif`.
4. Continúa evaluando los demás `elif`, si existen.
5. Si ninguna condición es verdadera, ejecuta el bloque `else`.

---

# Resumen de palabras clave

| Palabra clave | Función |
|---------------|---------|
| `if` | Inicia una condición. |
| `elif` | Evalúa otra condición si la anterior fue falsa. |
| `else` | Se ejecuta cuando ninguna condición anterior es verdadera. |
| `and` | Todas las condiciones deben ser verdaderas. |
| `or` | Basta con una condición verdadera. |
| `not` | Invierte el valor lógico de una condición. |
| `in` | Comprueba si un elemento pertenece a una secuencia. |

---

# Puntos clave

- Las sentencias condicionales permiten tomar decisiones dentro de un programa.
- `if` inicia una condición.
- `elif` permite evaluar condiciones adicionales.
- `else` se ejecuta cuando ninguna condición anterior es verdadera.
- Los operadores de comparación producen valores booleanos.
- `and`, `or` y `not` permiten combinar condiciones.
- El operador `in` verifica si un elemento pertenece a una secuencia.
- Python ejecuta únicamente el primer bloque cuya condición sea verdadera.

---

## Siguiente tema

➡️ **[06 - Bucles](06-bucles.md)**

⬅️ **[Volver al índice del módulo](README.md)**
