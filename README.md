# EDES U1 P14 - Código intermedio y máquina virtual Java

Plantilla de entrega para la práctica [EDES-U1.-Practica014](https://revilofe.github.io/section3/u01/practica/EDES-U1.-Practica014/).

Completa este `README.md`, crea y conserva `Suma.java` y añade las evidencias
solicitadas. No presentes el archivo `.class` como código fuente: documenta qué
archivo se genera y, si el aula lo permite, adjunta también el artefacto.

## 1. Identificación

| Dato | Valor |
|---|---|
| Nombre y apellidos | <!-- Completa este dato. --> |
| Módulo | Entornos de desarrollo |
| Unidad | U1 - Introducción al desarrollo de software |
| Práctica | P14 - Código intermedio y máquina virtual Java |
| Fecha | <!-- AAAA-MM-DD --> |

## 2. Entorno de trabajo

| Dato | Valor |
|---|---|
| Sistema operativo | <!-- Indica el sistema y su versión. --> |
| Arquitectura | <!-- Por ejemplo, x86_64 o arm64. --> |
| Versión de Java | <!-- Pega la salida de `java --version`. --> |
| Versión de `javac` | <!-- Pega la salida de `javac --version`. --> |
| Versión de `javap` | <!-- Pega la salida de `javap -version`. --> |
| Editor o IDE | <!-- Indica la herramienta utilizada. --> |
| Terminal | <!-- Bash, PowerShell, otra. --> |

Comandos utilizados para comprobar el entorno:

```text
<!-- Escribe los comandos y resume sus salidas. -->
```

## 3. Código fuente Java

Crea un archivo llamado exactamente `Suma.java` con este programa inicial:

```java
public class Suma {
    public static void main(String[] args) {
        int num1 = 5;
        int num2 = 7;
        int resultado = num1 + num2;
        System.out.println("El resultado es: " + resultado);
    }
}
```

`Suma.java` es el código fuente que se escribe y modifica. El nombre del
archivo debe coincidir con el de la clase pública `Suma`.

**Respuesta:**

<!-- Explica por qué `Suma.java` es código fuente y qué salida esperas obtener
antes de compilarlo. -->

## 4. Preparación, compilación y ejecución inicial

Crea una carpeta para la práctica y trabaja desde una terminal situada en ella.
Comprueba las versiones de las herramientas y registra el sistema operativo y
su versión.

Ejecuta:

```bash
java --version
javac --version
javap -version
```

Después, desde la carpeta que contiene `Suma.java`, ejecuta:

```bash
javac Suma.java
```

Si la compilación termina sin errores, comprueba que aparece `Suma.class`.

A continuación ejecuta:

```bash
java Suma
```

Conserva evidencias de las versiones, de la generación de `Suma.class` y de la
salida inicial.

## 5. Ejercicios y entregables

### Ejercicio 1: reconocer herramientas y artefactos

**Pregunta 1.a:** Completa una tabla con `Suma.java`, `Suma.class`, `javac`, `java`, `javap` y la JVM.

**Subpregunta 1.a.1:** ¿Qué representa o hace cada elemento?

**Subpregunta 1.a.2:** ¿En qué momento interviene cada elemento?

**Subpregunta 1.a.3:** ¿Cuál es código fuente, cuál es bytecode, cuáles son herramientas y cuál es el entorno de ejecución?

**Respuesta:**

Completa la tabla:

| Elemento | Tipo o función | Momento en el que interviene |
|----------|----------------|------------------------------|
| `Suma.java` |  |  |
| `Suma.class` |  |  |
| `javac` |  |  |
| `java` |  |  |
| `javap` |  |  |
| JVM |  |  |

<!-- Responde también a las tres subpreguntas con la tabla y, si es necesario,
con una explicación adicional. -->

### Ejercicio 2: proceso de ejecución y portabilidad

**Pregunta 2.a:** ¿Qué diferencia hay entre el código fuente y el bytecode de `Suma`?

**Respuesta:**

<!-- Escribe tu respuesta. -->

**Subpregunta 2.b:** ¿Qué hace `javac` y qué hace la herramienta `java`?

**Respuesta:**

<!-- Escribe tu respuesta. -->

**Subpregunta 2.c:** ¿Por qué no se ejecuta `Suma.class` directamente haciendo doble clic o escribiendo su nombre como si fuera un programa nativo?

**Respuesta:**

<!-- Escribe tu respuesta. -->

**Subpregunta 2.d:** ¿Qué representa `iadd` en la salida de `javap -c`?

**Respuesta:**

<!-- Escribe tu respuesta. -->

**Subpregunta 2.d.1:** ¿Por qué esa salida no es código máquina de tu procesador?

**Respuesta:**

<!-- Escribe tu respuesta. -->

**Subpregunta 2.e:** ¿Qué aporta la JVM a la portabilidad?

**Respuesta:**

<!-- Escribe tu respuesta. -->

**Subpregunta 2.e.1:** ¿Qué debe seguir siendo compatible en el equipo de destino?

**Respuesta:**

<!-- Escribe tu respuesta. -->

**Pregunta 2.f:** Compara este proceso con la compilación nativa habitual de C o C++.

**Subpregunta 2.f.1:** ¿Qué artefacto se distribuye en cada caso?

**Respuesta:**

<!-- Escribe tu respuesta. -->

**Subpregunta 2.f.2:** ¿Qué tendrías que comprobar para ejecutarlo en otro sistema?

**Respuesta:**

<!-- Escribe tu respuesta. -->

### Resultados iniciales de los pasos 4.3 y 4.4

**Paso 4.3 — Enunciado:** En la misma carpeta, ejecuta `java Suma` para iniciar el método `main` mediante la JVM y comprueba la salida.

**Resultado:**

```text
<!-- Pega aquí la salida. Debe ser «El resultado es: 12». -->
```

**Paso 4.4 — Enunciado:** Ejecuta `javap -c Suma` y localiza en `main` instrucciones relacionadas con los valores, la suma y la salida.

**Resultado:**

```bash
<!-- Escribe el comando utilizado. -->
```

Incluye también un fragmento de la salida de `javap -c Suma`:

```text
<!-- Pega aquí el fragmento relevante. -->
```


### Ejercicio 3: modificar los operandos y reconstruir

**Pregunta 3.a:** Cambia los operandos a `17` y `25`.

**Subpregunta 3.a.1:** Antes de ejecutar, incluye tu predicción del resultado.

**Respuesta:**

- Resultado previsto: <!-- Completa la predicción. -->
- Justificación: <!-- Explica tu predicción. -->

**Subpregunta 3.a.2:** Explica qué ocurriría si editases `Suma.java` pero ejecutases el `.class` antiguo sin recompilar.

**Respuesta:**

<!-- Escribe tu respuesta. -->

**Subpregunta 3.a.3:** ¿Qué salida obtienes al ejecutar?

**Respuesta:**

```text
<!-- Pega aquí la salida. Debe ser «El resultado es: 42». -->
```

**Subpregunta 3.b:** Guarda el fuente, vuelve a compilarlo con `javac` y ejecuta la clase actualizada con `java Suma`. Registra las órdenes.

**Respuesta:**

```bash
<!-- Registra aquí las órdenes utilizadas. -->
```

<!-- Explica también qué comprobaste al volver a generar Suma.class. -->

### Ejercicio 4: prácticas generales de trabajo

**Pregunta 4.a:** Enumera al menos cuatro prácticas generales de trabajo observadas en la actividad y explica cómo ayudan a evitar errores o a reproducir el proceso.

**Respuesta:**

| Práctica | Evidencia de esta actividad | Error que ayuda a prevenir |
|---|---|---|
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |

<!-- Puedes añadir más filas si las necesitas. Justifica cada práctica. -->

### Entregable

**Pregunta 5.a:** Entrega `Suma.java` y un `README.md` identificado con tu nombre, módulo, unidad y práctica. Incluye las versiones del entorno, las órdenes utilizadas, la tabla, las respuestas, una captura o transcripción de las dos ejecuciones, un fragmento de `javap -c` y la reflexión sobre las prácticas generales. Adjunta también `Suma.class` o, si el aula no admite archivos binarios, una evidencia verificable de su generación.

**Respuesta:**

Completa esta lista para comprobar tu entrega:

- [ ] He identificado el README con mi nombre, módulo, unidad y práctica.
- [ ] He incluido las versiones del entorno.
- [ ] He registrado las órdenes utilizadas.
- [ ] He completado la tabla y las respuestas.
- [ ] He incluido una captura o transcripción de las dos ejecuciones.
- [ ] He incluido un fragmento de `javap -c`.
- [ ] He conservado `Suma.java`.
- [ ] He adjuntado `Suma.class` o una evidencia verificable de su generación.
- [ ] He incluido la reflexión sobre las prácticas generales.

**Comprobación del entregable:**

<!-- Explica cómo has comprobado que el README, Suma.java, Suma.class o su
evidencia y el resto de materiales están incluidos y son identificables. -->

### Ejercicio 6: ampliación opcional de portabilidad

**Enunciado 6.a:** Intenta ejecutar el mismo `Suma.class` en otro sistema operativo o equipo. Indica qué archivos copiaste, la versión de JVM disponible y si hubo algún requisito de versión o dependencia que afectase al resultado. La prueba en otro sistema es opcional.

**Respuesta:**

| Dato | Valor |
|---|---|
| Archivos copiados |  |
| Sistema de destino |  |
| Versión de la JVM |  |
| Resultado |  |
| Incidencias o requisitos detectados |  |

<!-- Si no realizas la ampliación, indícalo y explica qué requisitos serían
necesarios para ejecutarlo en otro equipo. -->

## 6. Reflexión final

Explica qué has aprendido sobre el código fuente, el bytecode, `javac`, `java`,
`javap`, la JVM y las condiciones que hacen posible la portabilidad.

<!-- Escribe aquí tu reflexión. -->

## 7. Evidencias

Incluye evidencias de:

- las versiones de `java`, `javac` y `javap`;
- la generación de `Suma.class`;
- la salida inicial `12`;
- la inspección con `javap -c`;
- la salida final `42`;
- la ampliación opcional, si la realizas.

Si incorporas imágenes, guárdalas en `evidencias/` y enlázalas desde este
apartado.

```text
<!-- Añade aquí listados, transcripciones o enlaces a las capturas. -->
```
