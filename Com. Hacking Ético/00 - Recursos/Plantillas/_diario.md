---
aliases:
  - <% tp.date.now("DD/MM/YYYY", 0, tp.file.title, "YYYY-MM-DD") %>
  - <% tp.date.now("DD-MM-YYYY", 0, tp.file.title, "YYYY-MM-DD") %>
  - <% tp.date.now("dddd DD, MMMM YYYY", 0, tp.file.title, "YYYY-MM-DD") %>
---
> #tutorial : anotaciones para el día de hoy.
> Se incluye un espacio en blanco para que el usuario use el formato que quiera.

# Registro

> [!SUCCESS] Notas creadas el día *<% tp.date.now("dddd DD, MMMM YYYY", 0, tp.file.title, "YYYY-MM-DD") %>*
> ```dataview
> TABLE WITHOUT ID
>     file.link AS "Nota",
>     dateformat(date(file.ctime), "HH:mm") AS Hora
> WHERE
>     date(this.file.name) = date(file.cday) AND
>     this.file.name != file.name
> SORT file.cday DESC
> ```
^registro
