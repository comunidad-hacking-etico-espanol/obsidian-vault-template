---
aliases:
  - H4
tags:
  - MOC
webs:
  - https://h4cking.pro
---
> [!INFO] H4ckingPro
> Proyecto de formación gratuita en ciberseguridad creado por [[Moluma]].
^definicion

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    tags AS Etiquetas
FROM
    [[#]]
SORT
    length(file.inlinks) DESC,
    file.name ASC
```
^conexiones

# Sesiones 2023

```dataview
TABLE WITHOUT ID
    file.link AS Sesión,
    fecha AS Fecha
WHERE
    plataforma = [[H4ckingPro]]
SORT
    fecha ASC
```
^sesiones
