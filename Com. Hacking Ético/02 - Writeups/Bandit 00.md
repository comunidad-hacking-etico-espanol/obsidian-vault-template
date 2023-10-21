---
tags:
  - CTF
  - estado/completado
plataforma: "[[OverTheWire]]"
web: https://overthewire.org/wargames/bandit/bandit0.html
dificultad: fácil
autor:
---
# Datos

> [!TODO] Objetivo
> **Conectarse al juego usando [[SSH]].**
> 
> El host al que necesitas conectarte es `bandit.labs.overthewire.org`, en el puerto `2220`.
> 
> - Usuario: `bandit0`
> - Contraseña: `bandit0`
> 
> ---
> 
> Una vez conectado, ve a la página del [[Bandit 01]] para averiguar cómo superar ese nivel.

> [!TIP] Recursos
> **Comandos**
> - [ssh](https://man7.org/linux/man-pages/man1/ssh.1.html)
> 
> **Referencias**
> - [Secure Shell (SSH) en Wikipedia](https://en.wikipedia.org/wiki/Secure_Shell)
> - [Cómo usar SSH en WikiHow](https://en.wikipedia.org/wiki/Secure_Shell)
^recursos

# Resolución

> [!SUCCESS] Este comando cumple el [[#^objetivo|objetivo]]
> ```shell
> ssh bandit0@bandit.labs.overthewire.org -p 2220
> ```
