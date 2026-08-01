# Funciones definidas por el usuario

## ¿Qué es una función?

Una función es una sección de código reutilizable que ejecuta una tarea específica. Su principal objetivo es evitar escribir el mismo código varias veces, haciendo que los programas sean más organizados, fáciles de mantener y reutilizables.

En ciberseguridad, las funciones permiten automatizar procesos repetitivos como:

- Analizar registros (logs).
- Verificar intentos de inicio de sesión.
- Validar usuarios.
- Revisar permisos.
- Generar alertas.

---

## Funciones integradas vs funciones definidas por el usuario

Python posee dos tipos principales de funciones.

### Funciones integradas (Built-in Functions)

Son funciones que ya vienen incluidas en Python.

Ejemplos:

- `print()`
- `type()`
- `max()`
- `min()`
- `sorted()`

No necesitan ser creadas por el programador.

---

### Funciones definidas por el usuario

Son funciones creadas por el programador para resolver necesidades específicas.

Se definen utilizando la palabra reservada:

```python
def
```

---

## Sintaxis básica

```python
def nombre_funcion():
    print("Hola")
```

Componentes:

- `def` → indica el inicio de una función.
- `nombre_funcion` → nombre descriptivo de la función.
- `()` → paréntesis donde posteriormente se colocarán parámetros.
- `:` → final del encabezado.
- Bloque indentado → cuerpo de la función.

---

## Definir una función

Definir una función significa decirle a Python que esa función existe.

Ejemplo:

```python
def greet_employee():
    print("Welcome employee")
```

Al ejecutar este código no sucede nada visible.

La función solamente queda almacenada en memoria.

---

## Llamar una función

Para ejecutar una función es necesario llamarla.

Ejemplo:

```python
greet_employee()
```

Ahora Python ejecuta todo el código contenido dentro de la función.

---

## Flujo de ejecución

```text
Definir función
        ↓
La función queda almacenada
        ↓
Llamar función
        ↓
Python ejecuta el contenido
```

---

## Ventajas de utilizar funciones

- Evitan repetir código.
- Facilitan el mantenimiento.
- Mejoran la organización del programa.
- Hacen el código más legible.
- Permiten reutilizar procesos múltiples veces.

Si es necesario modificar una tarea, basta con cambiar una sola función en lugar de modificar muchas líneas del programa.

---

## Ejemplo práctico

```python
def alerta():
    print("Posible incidente de seguridad.")

alerta()
```

Salida:

```
Posible incidente de seguridad.
```

---

## Aplicación en ciberseguridad

Las funciones pueden utilizarse para automatizar tareas como:

- Mostrar alertas.
- Analizar registros.
- Validar credenciales.
- Revisar permisos.
- Detectar comportamientos sospechosos.
- Procesar eventos de seguridad.

---

## Buenas prácticas

- Asignar nombres descriptivos.
- Mantener una única responsabilidad por función.
- Evitar funciones demasiado largas.
- Escribir comentarios cuando la función sea compleja.
- Reutilizar funciones en lugar de duplicar código.

---

## Conceptos clave

- Función
- Función definida por el usuario
- Función integrada
- `def`
- Llamada a función
- Reutilización de código
