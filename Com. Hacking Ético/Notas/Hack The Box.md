---
aliases:
  - HTB
tags:
  - MOC
web: https://hackthebox.com
---
> [!INFO] Hack The Box
> Plataforma de entramiento en ciberseguridad mediante retos [[CTF]].
> 
> Se trata de **la plataforma más conocida**.
^descripcion

> [!FLAG] Máquinas realizadas
> 
> ```dataview
> TABLE WITHOUT ID
>     file.link AS Nota,
>     dificultad AS Dificultad,
>     dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
> FROM
> 	[[#]] AND
> 	!"00 - Recursos"
> WHERE
> 	plataforma = [[Hack The Box]]
> SORT
> 	file.name ASC
> ```
^maquinas
