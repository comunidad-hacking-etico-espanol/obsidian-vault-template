# Ciberseguridad & [[Obsidian]]

Hecho con ⚡ por [[Sr. Galán]]

---

## Ciberseguridad

|           Un proceso constante           |
|:----------------------------------------:|
| Disciplina, autosuperación, no rendirse… |

---

> [!BUG] No es posible memorizarlo todo

> [!FAQ] ¿Cuántas veces ha pasado?
> - "¡Ah! Esto se parece, ¿cómo era?"
> - "No me recuerdo cómo lo hice"
> - "Creo que he borrado el archivo"
> - "…"

---

Tu **cerebro** es genial para *producir ideas*<br>Sin embargo, es bastante **torpe** para *recordarlas*

---

## [[Obsidian]]

|    La *parte teórica* de la ciberseguridad    |
|:---------------------------------------------:|
| Apuntes, ideas, trucos, experiencias… |

---

### La aplicación

<img src="https://obsidian.md/images/screenshot-1.0-hero-combo.png" height=400>

|        |        |          |            |
|:------:|:------:|:--------:|:----------:|
| Simple | Ligera | Flexible | Extensible |

---

### Servicios oficiales

| [[Obsidian Sync\|Sync :obs_sync_small:]] | [[Obsidian Publish\|Publish :luc_globe:]] |
|:----------------------------------------:|:-----------------------------------------:|
|         sincronizar<br>compartir         |           publicar<br>colaborar           |

---

> [!INFO] [[Obsidian Sync]]
> - **Sincronizar** tus bóvedas *automágicamente*.
> - **Compartir** bóvedas con otros usuarios.

- Encriptación punto a punto
- Historial de versiones
- Multiplataforma
- Trabajar offline, sincronizar después

---

> [!WARNING] Todos deben usar [[Obsidian Sync|Sync]] para compartir

<img src="https://obsidian.md/images/sync-share-dark.png" height=500>

---

> [!INFO] [[Obsidian Publish]]
> **Publicación de notas** en un sitio web.
> - **Colaboración** con otros usuarios.

|                           Características                            |                                      Personalización                                       |
|:--------------------------------------------------------------------:|:------------------------------------------------------------------------------------------:|
| Miniaturas de notas<br>Vista de grafo<br>Páginas apiladas<br>Enlaces | Temas ([[CSS\|:fab_css3_alt:]] y [[JavaScript\|:fab_js_square:]])<br>Dominio personalizado<br>Protección con contraseña |

---

La página de ayuda de [[Obsidian]] usa [[Obsidian Publish|Publish]]:

<img src="https://obsidian.md/images/publish-example-dark.png" height="400">

---

Los cambios se actualizan bajo petición.

<img src="https://obsidian.md/images/publish-experience.png" height=400>

---

### Conceptos clave

| :obs_bracket_glyph: | :obs_redo_glyph: | :obs_hashtag: | :obs_folder: |
|:-------------------:|:----------------:|:-------------:|:------------:|
|     conexiones      |      alias       |   etiquetas   |   carpetas   |

---

> [!INFO] Conexión `[[...]]`
> Enlaces entre 2 o más notas.
> **[[Obsidian]] gira entorno a las conexiones.**

- Simulan el **funcionamiento del cerebro**
- No se necesitan carpetas

---

Las conexiones de este directo:

![[Grafo del Directo de Obsidian.png|500]]

---

> [!INFO] Alias `[[...|...]]`
> Un nombre alternativo para una nota.
> Se pueden definir como *propiedad*.

- Viene genial para las **siglas**

---

> [!INFO] Etiqueta `#...`
> Palabra clave o término para categorizar notas.
> Se pueden definir como *propiedad*.

- Suelen representar **estados**

---

Ejemplo de alias y etiquetas:

![[Concepto de Base de Datos.png]]

![[Concepto de VPN.png]]

---

> [!INFO] Carpeta

- [[Obsidian]] **no se organiza en carpetas**
- Almacenar multimedia (`Adjuntos/`)
- Organización temática (`XYZ - Carpeta/`)
- Proyectos / tareas

---

Ejemplo de carpetas (las mías):

![[Carpetas.png]]

---

#### Información adicional

---

¿Qué trabaja [[Obsidian]]?

| Contenido | Formatos                                             |
|:---------:| ---------------------------------------------------- |
|   Texto   | `md`                                                 |
|  Imagen   | `png`, `webp`, `jpg`, `jpeg`,<br>`gif`, `bmp`, `svg` |
|   Audio   | `mp3`, `webm`, `wav`, `m4a`,<br>`ogg`, `3gp`, `flac` |
|   Vídeo   | `mp4`, `webm`, `ogv`, `mov`, `mkv`                   |
| Documento | `pdf`                                                |
^recursos

---

¿Cómo trabaja [[Obsidian]]?

![[HTML Markdown Obsidian.excalidraw]]

---

### Casos de uso para la ciberseguridad

|    Cómo gestionar notas de ciberseguridad     |
|:---------------------------------------------:|
| Descripciones, procesos, writeups, proyectos… |

---

#### [[Obsidian]] como [[Caché|caché]]

Antes de buscarlo *otra vez* en [[Internet]], puede ser mejor buscarlo en **tu memoria** y con **tus palabras**

---

La ciberseguridad requiere consultar en [[Internet]]

![[Internet.excalidraw]]

> [!WARNING] Normalmente, **la información es independiente**
> - Se encuentra en distintas fuentes
> - Eres tú mismo el que la relaciona

---

Guarda esa información en tu bóveda

![[Internet a Obsidian.excalidraw]]

> [!NOTE] Procesar la información generará conexiones
> - Refuerzan la memoria
> - Producen conocimiento

---

Si olvidas algo, ¿dónde será más fácil encontrarlo?

| [[Internet]]                                                                                    | [[Obsidian]]                                                                               |
| ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| :luc_history: historial<br>:luc_bookmark: marcadores<br>:luc_text_cursor_input: autocompletado… | :luc_database: tu memoria<br>:luc_repeat: tu sistema de notas<br>:luc_map: tus conexiones… |
| **100 % online**                                                                                | **100 % offline**                                                                          |

> [!TIP] [[Obsidian]] es más rápido, **porque ya lo conoces**

---

#### Atomicidad

![[Atomicidad.excalidraw]]

---

#### Perfeccionismo

El objetivo de **tomar notas** *no es* **tomar notas**

---

### [[Plugin|Plugins]] relevantes

---

#### Internos

| Las "funcionalidades" de [[Obsidian]]                                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| :luc_layout_dashboard: [[Obsidian Canvas\|Canvas]]<br>:obs_presentation: Diapositivas<br>:obs_link: Enlaces entrantes y salientes<br>:obs_workspace_glyph: Espacios de trabajo<br>:obs_microphone: Grabadora de audio<br>:luc_file_text: Plantillas |

---

##### Ejemplos

![[confesión.webm]]

![[error win-xp.mp3]]

|                    |                     |     |
| ------------------ | ------------------- | --- |
| ![[INICIO.canvas]] | ![[Ejemplo.canvas]] |     |

---

#### Externos

|                                                                                                                                                                                   |                                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| :luc_table: Advanced Tables<br>:luc_pen_tool: Excalidraw<br>:luc_home: Homepage<br>:obs_reading_glasses: Reading Time<br>:luc_history: Recent Files<br>:fas_plug: Updates Tracker | :obs_gear: Style Settings<br>:obs_code_glyph: Templater<br>:fas_asterisk: Commander<br> :obs_plus_with_circle: QuickAdd<br>:obs_workspace_glyph: Workspace Plus<br>:luc_bar_chart_2: Vault Statistics |
^plugins-funciones

---

Adicionalmente, para mejorar la apariencia:

|                                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| :luc_text_cursor_input: Auto Link Title<br>:fas_icons: Icon shortcodes<br>:luc_menu: Quiet Outline<br>:luc_type: Smart Typography<br>:luc_link_2: Supercharged Links |
^plugins-apariencia

---

## La "Competencia"

|                    ¿Por qué [[Obsidian]]?                    |
|:------------------------------------------------------------:|
| Puntos fuertes y puntos débiles<br>contra otras herramientas |

---

> [!DANGER] [[Obsidian]] no es la herramienta definitiva
> Ninguna herramienta lo es.

Se está enfocando [[Obsidian]] a la<br>**gestión de conocimiento**

---

#### [[CherryTree]]

|            | [[Obsidian]]       | [[CherryTree]]    |
|:----------:| ------------------ | ----------------- |
| Aplicación | Gestión de notas   | Gestión de notas  |
|  Enfoque   | Notas y conexiones | Notas y jerarquía |
|   Coste    | Gratis             | Gratis            |

---

|                 | [[Obsidian]] | [[CherryTree]] |
|:---------------:| ------------ | -------------- |
|  Colaboración   | Baja         | Ninguna        |
| Personalización | Muy alta     | Baja           |
|    Velocidad    | Rápida       | Rápida         |

---

> [!INFO] [[Obsidian]], la opción moderna
> Puedes hacer fluir tus ideas y darles forma.

> [!INFO] [[CherryTree]], más *old school*
> No aporta nada que no aporte [[Obsidian]].

---

#### [[Notion]]

|            | [[Obsidian]]       | [[Notion]]             |
|:----------:|:------------------ |:---------------------- |
| Aplicación | Gestión de notas   | Suite de productividad |
|  Enfoque   | Notas y conexiones | Páginas y jerarquía    |
|   Coste    | Gratis             | *Freemium*             |

---

|                 | [[Obsidian]] | [[Notion]]    |
|:---------------:|:------------ |:------------- |
|  Colaboración   | Baja         | Media-alta    |
| Personalización | Muy alta     | Baja-media    |
|    Velocidad    | Rápida       | A veces lenta |

---

> [!INFO] [[Obsidian]], un lienzo en blanco
> Puedes hacer fluir tus ideas y darles forma.

> [!INFO] [[Notion]], una gran caja de LEGO
> Puedes construir prácticamente de todo,<br>pero debes usar bloques.

---

## Metodologías PKM

---

> [!INFO] [[PKM]] (_**P**ersonal **K**nowledge **M**anagement_)

Metodologías cuyo objetivo es<br>**describir el mejor sistema** para:

1. :luc_eye: Capturar
2. :obs_pencil: Escribir
3. :fas_gears: Procesar
4. :fas_project_diagram: Organizar
5. :luc_repeat: **Usar**

---

> [!INFO] [[MOC]] (_**M**ap **O**f **C**oncepts_)

Una nota cuyo objetivo es referenciar otras notas.

- Suele usarse para agrupar notas con temas parecidos
- En otras palabras: como carpeta

---

### P.A.R.A

**P**royectos, **A**reas, **R**ecursos, **A**rchivados

Se basa en **eliminar las indecisiones** a la hora de gestionar tu información.

---

![[PARA cocina.png]]

---

### Zettelkasten

Colección de **notas atómicas**, integradas y enlazadas, de varias fuentes de información.

---

![Zettel](https://imgs.search.brave.com/YglI_Vaj35Jrdm_cHU-iK5QgBLSWKhbEYtvH8JQd49c/rs:fit:860:0:0/g:ce/aHR0cHM6Ly9pMC53/cC5jb20vY29sYWJv/cmF0b3Jpby5uZXQv/d3AtY29udGVudC91/cGxvYWRzLzIwMjAv/MDYvWmV0dGVsa2Fz/dGVuX3BhcGVyX3Nj/aGVtYXRpYy5wbmc_/cmVzaXplPTY0MCw0/ODAmc3NsPTE)

---

## Preguntas

---

> [!FAQ] ¿Usaste [[Obsidian]] como un 2º cerebro digital?
> Muchas veces se habla de tomar notas/apuntes, pero pocas se habla del **gran potencial** que tiene esta aplicación para ayudarte a ***organizar* tu cerebro** en distintos campos de tu vida.
> 
> \- *4k4m1m3*

---

No solo lo he usado,<br>sino que **lo estoy usando**

---

> [!FAQ] ¿Alguna vez has conectado tu bóveda con aplicaciones de terceros?
> Por ejemplo, tengo entendido que podría implementarse un calendario en [[Obsidian]], que no sea únicamente de [[Obsidian]], como [[Google Calendar]].
> 
> \- *[[RiJaba1]]*

---

Actualmente tengo conectado [[Wakatime]]

---

Además de **tomar notas** y **guardar información**:

> [!FAQ] ¿[[Obsidian]] puede ayudarnos a estudiar de alguna manera? 
> Si es así, ¿cuáles serían las mejores formas?
> 
> \- *Race_Bannon*

---

- **Nota aleatoria**
- Revisar *notas pendientes*
- Repetición espaciada + **Tarjetas Anki**

---

> [!FAQ] ¿Cómo gestionar las copias de seguridad?
> - Comprimir la bóveda
> - Sincronización con terceros
> - Plugin(s) especializado(s)
> - (…)
> 
> \- *[[RiJaba1]]*

---

Todo se resume en<br>**cómo almacenar una carpeta**

|                               |                                                                                                                               |
|:-----------------------------:|:----------------------------------------------------------------------------------------------------------------------------- |
| Local<br>Remoto<br>[[Plugin]] | Comprimir la bóveda (+ contraseña)<br>Usar un repositorio ([[GitHub]], [[GitLab]]…)<br>Usar *Obsidian Git* con un repositorio |

---

Mi sistema:

|       Herramienta       | Objetivo                        |
|:-----------------------:|:------------------------------- |
| [[Obsidian Sync\|Sync]] | *Sincronizar* mi bóveda         |
|         [[Git]]         | *Crear* las copias de seguridad |
|       [[GitHub]]        | *Almacenar* copias de seguridad |

---

> [!FAQ] ¿Qué aconsejas para integrar eficazmente fuentes externas de información?
> \- *[[RiJaba1]]*

---

- Una **gestión adecuada de enlaces** (nota)
- Un **apartado *Referencias***  (`# Referencias`)
- Usar ***footnotes*** en las notas (`[^1]`)

---

> [!FAQ] ¿Hay alguna forma de *añadir* un sitio web o documento de manera más **profesional**?
> Podría ser útil para conectar **parte de ese documento** entre notas o tareas.
> 
> \- *[[RiJaba1]]*
^pregunta

---

Enlazar [[#^recursos|recursos compatibles]]:

| Recurso |  [[Markdown]]   | [[Obsidian]]  |
|:-------:|:---------------:|:-------------:|
| Normal  | `[id](fuente)`  | `[[fuente]]`  |
| Anidado | `![id](fuente)` | `![[fuente]]` |

> [!TIP] También se puede usar `<iframe>` de [[HTML]]

---

```html
<iframe src="https://ctf.comunidadhackingetico.es/home" width="900" height="500"></iframe>
```

<iframe src="https://ctf.comunidadhackingetico.es/home" width="900" height="500"></iframe>

---

También es posible anidar contenido de una nota en otra usando las referencias (`^bloque`).

![[#^pregunta]]

> [!FAIL] No es posible extraer fragmentos de [[PDF|PDFs]]

---

> [!FAQ] ¿Qué tal la seguridad de la información en [[Obsidian]]? ¿Conoces algún fallo?
> - _Race_Bannon_

---

[[Obsidian]] es completamente **local**, por lo que estará **tan protegida como tu dispositivo**

> [!DANGER] Existen [[Vulnerabilidad|vulnerabilidades]] conocidas entre 2021 y 2023
> - [>] [CVEdetails.com](https://www.cvedetails.com/vulnerability-list/vendor_id-25830/Obsidian.html)

---

> [!FAQ] ¿Cómo podemos evitar las fugas de datos?
> \- *Race_Bannon*

---

- Usar varias bóvedas

---

## Muchísimas gracias

![[qrcode2.png|250]]

Mi contacto
