# Parámetros, argumentos y `return`

## Introducción

Las funciones se vuelven realmente útiles cuando pueden recibir información y devolver resultados.

Para ello, Python utiliza tres conceptos fundamentales:

- Parámetros
- Argumentos
- `return`

Estos tres elementos permiten crear funciones reutilizables y flexibles.

---

# Parámetros

Un parámetro es una variable que se declara en la definición de una función.

Su función es recibir información cuando la función sea llamada.

Ejemplo:

```python
def saludar(nombre):
    print("Hola", nombre)
```

En este ejemplo:

```python
nombre
```

es un **parámetro**.

---

# Argumentos

Un argumento es el valor real que se envía a una función cuando se llama.

Ejemplo:

```python
saludar("Luis")
```

Aquí:

```python
"Luis"
```

es el **argumento**.

Durante la ejecución ocurre lo siguiente:

```
Parámetro ← Argumento

nombre    ← "Luis"
```

---

# Relación entre parámetros y argumentos

```python
def saludar(nombre):
    print("Hola", nombre)

saludar("Luis")
```

- `nombre` → parámetro.
- `"Luis"` → argumento.

El argumento pasa al parámetro y la función puede utilizar ese valor.

---

# Funciones con varios parámetros

Una función puede recibir varios parámetros.

Ejemplo:

```python
def login(usuario, contraseña):
    print(usuario)
    print(contraseña)

login("luis", "1234")
```

Correspondencia:

| Parámetro | Argumento |
|-----------|-----------|
| usuario | "luis" |
| contraseña | "1234" |

El orden es importante.

---

# ¿Qué es `return`?

La palabra reservada `return` permite devolver información desde una función.

En lugar de solamente mostrar información en pantalla con `print()`, una función puede entregar un resultado para utilizarlo posteriormente.

Sintaxis:

```python
return valor
```

---

# Ejemplo de `return`

```python
def suma(a, b):
    return a + b
```

Llamada:

```python
resultado = suma(5, 3)

print(resultado)
```

Salida:

```
8
```

En este ejemplo:

- La función calcula el resultado.
- `return` devuelve ese valor.
- El resultado se almacena en una variable.

---

# Diferencia entre `print()` y `return`

## Usando `print()`

```python
def suma(a, b):
    print(a + b)
```

Solo muestra el resultado en pantalla.

---

## Usando `return`

```python
def suma(a, b):
    return a + b
```

Devuelve el resultado para poder utilizarlo después.

Por ejemplo:

```python
resultado = suma(5, 3)

if resultado > 5:
    print("Número válido")
```

Esto no sería posible utilizando únicamente `print()`.

---

# El flujo de `return`

Cuando Python encuentra un `return`:

1. Devuelve el valor indicado.
2. Finaliza inmediatamente la función.
3. No ejecuta ninguna línea que esté debajo del `return`.

Ejemplo:

```python
def ejemplo():

    print("Inicio")

    return 5

    print("Fin")
```

Salida:

```
Inicio
```

La línea:

```python
print("Fin")
```

nunca se ejecuta.

---

# Ejemplo del curso

El curso utiliza una función para calcular el porcentaje de intentos fallidos de inicio de sesión.

```python
def calculate_fails(total_attempts, failed_attempts):

    fail_percentage = failed_attempts / total_attempts

    return fail_percentage
```

Llamada:

```python
percentage = calculate_fails(4, 2)
```

Resultado:

```
0.5
```

Ese valor puede utilizarse posteriormente.

Ejemplo:

```python
if percentage >= 0.5:
    print("Cuenta bloqueada")
```

---

# Aplicación en ciberseguridad

Las funciones con parámetros y `return` permiten crear herramientas reutilizables para:

- Calcular porcentajes de intentos fallidos.
- Validar usuarios.
- Revisar permisos.
- Analizar registros.
- Detectar actividad sospechosa.
- Automatizar decisiones de seguridad.

---

# Buenas prácticas

- Utilizar nombres descriptivos para los parámetros.
- Mantener el orden correcto de los argumentos.
- Utilizar `return` cuando el resultado vaya a reutilizarse.
- Evitar imprimir resultados dentro de funciones que devolverán datos.
- Mantener una única responsabilidad por función.

---

# Conceptos clave

- Parámetro
- Argumento
- `return`
- Valor de retorno
- Función reutilizable
- Llamada a función
- Flujo de ejecución
