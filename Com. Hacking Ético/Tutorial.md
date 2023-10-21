# Introducción

Esta nota sirve como guía introductoria al uso de esta bóveda.

> [!IMPORTANT] Lo primero y más importante: las etiquetas #tutorial 
> Estas etiquetas se encuentran repartidas por varias notas de la bóveda, y su función es precisamente, hacer un pequeño comentario a modo de tutorial.
> 
> > Piensa en ellas como el aviso que aparece en algunos videojuegos cuando haces algo por primera vez; y por supuesto, elimínalas cuando te canses de ellas: tu *bóveda final* no debería tener ninguna.

Adicionalmente, puedes consultar estos vídeos sobre el uso de [[Obsidian]] en base a la ciberseguridad:

|                                                                                                                                         Parte I                                                                                                                                         |                                                                                                                                        Parte II                                                                                                                                         |
|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| <iframe width="375" height="257" src="https://www.youtube.com/embed/lmQlrQCa57M?si=Lxi071-KCVejcsdZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe> | <iframe width="357" height="257" src="https://www.youtube.com/embed/J5yd5ZgCedM?si=f13qV5IVDrvY1BhN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe> |

# Flujo de trabajo

## Notas nuevas

> [!INFO] Las notas nuevas se almacenan automáticamente  en `Notas/Procesar/`
> Salvo que se haya creado con uno de los botones del menú ribbon (a la izquierda).
> 
> Más información en el apartado [[#Plantillas]].

Además, puedes observar que existe una carpeta `Notas/`: la intención de dicha carpeta es recoger todas aquellas notas que no pertenezcan a ninguna de las carpetas precedentes (nota de diario, un *writeup*, una persona o un [[Script]]).

Esto se ha planteado así para que las notas no *cuelguen de la raíz* (aunque es un uso más natural).

## Recursos y ficheros multimedia

> [!INFO] Cualquier otro archivo se almacena automáticamente en `00 - Recursos/`
> Actualmente no existe una forma de clasificar un fichero por su extensión, por lo que no es posible automatizar un filtrado de ficheros en las subcarpetas de `00 - Recursos/`.
> 
> Existen subcarpetas (`Imágenes`, `Grabaciones`…) para aquellos usuarios más minuciosos.

Por otra parte, existen las siguientes excepciones que sí son automáticas:

- [[Obsidian Canvas|Canvas de Obsidian]]: `00 - Recursos/Diagramas/Canvas/`
- Diagrama de [[Excalidraw]]: `00 - Recursos/Diagramas/Canvas/Excalidraw/`  

# Plantillas

> [!FAQ] ¿Qué es una plantilla?
> Se trata de una nota con la que poder crear otras notas, replicando su contenido.

Adicionalmente, esta bóveda usa el siguiente esquema:

![[Automatización.excalidraw|700]]

> [!INFO] Las plantillas también están disponibles en el menú ribbon
> El menú de la izquierda, los iconos coloreados.

Se han considerado los siguientes tipos de notas habituales en ciberseguridad.

## Writeups

> [!INFO] Registrar cómo se resolvió un [[CTF]]
> Plantillas: `00 - Recursos/Plantillas/_writeup/*`

> [!WARNING] Existen varias plantillas diferentes
> Todas las plantillas contienen el mismo [[#Contenido|contenido]], pero sus [[#Metadatos|metadatos]] varían según la plataforma a la que pertenezca la máquina.

### Metadatos

|     Nombre     |        Tipo        | Función                                                                        |
|:--------------:|:------------------:|:------------------------------------------------------------------------------ |
| **plataforma** | Texto (`[[Nota]]`) | Vincular el *writeup* a una plataforma<br>*([[TryHackMe]], [[Hack The Box]]…)* |
|   **web** \*   |    Texto (URL)     | Acceder a la web específica del [[CTF]]                                        |
| **dificultad** |       Texto        | Referenciar la dificultad según la plataforma                                  |
|   **autor**    | Texto (`[[Nota]]`) | Vincular el *writeup* a una [[#Persona\|persona]]                              |

\* Solo disponible en las plataformas que ofrecen una página específica para un [[CTF]].

### Contenido

Todas las plantillas de *writeups* cuentan con 4 apartados, correspondiente a las fases habituales de resolución de un [[CTF]].

| Fase                                           | Función                          |
|:---------------------------------------------- |:-------------------------------- |
| :obs_search: Reconocimiento                    | ¿Qué información puedes obtener? |
| :obs_broken_link: Análisis de Vulnerabilidades | ¿Qué vulnerabilidades existen?   |
| :luc_unlock: Explotación                       | ¿Cómo puedes obtener acceso?     |
| :fas_stairs: Escalada de Privilegios           | ¿Cómo puedes ser `root`?         |

## Código

> [!INFO] Registrar cómo se desarrolló un [[Programa|programa]] o [[Script|script]]
> Plantilla: [[_código]]

### Metadatos

|     Nombre      |             Tipo             | Función                                                                |
|:---------------:|:----------------------------:|:---------------------------------------------------------------------- |
|  **lenguajes**  | Lista de texto (`[[Notas]]`) | Vincular el código a sus lenguajes<br>*([[Bash]], [[C]], [[Python]]…)* |
| **repositorio** |         Texto (URL)          | Acceder al repositorio (si lo tiene)<br>_Por defecto: [[GitHub]]_      |

## Contenido

#### Código

Bloque de código ([[Markdown]]) para insertar el código o una parte de él.

- Incluye la referencia `^codigo` para acceder desde otras notas.
	- Por ejemplo: `[[h4_hash-cracker#^codigo]]`.
#### Descripción

Un breve resumen del objetivo y/o funcionamiento del código.

- Incluye la referencia `^descripcion` para acceder desde otras notas.
	- Por ejemplo: `[[h4_hash-cracker#^descripcion]]`.
#### Referencias

Recursos consultados durante la resolución de la máquina.

Por ejemplo: documentación, páginas webs, vídeos…

## Concepto

> [!INFO] Información sobre un concepto o término
> Plantilla: [[_contenido]]

### Metadatos

|   Nombre    |      Tipo      | Función                                                               |
|:-----------:|:--------------:|:--------------------------------------------------------------------- |
| **aliases** | Lista de texto | Nombres alternativos para la nota<br>_Sobre todo si es una **sigla**_ |
|  **tags**   |    Etiqueta    | Caracterizar la nota<br>_Por defecto: #concepto _                     |

### Contenido

#### Definición

- Incluye la referencia `^definicion` para acceder desde otras notas.
	- Por ejemplo: `![[VPN#^definicion]]`
- Si el concepto son siglas, resulta muy útil incluir su significado.
	- Por ejemplo: `> [!INFO] VPN (*Virtual Private Network*)`
#### Un espacio en blanco

- Gestionar información adicional sobre el concepto.
- Crear conexiones con otras notas relacionadas.
- Personalizar este apartado con tus propios apartados.

### Referencias

> Consultar [[#Referencias]].

## Creación de contenido

> [!INFO] Registrar información, ideas y recursos para creación de contenido
> Plantilla: [[_contenido]]

> Si no creas contenido, esta plantilla no te sirve de nada y puedes eliminarla.
> 
> 1. Borrando el icono del menú en el plugin Commander.
> 2. Borrando el comando creado en el plugin QuickAdd.
> 3. Borrando la plantilla.

### Metadatos

|     Nombre     |        Tipo        | Función                                                             |
|:--------------:|:------------------:|:------------------------------------------------------------------- |
| **plataforma** | Texto (`[[Nota]]`) | Vincular la nota con una plataforma<br>*([[Youtube]], [[Twitch]]…)* |

### Contenido

Distintos apartados para el flujo de trabajo habitual de un creador de contenido.

## Diario

> [!INFO] Nota con la que llevar un registro de eventos
> Plantilla: [[_diario]]

> [!TIP] Representa un día
> Esto quiere decir que puede utilizarse con muchos plugins compatibles, normalmente aquellos que involucran calendarios.

Los alias son automáticos y representan la fecha de distintas formas.

- Se recomienda usar el botón  del menú para crear automáticamente la nota diaria.
- Se puede crear una nota de cualquier día con el botón de *Templater* y la plantilla.

### Metadatos

|   Nombre    |      Tipo      | Función                            |
|:-----------:|:--------------:|:---------------------------------- |
| **aliases** | Lista de texto | Mostrar la fecha en otros formatos |

Estos formatos se generan automáticamente y son los siguientes:

- `día`/`mes`/`año`
- `día`-`mes`-`año`
- `día de la semana` y `día`, `mes` de `año`

### Contenido

#### Un espacio en blanco

> Consultar [[#Un espacio en blanco]].

#### Registro de notas

Sección automatizada con las notas creadas ese mismo día.

## [[MOC]]

> [!INFO] Nota que representa un *mapa de conceptos*
> Plantilla: [[_moc]]

### Metadatos

|   Nombre    |      Tipo      | Función                           |
|:-----------:|:--------------:|:--------------------------------- |
| **aliases** | Lista de texto | Nombres alternativos para la nota |
|  **tags**   |    Etiqueta    | Caracterizar la nota              |

### Contenido

#### Descripción

Un breve resumen de lo que consiste el [[MOC]].

#### Conexiones con otras notas

Tabla con otras notas relacionadas con el [[MOC]].

#### Referencias

> Consultar [[#Referencias]]

## Persona

> [!INFO] Nota con información destacada sobre una persona o figura relevante
> Plantilla: [[_persona]]

> [!DANGER] No es recomendable almacenar información personal

La idea original de esta nota es almacenar información pública y profesional de un miembro del sector, como su trayectoria profesional o su currículum, para poder referenciar su trabajo, sus proyectos y sus logros.

### Metadatos

|   Nombre    |      Tipo      | Función                                                               |
|:-----------:|:--------------:|:--------------------------------------------------------------------- |
| **aliases** | Lista de texto | Nombres alternativos para la persona<br>*(motes, nombre de usuario…)* |

### Contenido

#### Introducción

Breve descripción de la persona y datos remarcables.

#### Comunidades

Ya que esta bóveda es un proyecto para [[Comunidad de Hacking Ético|Com. Hacking Ético en Español]], se incluye una sección para otras comunidades.

> Por defecto, aparecen las comunidades:
> 
> - [[Comunidad de Hacking Ético|Com. Hacking Ético]]
> - [[H4ckingPro]]

#### Certificaciones

Una tabla con distintas certificaciones donde se puedan vincular con las `[[notas]]` de dichas certificaciones, así como con el enlace habitual de verificación.

> Se incluyen las certificaciones más habituales: [[eJPT v2]], [[eCPPT v2]] y [[OSCP]].

#### Formación

Dividida en 2 secciones principales:

- Académica: formación reglada y oficial.
- Complementaria: cursos, bootcamps u otra formación adicional.

#### Proyectos

Código [[Open Source|open source]] o trabajos relevantes de la persona.

#### Voluntariado

Colaboraciones no-remuneradas en proyectos mayores.

# Plugins

Qué herramientas vienen pre-configuradas.

![[Directo de Obsidian#^plugins-funciones]]

![[Directo de Obsidian#^plugins-apariencia]]

A continuación se muestran los plugins instalados, su función, y algún detalle adicional sobre su uso en esta bóveda.

> [!TIP] Están ordenados alfabéticamente

## Advanced Tables

Crea y modifica tablas [[Markdown]] de forma mucho más cómoda y eficiente.

También deja el formato mucho más limpio:

```markdown
|                |     CHEE      |         H4          |
|:--------------:|:-------------:|:-------------------:|
| :fab_telegram: | administrador |    administrador    |
| :fab_discord:  | administrador | ayudante (*helper*) |
|  :fab_github:  | administrador |          -          |
```

## Auto Link Title

Sea `[título](url)` el formato de un enlace, genera un título automáticamente basado en el contenido de la [[URL]] que se ha pegado en una nota.


## Commander

Permite asociar comandos de la bóveda a distintos recursos de la [[GUI]] de [[Obsidian]].

- Usa [[#QuickAdd]] para asociar comandos personalizados al menú ribbon (iconos coloridos).

## Dataview

Permite realizar consultas (parecidas a [[SQL]]) sobre la bóveda, lo que permite a su vez generar tablas dinámicas o tablas de [[Base de Datos|bases de datos]] con las notas y sus metadatos.

```sql
TABLE WITHOUT ID
	file.link AS Máquina,
	plataforma AS Plataforma,
	dateformat(date(file.mtime), "ccc dd, LLLL") AS Inicio
FROM
	"02 - Writeups"
LIMIT
	5
SORT
	file.cday DESC
```

- Se usa mucho en los [[MOC|MOCs]] para detectar las notas relacionadas.

## Excalidraw

Crea y modifica diagramas de [[Excalidraw]] desde [[Obsidian]], y úsalo como si fueran notas.

![[Automatización.excalidraw]]

- Se configuró para que tengan la extensión `(...).excalidraw`

## Homepage

Establece un recurso para que se abra siempre al inicio de la bóveda.

- Se configuró para que se abra el diagrama [[INICIO.canvas]]

## Icon Shortcodes

Permite añadir iconos { :obs_folder: :far_circle_dot: :fab_docker: :fab_python: … } y emojis { ⚡ ✍️ 🇪🇸 🕵️‍♂️ } usando `:shortcodes:`.

## Plugin Updates tracker

Comprueba los plugins desactualizados y te permite actualizarlos todos a la vez.

## QuickAdd

Permite crear comandos personalizados para la bóveda.

- Usa [[#Templater]] para crear notas en función de las plantillas existentes.
- Se usa por el comando [[#Commander]] para crear botones en el menú ribbon.

## Quiet Outline

Una versión mejorada del esquema (índice) de una nota.

- Se configuró para aparecer arriba a la izquierda.

## Reading Time

Indica el tiempo aproximado de lectura de una nota, en función de su cantidad de contenido.

Muy útil para saber si una nota es muy corta o muy larga.

## Recent Files

Muestra los archivos modificados recientemente.

- Se ha colocado la pestaña del plugin :luc_clock_4: entre el buscador :obs_search_glyph: y la carpeta :far_folder: de notas.

## Smart Typography

Convierte algunas combinaciones de caracteres en caracteres mejores, para que se lea mejor.

Por ejemplo: al escribir "<=", esto se convierte en '≤'.

- Se ha desactivado la opción de "comillas cursivas", ya que en este contexto, se necesitan las comillas rectas para que sea compatible con código.

## Style Settings

Permite modificar el aspecto o incluso el funcionamiento de algunos temas y plugins.

Este plugin es vital para el funcionamiento de otros (por ejemplo, [[#Supercharged Links]]).

## Supercharged Links

Permite colorear las conexiones (`[[nota]]`) de notas en función de condiciones.

Muy últil para darle una información añadida a una nota, fuera de ella.

- Requiere del plugin [[#Style Settings]] para definir las condiciones y los valores.

## Templater

Permite crear plantillas de notas mejoradas, usando una sintaxis especial de [[JavaScript]].

```javascript
<% tp.file.title %>
```

- Se usa para las [[#Plantillas]] definidas en la bóveda.
- Se usa por el plugin [[#QuickAdd]].

## Vault Statistics

Genera estadísticas de la bóveda (número de notas, espacio ocupado…).

Ideal para los fanáticos de los *numeritos*.

## Workspaces Plus

Una versión mejorada del plugin principal *Workspace*.

- Necesita tener activo el plugin principal *Workspace*.

# Contenido de ejemplo

- [[Mapas HTML]]
  Nota normal con mapas interactivos cargados con `<iframe>` de [[HTML]].

- **[[OverTheWire]] / [[Hack The Box]] / [[TryHackMe]]**
  Notas [[MOC|MOCs]] que contienen conexiones a notas de *writeups*.
  Los *writeups* usan las plantillas: [[_overthewire]], [[_hack the box]] y [[_tryhackme]].

- [[Sr. Galán]] / [[Mr. Wh1t3]]
  Notas [[_persona]] con información relevante sobre sus trayectorias.

> [!TIP] Estas solo son unas pocas notas, ¡pero hay muchas más!
> También hay ficheros de recursos de ejemplo, al menos uno de cada tipo.
