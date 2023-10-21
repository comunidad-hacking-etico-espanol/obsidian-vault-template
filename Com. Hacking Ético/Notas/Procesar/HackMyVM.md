---
aliases: 
tags:
  - "#MOC"
---
> [!INFO] HackMyVM
> Descripción del [[MOC]].
^descripcion

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    tags AS Etiquetas
FROM
    [[#]] AND
    !"00 - Recursos"
SORT
    length(file.inlinks) DESC,
    file.name ASC
```
^conexiones

# Referencias

> #tutorial : recursos interesantes, como fuentes externas de información.
> Se ha incluido un formato de lista vacía (*bullet list*) para que sea minimalista.
> Otra opción es usar la sintaxis `[^id]` para referenciar la información exterior.

- 
- 
