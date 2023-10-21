---
lenguajes: "[[Python]]"
repositorio: https://github.com/15Galan/h4_hash-cracker
---
```python
#!/bin/env python3.9

import sys

from src import input
from src import cracker


def main():
    """
    Función principal del programa.
    """
    args = input.get_args()
	
    if args['hashes_ko']:
        print('Hashes inválidos:')
        print('\n'.join(args['hashes_ko']), end='\n\n')
		
    if args['algorithms_ko']:
        print('Algoritmos inválidos:')
        print(', '.join(args['algorithms_ko']), end='\n\n')
		
    if args['hashes_ok'] or args['algorithms_ok']:
        cracked = cracker.crack(args['hashes_ok'], args['algorithms_ok'], args['words'])
		
        if cracked is None:
            print('No se obtuvo ninguna coincidencia usando esa wordlist.')


if __name__ == '__main__':
    """
    Punto de entrada al ejecutarse como programa.
    """
    try:
        main()
		
    except KeyboardInterrupt:
        pass
		
    except Exception as e:
        print(e, file=sys.stderr)
        exit(1)
		
    exit(0)
```
^codigo

# Descripción

Este es un programa orientado a la obtención de elementos a partir de [[Hash|hashes]].

- Programa desarrollado como formación en [[H4ckingPro]].

> [!WARNING] Esto solo es un ejemplo de nota, el código está incompleto
> #tutorial : solo se muestra el fichero principal `main.py`.

## Argumentos

El proyecto funciona con **4 tipos de argumentos distintos**, pero si no se proporciona ninguno, su comportamiento por defecto es mostrar la ayuda (equivalente a `./main.py -h`).

> [!INFO] Los argumentos `-hl` y `-hf` son compatibles entre sí
>  De hecho, cumplen la misma función: **definir los [[Hash|hashes]] para [[Cracking|crackear]]**.
>  Si se proporcionan ambos, se combinarán en un único dato.

### `-hl` / `--hashlist`

El programa recibe una una **lista de [[Hash|hashes]]** como argumento de entrada y comprueba que haya al menos un [[Hash|hash]] válido para poder operar.

Si todo es correcto, se procederá a intentar [[Cracking|crackear]] cada [[Hash|hash]] válido de la lista.

### `-hf` / `--hashfile`

El programa recibe un **fichero de texto con [[Hash|hashes]]** como argumento de entrada y comprueba que el fichero sea accesible y que haya al menos un [[Hash|hash]] válido para poder operar.

Si todo es correcto, se procederá a intentar [[Cracking|crackear]] cada [[Hash|hash]] válido de la lista.

### `-ag` / `--algorithms`

El programa recibe una **lista de [[Algoritmo|algoritmos]]** como argumento de entrada y comprueba que haya al menos un algoritmo válido para poder operar.

Si todo es correcto, se procederá a intentar [[Cracking|crackear]] cada [[Hash|hash]] válido de los argumentos anteriores con cada algoritmo válido de la lista.

### `-wl` / `--wordlist`

El programa recibe un **fichero de texto con posibles valores de un [[Hash|hash]]** como argumento de entrada y comprueba que el fichero sea accesible y tenga contenido.

Si todo es correcto, se procederá a intentar [[Cracking|crackear]] cada [[Hash|hash]] válido de los argumentos anteriores con cada algoritmo válido de los argumentos anteriores y cada posible valor del archivo.

# Ejemplo de uso

```bash
./app/main.py -hl 1D616F28163414582BA7E2EB400485B9 d616f28163414582ba7e2eb400485b9 c06ed8affb5cdfab49fd531429fe1929 358169735b397d125511972057478501 2378648237 32485725dshjfg -hf hashes.txt -ag md5 md8 sha1 MD5 sha420 sha256 -wl h4ckingyou.txt
```

```text
Hashes inválidos:
d616f28163414582ba7e2eb400485b9
2378648237
32485725dshjfg

Algoritmos inválidos:
md8, sha420

Hashes válidos:
1d616f28163414582ba7e2eb400485b9 : srgalan  (md5)
358169735b397d125511972057478501 * no encontrado
7b4bf604ff3032c625532a803eaedddc : H4CKINGPRO   (md5)
c06ed8affb5cdfab49fd531429fe1929 : sleepy_rafa  (md5)
e772e0266541435a1b52df6bb498cb62e6749c95e59b580d71c9fb16b4125af9 : srgalan  (sha256)
```
