# DOSW_Lab4_Inicial_Kevyn_Diego_Juliana

## Laboratorio 4 - Bankify

### Integrantes
- Kevyn
- Diego
- Juliana

---

## Parte 1 – Estructura del Proyecto

### Preguntas

#### a. ¿Qué es un arquetipo (Archetype) en Maven?

Un arquetipo en Maven es una plantilla o modelo de proyecto que define una estructura de directorios estándar, archivos de configuración iniciales y dependencias básicas. Los arquetipos permiten generar rápidamente la estructura base de un proyecto siguiendo las convenciones y mejores prácticas de Maven, evitando que el desarrollador tenga que crear manualmente todos los archivos y carpetas necesarios. En esencia, un arquetipo es un patrón o prototipo a partir del cual se crean nuevos proyectos (Apache Maven Project, s.f.).

#### b. ¿Para qué sirve el arquetipo maven-archetype-quickstart?

El arquetipo `maven-archetype-quickstart` sirve para generar un proyecto Java básico con la estructura estándar de Maven. Al utilizarlo, se crea automáticamente:

- Un archivo `pom.xml` con la configuración básica del proyecto.
- Un directorio `src/main/java` con una clase principal de ejemplo (`App.java`).
- Un directorio `src/test/java` con una clase de prueba unitaria de ejemplo (`AppTest.java`).

Este arquetipo es ideal para iniciar rápidamente un proyecto Java simple, ya que proporciona la estructura mínima necesaria para compilar, ejecutar pruebas y empaquetar el proyecto (Apache Maven Project, s.f.).

#### c. ¿Cuál es el comando con el cual se puede crear un proyecto basado en un arquetipo Maven?

El comando para crear un proyecto basado en un arquetipo Maven es:

```bash
mvn archetype:generate -DgroupId=<groupId> -DartifactId=<artifactId> -DarchetypeArtifactId=<archetype> -DinteractiveMode=false
```

Donde:
- `-DgroupId`: Identificador del grupo o la organización (por ejemplo, `edu.dosw.lab`).
- `-DartifactId`: Nombre del proyecto o artefacto (por ejemplo, `DOSW-Laboratorio4`).
- `-DarchetypeArtifactId`: Nombre del arquetipo a utilizar (por ejemplo, `maven-archetype-quickstart`).
- `-DinteractiveMode=false`: Desactiva el modo interactivo para que Maven no solicite confirmación de parámetros.

#### d. ¿Qué es un pull request en GitHub?

Un pull request (PR) en GitHub es una solicitud formal para integrar los cambios realizados en una rama de un repositorio a otra rama (generalmente a la rama principal o `develop`). El pull request permite a los miembros del equipo revisar el código propuesto, agregar comentarios, solicitar cambios o aprobar las modificaciones antes de que se fusionen. Es una herramienta fundamental para la colaboración y la revisión de código en proyectos de software (GitHub Docs, s.f.).

#### e. ¿Cómo se crea un pull request en GitHub?

Para crear un pull request en GitHub se siguen los siguientes pasos:

1. Realizar un push de la rama con los cambios al repositorio remoto en GitHub.
2. Ir al repositorio en GitHub y hacer clic en la pestaña **"Pull requests"**.
3. Hacer clic en el botón **"New pull request"**.
4. Seleccionar la **rama base** (la rama donde se quieren integrar los cambios, por ejemplo `develop`) y la **rama de comparación** (la rama con los cambios, por ejemplo `feature/proj-structure`).
5. Revisar los cambios que se van a incluir en el pull request.
6. Agregar un **título** descriptivo y una **descripción** detallada de los cambios realizados.
7. Hacer clic en **"Create pull request"** para enviarlo.

#### f. ¿Cómo se aprueba un pull request en GitHub?

Para aprobar un pull request en GitHub:

1. Ir al repositorio en GitHub y acceder a la pestaña **"Pull requests"**.
2. Seleccionar el pull request que se desea revisar.
3. Revisar los cambios en la pestaña **"Files changed"**.
4. Hacer clic en el botón **"Review changes"**.
5. Seleccionar la opción **"Approve"** y opcionalmente agregar un comentario.
6. Hacer clic en **"Submit review"** para confirmar la aprobación.
7. Una vez aprobado, la persona autorizada puede hacer clic en **"Merge pull request"** para fusionar los cambios en la rama base.

**Nota importante:** El pull request no puede ser aprobado por la misma persona que lo creó.

#### g. Bibliografía

- Apache Maven Project. (s.f.). *Introduction to Archetypes*. Maven. Recuperado el 18 de febrero de 2026, de https://maven.apache.org/guides/introduction/introduction-to-archetypes.html

- Apache Maven Project. (s.f.). *Maven Archetype Plugin – archetype:generate*. Maven. Recuperado el 18 de febrero de 2026, de https://maven.apache.org/archetype/maven-archetype-plugin/generate-mojo.html

- GitHub Docs. (s.f.). *About pull requests*. GitHub. Recuperado el 18 de febrero de 2026, de https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests

- GitHub Docs. (s.f.). *Creating a pull request*. GitHub. Recuperado el 18 de febrero de 2026, de https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request

---

### Comando ejecutado para crear la estructura del proyecto

```bash
mvn archetype:generate -DgroupId=edu.dosw.lab -DartifactId=DOSW-Laboratorio4 -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.5 -DinteractiveMode=false
```