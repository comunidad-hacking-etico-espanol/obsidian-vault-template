---
tags:
  - CTF
  - estado/completado
plataforma: "[[OverTheWire]]"
web: https://overthewire.org/wargames/bandit/bandit2.html
dificultad: fácil
autor:
---
# Datos

> [!TODO] Objetivo
> La contraseña para el [[Bandit 03|siguiente nivel]] se almacena en un archivo llamado *-* ubicado en el *home directory* del usuario.
> 
> **Usa esta contraseña para entrar en `bandit2` usando [[SSH]].**
> 
> ---
> 
> Una vez conectado, ve a la página [[Bandit 03]] para averiguar cómo superar ese nivel.
^objetivo

> [!TIP] Recursos
> **Comandos**
> - [ls](https://man7.org/linux/man-pages/man1/ls.1.html)
> - [cd](https://man7.org/linux/man-pages/man1/cd.1.html)
> - [cat](https://man7.org/linux/man-pages/man1/cat.1.html)
> - [file](https://man7.org/linux/man-pages/man1/file.1.html)
> - [du](https://man7.org/linux/man-pages/man1/find.1.html)
> - [find](https://man7.org/linux/man-pages/man1/find.1.html)
>   
> **Referencias**
> - ["Dashed filename" buscado en Google](https://www.google.com/search?q=dashed+filename)
> - [Guía Avanzada de Bash-Scripting - Capítulo 3 - Caracteres especiales](https://tldp.org/LDP/abs/html/special-chars.html)
^recursos

# Resolución

Usando el usuario `bandit1` del [[Bandit 01|ejercicio anterior]]:

```shell
ls
```
```
-
```

Efectivamente, **hay un fichero llamado *-* en el directorio `home` del usuario**.

Sin embargo, sucede que al realizar cualquiera de estos comandos, el proceso se queda "colgado":

```shell
ls -
cat -
file -
```

> [!FAQ] ¿Por qué ocurre esto?
> Como **el guión (`-`) es un carácter especial**, la consola lo interpreta como algo especial.
> 
> Los comandos interpretan `-` como:
> - Una **opción** (*flag*, filtro…).
> - Un **prefijo** (un operador como `-eq`, `-ot`…).
> - Una **redirección** desde/hasta [[stdin]] o [[stdout]].
> - El **directorio de trabajo anterior**.

Para lograr ver el archivo se puede usar una **redirección** para enviarle a [[cat]] el *fichero -*:

```shell
cat < -
```
```
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi
```

Pruebo a conectarme por [[SSH]] usando las siguientes credenciales:

- Usuario: `bandit2`
- Contraseña: `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi`

```shell
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

> [!SUCCESS] La conexión tiene éxito, por lo que la contraseña es correcta


# Bandera

> [!FLAG] `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi`
^bandera
