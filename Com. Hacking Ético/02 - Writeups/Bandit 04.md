---
tags:
  - CTF
  - estado/incompleto
plataforma: "[[OverTheWire]]"
web: https://overthewire.org/wargames/bandit/bandit4.html
dificultad: fácil
autor:
---
# Datos

> [!TODO] Objetivo
> La contraseña para el [[Bandit 05|siguiente nivel]] se almacena en un archivo oculto llamado *inhere* ubicado en el *home directory* del usuario.
> 
> **Usa esta contraseña para entrar en `bandit4` usando [[SSH]].**
> 
> ---
> 
> Una vez conectado, ve a la página [[Bandit 05]] para averiguar cómo superar ese nivel.
^objetivo

> [!TIP] Recursos
> **Comandos**
> - [ls](https://man7.org/linux/man-pages/man1/ls.1.html)
> - [cd](https://man7.org/linux/man-pages/man1/cd.1.html)
> - [cat](https://man7.org/linux/man-pages/man1/cat.1.html)
> - [file](https://man7.org/linux/man-pages/man1/file.1.html)
> - [du](https://man7.org/linux/man-pages/man1/find.1.html)
> - [find](https://man7.org/linux/man-pages/man1/find.1.html)
^recursos
# Resolución

Usando el usuario `bandit3` del [[Bandit 03|ejercicio anterior]]:

```shell
ls
```
```text
inhere
```

Sin embargo, *inhere* no es un fichero, **sino un directorio**; y además, **está vacío**.

Ejecutando `ls` con la opción `-a` (`--all`) para el directorio *inhere* se muestran todos los archivos, **incluidos aquellos ocultos**:

```shell
ls -a inhere
```
```text
.  ..  .hidden
```

> [!INFO] Ficheros especiales
> **El *fichero `.`* hace referencia al *directorio actual***
> Por ejemplo, `cd .` te mueve al directorio actual (es decir, no hace nada).
> 
> **El *fichero `..`* hace referencia al *directorio superior***
> Por ejemplo, `cd ..` te mueve al directorio que contiene al directorio actual. 

#todo/completar

# Bandera

> [!FLAG] `flag{B4nd3r4}`
^bandera
