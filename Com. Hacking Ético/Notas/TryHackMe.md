---
aliases:
  - THM
tags:
  - MOC
web: https://tryhackme.com
---
> [!INFO] TryHackMe
> Plataforma de entrenamiento en ciberseguridad mediante retos [[CTF]].
> 
> Se considera **una de las mejores plataformas para empezar**.
^descripcion

> [!FLAG] Máquinas realizadas
> Estos son los últimos [[CTF|retos CTF]] realizados.
> 
> ```dataview
> TABLE WITHOUT ID
>     file.link AS Nota,
>     dificultad AS Dificultad,
>     dateformat(date(file.cday), "ccc dd, LLL. yyyy") AS Inicio
> FROM
> 	[[#]] AND
>     !"00 - Recursos"
> WHERE
> 	plataforma = [[TryHackMe]]
> SORT
> 	file.name ASC
> ```
^maquinas
