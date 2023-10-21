# Actividad de CTFs
## Últimos CTFs

```dataview
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

## CTFs pendientes

```dataview
TABLE WITHOUT ID
    plataforma AS Plataforma,
	rows.file.link AS Máquina
FROM
    "02 - Writeups" AND
	!#estado/completado
LIMIT
	5
GROUP BY
    plataforma
SORT
	file.ctime
```

# Uso de notas

## Notas entrantes

Las notas **más mencionadas** en otras notas.

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    length(file.inlinks) AS Conexiones
FROM
    !"00 - Recursos" AND
    !#MOC
LIMIT
	10
SORT
    length(file.inlinks) DESC,
    file.link ASC
```

## Notas salientes

Las notas **que mencionan** más notas.

> [!WARNING] El atributo `file.outlinks` no funciona como se espera

```text
TABLE WITHOUT ID
    file.link AS Nota,
    length(file.outlinks) AS Conexiones,
    file.outlinks
FROM
    !"00 - Recursos"
LIMIT
	10
SORT
    length(file.outlinks) DESC,
    file.link ASC
```

## MOCs

Los [[MOC|MOCs]] **más usados** en la bóveda.

```dataview
TABLE WITHOUT ID
    file.link AS MOC,
    length(file.inlinks) AS Entrantes
FROM
    #MOC 
LIMIT
	10
SORT
    length(file.inlinks) DESC,
    file.link ASC
```


# Registro

## Notas creadas hoy

```dataview
TABLE WITHOUT ID
    file.link AS "Nota",
    dateformat(date(file.ctime), "HH:mm") AS Hora
WHERE
    date(today) = date(file.cday) AND
	!containsword(file.name, ".excalidraw")
LIMIT
	20
SORT
	file.ctime DESC
```


## Últimas modificaciones

```dataview
TABLE WITHOUT ID
    file.link AS "Nota",
    dateformat(date(file.mtime), "ccc dd, LLL (HH:mm)") AS Fecha
LIMIT
	20
WHERE
	!containsword(file.name, ".excalidraw")
SORT
	file.mtime DESC
```
