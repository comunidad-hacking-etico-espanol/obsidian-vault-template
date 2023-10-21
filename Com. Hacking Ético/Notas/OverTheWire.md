---
aliases: 
tags:
  - "#MOC"
---
> [!INFO] OverTheWire
> Plataforma simple de entrenamiento en ciberseguridad mediante retos [[CTF]].
> 
> Los retos *wargames* se dividen en [[#Niveles de *wargames*|niveles]], y cada nivel cuenta con una serie de retos que deben superarse en orden para poder avanzar entre ellos, hasta terminar el nivel.
^descripcion

# Niveles de *wargames*

## Bandit

Introducción a la [[Terminal|terminal]] de [[Linux]].

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Bandit")
SORT
    file.name ASC
```
^bandit

## Natas

Introducción a la seguridad web.

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Natas")
SORT
    file.name ASC
```
^natas

## Leviathan

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Leviathan")
SORT
    file.name ASC
```
^leviathan

## Krypton

Introducción a la [[Criptografía|criptografía]].

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Krypton")
SORT
    file.name ASC
```
^krypton

## Narnia

Introducción a la [[Exploit|explotación]].

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Narnia")
SORT
    file.name ASC
```
^narnia

## Behemoth

Introducción a las [[Vulnerabilidad|vulnerabilidades]] más comunes.

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Behemoth")
SORT
    file.name ASC
```
^behemoth

## Utumno

Retos un poco más complicados que [[#Behemoth]].

> [!WARNING] Se recomienda haber superado los retos anteriores

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Utumno")
SORT
    file.name ASC
```
^utumno

## Maze

Retos complicados y algunos de ellos también extraños, que requerirán [[GDB|gdb]].

> [!TODO] Conocimientos necesarios
> - [ ] Técnicas de [[Exploit|explotación]]
> - [ ] Programación
> - [ ] [[Reversing]]

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Maze")
SORT
    file.name ASC
```
^maze

## Vortex

Retos relacionados con ficheros de [[C]].

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Vortex")
SORT
    file.name ASC
```
^vortex

## Manpage

Retos que desmitifican algunos conceptos erróneos comunes de programación en [[C]] en [[Linux]].

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Manpage")
SORT
    file.name ASC
```
^manpage

## Drifter

Retos muy relacionados con los de [[#Vortex]].

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "Drifter")
SORT
    file.name ASC
```
^drifter

## FormulaOne

*Sin descripción.*

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    dificultad AS Dificultad,
    dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
FROM
    [[#]] AND
    !"00 - Recursos"
WHERE
    contains(file.name, "FormulaOne")
SORT
    file.name ASC
```
^formulaone
