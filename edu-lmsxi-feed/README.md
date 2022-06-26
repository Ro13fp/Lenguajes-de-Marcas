# README

## Para qué es este repo?

Este repo plantea uno esquema de documentación para realizar un ejercicio de investigación sobre agregadores de contenidos.

## Concreciones sobre especificaciones

### Despliega tu entorno necesario

Simplemente necesitarás un editor de texto plano para editar tu documentación en markdown, una herramienta de captura imágenes de pantalla (nativa en la mayoría de SOs) y si fuese necesario una herramienta de vídeo en forma de gifs animados.

### Documenta tus ejercicios

Existe una carpeta en `doc/` para que documentes todo el proceso de investigación. Emplea la sintaxis [Markdown](https://es.wikipedia.org/wiki/Markdown)

Obtén más detalles en [`doc/README.md`](doc/README.md).

## Ejercicios

Los ejercicios en este caso estarán detallados en el fichero [`doc/Objetivos.md`](doc/Objetivos.md)

## Especificificaciones, consejos y recomendaciones

- Antes de afrontar la tarea debes haber leído y comprendido el contenido de la unidad.
- No tienes porque estudiar toda la unidad para comenzar a realizar la tarea.

## Pre-requisitos

Como requisitos previos se asumen:

- Escritura de documentación en texto plano y con la sintaxis Markdown.
- Nociones básicas de GIT

## Lo que se pretende aprender de este ejercicio

- Documentar un proceso

## Antes de ponerte a trabajar

### Haz un fork del repositorio original

Haz un fork del repositorio original y **configúralo de forma privada** (la actividad propuesta es individual ;)
Habilita las issues y **otorga permisos de escritura al profesor** en tu repo.

### Clona el repositorio en tu máquina de trabajo

```shell
git clone <url de tu fork>
```

### Crea tu rama (personal)de trabajo o release branch

Crea tu propia rama de trabajo! Crea una nueva rama a partir de `master` que se llame como el nombre de tu usuario en el curso (este nombre de usuario se te facilitará en clase). Te recuerdo cómo:

El nombre de usuario para el curso será por defecto nombreApellido1. Utiliza la notación [*lower Camel Case*](https://es.wikipedia.org/wiki/Camel_case). Es decir, es sensible a mayúsculas y minúsculas. La primera debe ser en minúscula!

```shell
git checkout -b <rb-usuario>
```

**Esta será tu *release branch* a partir de ahora.**

La evolución de tu solución final (si no estás trabajando en equipo)deberá estar apuntada por esta rama. Puedes utilizar todas las ramas que quieras, pero **no trabajes en la master** y asegúrate, si tienes otras ramas que forman parte de tu solución, de combinarlas con tu rama con el nombre de tu usuario.

**No modifiques** ningún fichero `README.md`.

### Revisa si se han producido actualizaciones en las especificaciones

Cada vez que retomes tu trabajo asegúrate tener la última versión de las especificaciones. Para ello:

1. (*Sólo la primera vez*) Añade como repo remoto el repo del profesor desde el que has creado tu fork.

    `git remote add profesor <url-repoProfesor>`

2. (C*ada vez que retomes trabajo*) Revisa novedades y obtenlas del repo del profesor

    `git fetch profesor master`

3. (*Cada vez que haya novedades*) Mezcla estas novedades con tu *release branch*. Si has seguido las indicaciones de este README no deberían producirse conflictos. Si se produjesen adviértelo al profesor.

    ```bash
    # Asegúrate primero de estar en tu release branch
    git checkout rb-usuario
    
    # Después mézclate en tu rama actual las novedades
    git merge profesor/master
    ```

## Documenta tu trabajo

El repo debe contener una carpeta nombrada como `doc`. [Sigue las instrucciones](doc/README.md) de cómo documentar.

## Cuándo termines tu trabajo... o eso crees

### Etiqueta tu versión

Cuando tengas un revisión de tu código que consideres estable, etiquétala de la forma que te indique el [mecanismo de versionado](doc/README.md). Modifica tambien el [changelog](doc/changelog.md) indicando las novedades de la versión.
Puedes hacer etiquetado de tu último commit de la siguiente manera:

```git
# Si quieres hacer una etiqueta ligera (solo nombrar un commit
git tag <etiqueta>

# Si quieres hacer una etiqueta que contenga más información
git tag -a <etiqueta> -m 'El mensaje'
```

Si quieres poner una etiqueta a un commit anterior, pon su checksum al final de las instrucciones anteriores.

```git
git tag <etiqueta> <checksum>
```

Recuerda enviar tus tags a tus repos remotos de la siguiente manera:

```git
git push <remoto> <tag>
```

Consulta esta [fuente](https://git-scm.com/book/es/v2/Fundamentos-de-Git-Etiquetado) para más detalles.

## Estrategia de ramificación

Ten en cuenta que no todas las ramas serán facilitadas de inicio. Algunas se irán publicando, otras no.

Rama                    | Uso
------------            | -------------
`master`                | Evolución del enunciado del ejercicio
`test`                  | Evolución de la rama de tests.
`remote\usuario`        | Evolución de la solución de cada alumno
`remote\teamA..B..C`    | Evolución de la solución de cada equipo
`solucionX`             | Rama que representa una solución (puede derivar de master u otra rama)

### Changelog de enunciado

Se irán etiquetando enunciados consolidados y entregados a alumnos. Se dará una explicación general de cada cambio:

Tag                | Descripción
------------       | -------------
`enum-v1`          | Enunciado inicial

### Snapshot actual del enunciado

```Shell
.
├── README.md
└── doc
    ├── Objetivos.md
    ├── README.md
    ├── Work.md
    ├── changelog.md
    └── img
        └── README.md

2 directories, 6 files
```

## Guía de contribuciones

- Propuestas

## Con quien hablo

- Propietario del repo
