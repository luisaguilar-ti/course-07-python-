# Variables globales y locales

## Introducción

Las funciones trabajan constantemente con variables. Sin embargo, no todas las variables tienen el mismo alcance dentro de un programa.

En Python existen dos tipos principales:

- Variables globales
- Variables locales

Comprender la diferencia entre ambas es fundamental para evitar errores y escribir código más organizado.

---

# Variables globales

Una variable global es una variable creada fuera de cualquier función.

Puede utilizarse desde cualquier parte del programa, incluyendo el interior de las funciones.

Ejemplo:

```python
username = "elarson"

def mostrar_usuario():
    print(username)

mostrar_usuario()
```

Salida:

```
elarson
```

La función puede acceder a la variable porque fue creada fuera de ella.

---

# Características de una variable global

- Se define fuera de una función.
- Está disponible en todo el programa.
- Puede ser utilizada por varias funciones.
- Permanece en memoria mientras el programa se ejecuta.

---

# Variables locales

Una variable local es una variable creada dentro de una función.

Solo existe mientras esa función se está ejecutando.

Cuando la función termina, Python elimina esa variable de la memoria.

Ejemplo:

```python
def saludo():

    mensaje = "Bienvenido"

    print(mensaje)

saludo()
```

La variable:

```python
mensaje
```

solo existe dentro de la función.

---

# ¿Qué ocurre fuera de la función?

Si intentamos usar una variable local fuera de la función:

```python
def saludo():

    mensaje = "Bienvenido"

print(mensaje)
```

Python genera un error porque la variable ya no existe fuera del cuerpo de la función.

---

# Los parámetros también son variables locales

Los parámetros creados en la definición de una función también son variables locales.

Ejemplo:

```python
def saludar(nombre):

    print(nombre)
```

Aquí:

```python
nombre
```

es una variable local.

Solo existe mientras la función se está ejecutando.

---

# Variables locales creadas dentro de la función

También pueden crearse variables adicionales.

Ejemplo:

```python
def greet_employee(nombre):

    mensaje = "Bienvenido " + nombre

    return mensaje
```

Variables locales:

- nombre
- mensaje

Ambas desaparecen cuando termina la función.

---

# Variables globales dentro de funciones

Las funciones pueden leer variables globales.

Ejemplo:

```python
usuario = "elarson"

def identificar():

    print(usuario)

identificar()
```

La salida será:

```
elarson
```

---

# Reutilizar nombres de variables

Es posible crear una variable local con el mismo nombre que una variable global.

Ejemplo:

```python
usuario = "elarson"

def saludo():

    usuario = "bmoreno"

    print(usuario)

saludo()

print(usuario)
```

Salida:

```
bmoreno
elarson
```

¿Qué ocurrió?

Dentro de la función existe una variable local llamada `usuario`.

Fuera de la función sigue existiendo la variable global.

Son dos variables distintas aunque tengan el mismo nombre.

---

# ¿Por qué puede ser un problema?

Reutilizar nombres puede hacer que el código sea difícil de entender.

Puede parecer que una variable cambió cuando en realidad Python está utilizando dos variables diferentes.

Por esta razón, el curso recomienda evitar reutilizar nombres entre variables globales y locales.

---

# Buenas prácticas

- Utilizar parámetros en lugar de depender de variables globales.
- Asignar nombres descriptivos a las variables.
- Evitar reutilizar el mismo nombre para variables globales y locales.
- Mantener las funciones independientes siempre que sea posible.

---

# Aplicación en ciberseguridad

Las variables locales ayudan a que cada función procese únicamente la información necesaria.

Por ejemplo:

- Validar un usuario.
- Analizar un registro.
- Revisar permisos.
- Calcular intentos fallidos.

Mientras que las variables globales pueden utilizarse para almacenar información compartida, como:

- Configuración del sistema.
- Directorios de trabajo.
- Rutas de archivos.
- Constantes del programa.

---

# Resumen

| Variable global | Variable local |
|-----------------|----------------|
| Se crea fuera de una función | Se crea dentro de una función |
| Disponible en todo el programa | Solo existe dentro de la función |
| Permanece durante la ejecución | Desaparece al terminar la función |
| Puede ser utilizada por varias funciones | Solo puede utilizarse dentro de la función |

---

# Conceptos clave

- Variable global
- Variable local
- Alcance (Scope)
- Parámetro
- Función
- Memoria
- Reutilización de variables
