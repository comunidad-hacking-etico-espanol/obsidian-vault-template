---
tags:
  - CTF
  - estado/completado
plataforma: "[[OverTheWire]]"
web: https://overthewire.org/wargames/bandit/bandit01.html
dificultad: fácil
autor:
---
# Datos

> [!TODO] Objetivo
> La contraseña para el [[Bandit 02|siguiente nivel]] se almacena en un archivo llamado *readme* ubicado en el *home directory* del usuario.
> 
> **Usa esta contraseña para entrar en `bandit1` usando [[SSH]].**
> 
> ---
> 
> Una vez conectado, ve a la página [[Bandit 02]] para averiguar cómo superar ese nivel.
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

Usando el usuario `bandit0` del [[Bandit 00|ejercicio anterior]]:

```shell
ls /home/
```
```
bandit0   bandit15  bandit21  bandit27-git  bandit30-git  bandit6    drifter12  drifter5     formulaone2  krypton4
bandit1   bandit16  bandit22  bandit28      bandit31      bandit7    drifter13  drifter6     formulaone3  krypton5
bandit10  bandit17  bandit23  bandit28-git  bandit31-git  bandit8    drifter14  drifter7     formulaone5  krypton6
bandit11  bandit18  bandit24  bandit29      bandit32      bandit9    drifter15  drifter8     formulaone6  krypton7
bandit12  bandit19  bandit25  bandit29-git  bandit33      drifter0   drifter2   drifter9     krypton1     ubuntu
bandit13  bandit2   bandit26  bandit3       bandit4       drifter1   drifter3   formulaone0  krypton2
bandit14  bandit20  bandit27  bandit30      bandit5       drifter10  drifter4   formulaone1  krypton3
```

> [!CITE] Al leer *home directory* en el [[#^objetivo|objetivo]] supuse que se refería al *directorio `/home`*
> Sin embargo, el término *home directory* también puede referirse al *directorio home del usuario*; es decir, al *directorio `/home/usuario/`.*

No veo ningún *readme* en `/home`, probaré a usar [[find]].

```shell
find /home/ -name readme
```

- `-name` especifica el nombre literal que debe tener el archivo (no es [[regex]]).

```
find: ‘/home/bandit29-git’: Permission denied
/home/bandit18/readme
find: ‘/home/drifter6/data’: Permission denied
find: ‘/home/bandit28-git’: Permission denied
find: ‘/home/drifter8/chroot’: Permission denied
find: ‘/home/ubuntu’: Permission denied
/home/bandit0/readme
find: ‘/home/bandit5/inhere’: Permission denied
find: ‘/home/bandit27-git’: Permission denied
find: ‘/home/bandit30-git’: Permission denied
find: ‘/home/bandit31-git’: Permission denied

```

Visto el resultado, asumo que se trata de `/home/bandit0/readme`:

```shell
cat /home/bandit0/readme
```
```
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
```

Pruebo a conectarme por [[SSH]] usando las siguientes credenciales:

- Usuario: `bandit1`
- Contraseña: `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`

```shell
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

> [!SUCCESS] La conexión tiene éxito, por lo que la contraseña es correcta

# Bandera

> [!FLAG] `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`
^bandera
