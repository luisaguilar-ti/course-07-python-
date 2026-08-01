# Guía de estilo PEP 8 y legibilidad del código

## Introducción

Python es un lenguaje de programación reconocido por su facilidad de lectura. Para mantener esa característica, la comunidad de Python creó la **Guía de estilo PEP 8**, un conjunto de recomendaciones para escribir código de forma clara y consistente.

PEP significa **Python Enhancement Proposal (Propuesta de Mejora de Python)**.

Aunque estas recomendaciones no son obligatorias, ayudan a que el código sea más fácil de leer, mantener y compartir con otros programadores.

---

# ¿Qué es la guía PEP 8?

La **Guía de estilo PEP 8** es un recurso que proporciona recomendaciones sobre cómo escribir y dar formato al código Python.

Su propósito es que los programadores sigan convenciones similares al escribir código.

El principio principal de PEP 8 es:

> **"El código se lee mucho más de lo que se escribe."**

---

# Comentarios

Un comentario es una nota que los programadores escriben para explicar la intención del código.

Los comentarios ayudan a que otras personas comprendan rápidamente qué hace un programa y también facilitan que el propio autor pueda entender su código cuando lo revise tiempo después.

PEP 8 recomienda que los comentarios sean:

- Claros.
- Breves.
- Mantenerse actualizados cuando el código cambie.

Ejemplo:

```python
# Bloquear la cuenta cuando se exceda el número máximo de intentos
```

---

# Código con y sin comentarios

Sin comentarios:

```python
failed_attempts = 6

if failed_attempts > 5:
    print("Account locked")
```

El programa funciona correctamente, pero otra persona podría no entender fácilmente el propósito del código.

Con comentarios:

```python
# Bloquear la cuenta cuando existan más de cinco intentos fallidos

failed_attempts = 6

if failed_attempts > 5:
    print("Account locked")
```

El comentario explica la intención del código y mejora su comprensión.

---

# Indentación

La **indentación** es el espacio que se agrega al inicio de una línea de código.

En Python, la indentación tiene dos funciones importantes:

- Mejorar la legibilidad.
- Indicar qué instrucciones pertenecen a un mismo bloque de código.

Por ejemplo, el cuerpo de una sentencia `if` debe estar indentado para que Python entienda que esas instrucciones solo deben ejecutarse cuando la condición sea verdadera.

```python
if updates_needed:
    print("Updates required")
```

Si la línea `print()` no estuviera indentada, dejaría de pertenecer al bloque del `if` y el programa tendría un comportamiento diferente.

---

# Recomendación de PEP 8

PEP 8 recomienda utilizar **cuatro espacios** por cada nivel de indentación.

Esto ayuda a mantener un formato uniforme y facilita la lectura del código.

---

# Importancia de seguir una guía de estilo

Cuando varias personas trabajan sobre un mismo proyecto, utilizar una guía de estilo común facilita:

- Leer el código.
- Comprender su funcionamiento.
- Modificarlo con el paso del tiempo.
- Colaborar con otros programadores.

---

# Ideas principales

- PEP 8 es la guía oficial de estilo para Python.
- Su objetivo es mejorar la legibilidad y consistencia del código.
- Los comentarios explican la intención del programa.
- La indentación mejora la lectura del código y es necesaria para que Python interprete correctamente los bloques.
- PEP 8 recomienda utilizar cuatro espacios por nivel de indentación.

---

# Conceptos clave

- PEP 8
- Guía de estilo
- Comentarios
- Indentación
- Legibilidad
