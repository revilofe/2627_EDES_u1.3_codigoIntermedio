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

Explica por qué `Suma.java` es código fuente y qué salida esperas obtener antes
de compilarlo.

**Respuesta:**

<!-- Escribe aquí tu explicación. -->

## 4. Compilación y generación de bytecode

Ejecuta el comando siguiente:

```bash
javac Suma.java
```

Completa la tabla:

| Elemento | Tipo o función | Momento en el que interviene | Evidencia |
|---|---|---|---|
| `Suma.java` |  |  |  |
| `javac` |  |  |  |
| `Suma.class` |  |  |  |

Explica qué diferencia hay entre el código fuente y el bytecode, y por qué
`Suma.class` no es un ejecutable nativo para una CPU concreta.

**Respuesta:**

<!-- Completa la respuesta. -->

## 5. Ejecución en la JVM

Ejecuta:

```bash
java Suma
```

Salida inicial:

```text
<!-- Pega aquí la salida. Debería ser «El resultado es: 12». -->
```

Responde:

- ¿Qué hace la herramienta `java`?
- ¿Qué papel desempeña la JVM?
- ¿Qué relación existe entre `Suma.class`, la JVM y el sistema operativo?

**Respuesta:**

<!-- Escribe aquí tus respuestas. -->

## 6. Inspección del bytecode

Ejecuta:

```bash
javap -c Suma
```

Incluye un fragmento de la salida:

```text
<!-- Pega aquí el fragmento relevante de `javap -c Suma`. -->
```

Responde:

1. ¿Qué instrucciones relacionadas con la suma o la salida puedes identificar?
2. ¿Por qué la salida de `javap -c` no es código máquina de tu procesador?
3. ¿Qué información puedes observar y qué información no puedes deducir solo
   con esta salida?

**Respuesta:**

<!-- Completa la respuesta. -->

## 7. Modificación y reconstrucción

Cambia los valores de `num1` y `num2` a `17` y `25`.

### 7.1. Predicción

- Resultado esperado: <!-- Completa la predicción. -->
- Motivo por el que hay que volver a compilar: <!-- Completa la explicación. -->

### 7.2. Comandos y resultados

```bash
<!-- Escribe los comandos utilizados para compilar y ejecutar de nuevo. -->
```

Salida después de recompilar:

```text
<!-- Pega aquí la salida. Debería ser «El resultado es: 42». -->
```

Explica qué podría ocurrir si modificases `Suma.java` pero ejecutases el archivo
`.class` antiguo sin volver a compilar.

**Respuesta:**

<!-- Completa la respuesta. -->

## 8. Portabilidad y requisitos del entorno

Explica si bastaría con copiar `Suma.class` a otro equipo para ejecutarlo.
Indica qué requisitos deben cumplirse y qué papel tienen la versión de la JVM,
las bibliotecas y las dependencias.

**Respuesta:**

<!-- Escribe aquí tu explicación. -->

### Ampliación opcional: otro equipo o sistema operativo

| Dato | Valor |
|---|---|
| Archivos copiados |  |
| Sistema de destino |  |
| Versión de la JVM |  |
| Resultado |  |
| Incidencias o requisitos detectados |  |

## 9. Prácticas generales de trabajo

Identifica al menos cuatro prácticas transferibles a otros lenguajes o
herramientas y justifica cómo ayudan a evitar errores o a reproducir el proceso.

| Práctica | Evidencia de esta actividad | Error que ayuda a prevenir |
|---|---|---|
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |

## 10. Evidencias

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

## 11. Reflexión final

Explica qué has aprendido sobre el código fuente, el bytecode, `javac`, `java`,
`javap`, la JVM y las condiciones que hacen posible la portabilidad.

<!-- Escribe aquí tu reflexión. -->

## 12. Lista de comprobación

- [ ] He completado la identificación y el entorno de trabajo.
- [ ] He creado y conservado `Suma.java`.
- [ ] He generado `Suma.class` con `javac`.
- [ ] He ejecutado el programa y he documentado la salida `12`.
- [ ] He inspeccionado el bytecode con `javap -c`.
- [ ] He cambiado los operandos a `17` y `25` y he obtenido `42`.
- [ ] He explicado el papel de la JVM y los requisitos de portabilidad.
- [ ] He identificado al menos cuatro prácticas generales de trabajo.
- [ ] He añadido las evidencias solicitadas.
- [ ] He escrito la reflexión final.
