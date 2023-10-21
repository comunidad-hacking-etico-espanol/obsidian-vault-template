---
aliases:
  - Com. Hacking Ético en Español
  - Com. Hacking Ético
  - CHEE
  - HEE
tags:
  - "#MOC"
webs:
  - https://comunidadhackingetico.es
  - https://comunidadhackingetico.es/circular
  - https://ctf.comunidadhackingetico.es/home
---
> [!INFO] Comunidad de Hacking Ético Español
> Comunidad de ciberseguridad en español fundada por [[Mr. Wh1t3|Mr. Wh1t3]].
^definicion

```dataview
TABLE WITHOUT ID
    file.link AS Nota,
    tags AS Etiquetas,
    file.cday AS Creación
FROM
    [[#]] AND
    !"00 - Recursos" AND
    !"02 - Writeups"
SORT
    length(file.inlinks) DESC,
    file.name ASC
```
^conexiones

# Proyectos

## Iniciativa CTF

<iframe src="https://ctf.comunidadhackingetico.es/home" width="700" height="500"></iframe>

> [!INFO] [ctf.comunidadhackingetico.es](https://ctf.comunidadhackingetico.es/home)
> Página web de [[CTF|retos CTF]] pública y gratuita, donde los miembros pueden publicar sus propios retos para que sean resueltos por otros usuarios.

> [!FLAG] Progreso de los retos
> ```dataview
> TABLE WITHOUT ID
>     file.link AS Máquina,
> 	dificultad AS Dificultad
> FROM
> 	"02 - Writeups" 
> WHERE
> 	plataforma = [[Comunidad de Hacking Ético]]
> SORT
> 	file.name ASC
> ```

# Recursos

<iframe src="https://discord.com/widget?id=544877010783174656&theme=dark" width="350" height="500" allowtransparency="true" frameborder="0" sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"></iframe>

^vista-discord
