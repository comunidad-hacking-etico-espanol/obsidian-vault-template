---
tags:
  - CTF
  - estado/completado
plataforma: "[[OverTheWire]]"
web: https://overthewire.org/wargames/bandit/bandit3.html
dificultad: fácil
autor:
---
# Datos

> [!TODO] Objetivo
> La contraseña para el [[Bandit 04|siguiente nivel]] se almacena en un archivo llamado *spaces in this filename* ubicado en el *home directory* del usuario.
> 
> **Usa esta contraseña para entrar en `bandit3` usando [[SSH]].**
> 
> ---
> 
> Una vez conectado, ve a la página [[Bandit 04]] para averiguar cómo superar ese nivel.
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
> - ["Spaces in filename" buscado en Google](https://www.google.com/search?q=spaces+in+filename)
^recursos

# Resolución

Usando el usuario `bandit2` del [[Bandit 02|ejercicio anterior]]:

```shell
ls
```
```
spaces in this filename
```

Para lograr ver el archivo se puede usar:

- Un **sangrado[^1] en los espacios** del nombre del fichero, para que los espacios sean espacios.
- Todo el nombre entre **comillas dobles (`"`)**, para que sea interpretado literalmente.
- Todo el nombre entre **comillas simples (`'`)**, para que sea interpretado literalmente.

```shell
cat spaces\ in\ this\ filename
cat "spaces in this filename"
cat 'spaces in this filename'
```
```
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
```

> [!INFO] La terminal interpreta los espacios como **separadores de argumentos en los comandos**
> El siguiente comando [[cat]] se ejecutaría 4 veces: una para un fichero *spaces*, otra para *in*, otra para *this* y otra para *filename*:
> ```shell
> cat spaces in this filename
> ```
> ```text
> cat: spaces: No such file or directory
> cat: in: No such file or directory
> cat: this: No such file or directory
> cat: filename: No such file or directory
> ```

Pruebo a conectarme por [[SSH]] usando las siguientes credenciales:

- Usuario: `bandit3`
- Contraseña: `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG`

```shell
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

> [!SUCCESS] La conexión tiene éxito, por lo que la contraseña es correcta

# Bandera

> [!FLAG] `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG`
^bandera

[^1]: Yo le he dicho *sangrado* toda mi vida, pero se refiere al uso de `\` para anular las funcionalidades de los caracteres especiales.
