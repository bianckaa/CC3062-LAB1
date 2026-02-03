## Bandit Level 0
**Objetivo:**  
Encontrar la contraseña del siguiente nivel.
**Comandos utilizados:**
```bash
ls 
cat readme
```

## Explicación:
Se listaron los archivos y se abrió el archivo readme para ver cual era la contraseña. 

## Contraseña obtenida:
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

## Bandit Level 1
**Objetivo:**  
Encontrar la contraseña del siguiente nivel.
**Comandos utilizados:**
```bash
ls 
cat ./-
```

## Explicación:
Se listaron los archivos y se abrió el archivo con nombre - utilizando una ruta relativa (./-)

## Contraseña obtenida:
263JGJPfgU6LtdEvgfWU1XP5yac29mFx

## Bandit Level 2
**Objetivo:**  
Encontrar la contraseña del siguiente nivel.
**Comandos utilizados:**
```bash
ls 
cat ./--spaces\ in\ this\ filename--
```

## Explicación:
Se listaron los archivos y se abrió el archivo con nombre --spaces in this filename-- utilizando una ruta relativa (./--spaces\ in\ this\ filename--) para que el comando cat no lo malinterpretará

## Contraseña obtenida:
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

## Bandit Level 3
**Objetivo:**  
Encontrar la contraseña del siguiente nivel.
**Comandos utilizados:**
```bash
ls 
cd inhere
ls -al
cat ...Hiding-From-You
```

## Explicación:
Se listaron los archivos ocultos y se abrió el archivo con nombre ...Hiding-From-You 

## Contraseña obtenida:
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

## Bandit Level 4
**Objetivo:**  
Encontrar la contraseña del siguiente nivel.
**Comandos utilizados:**
```bash
ls -alps
cd inhere/
ls
find . -type f | xargs file
cat ./-file07
```

## Explicación:
Se listaron los archivos del directorio inhere y se usó el comando file para identificar el único archivo con contenido ASCII. Luego se leyó este archivo (-file07) usando una ruta relativa para evitar que fuera malinterpretado. 

## Contraseña obtenida:
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

## Bandit Level 5
**Objetivo:**  
Encontrar la contraseña del siguiente nivel.
**Comandos utilizados:**
```bash
ls 
cd inhere/
ls
find . -type f -size 1033c ! -executable
 cat ./maybehere07/.file2
```

## Explicación:
Se ingresó al directorio indicado y se realizó una búsqueda de archivos según su tamaño y permisos, identificando el archivo correcto para luego acceder a su contenido y obtener la contraseña.

## Contraseña obtenida:
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

## Bandit Level 6
**Objetivo:**  
Encontrar la contraseña del siguiente nivel.
**Comandos utilizados:**
```bash
find / -type f -user bandit7 -group bandit6 -size 33c
cat /var/lib/dpkg/info/bandit7.password
```

## Explicación:
Se realizó una búsqueda en todo el sistema para localizar un archivo que cumpliera con condiciones específicas de usuario, grupo y tamaño. Una vez identificado el archivo correcto, se accedió a su contenido.

## Contraseña obtenida:
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

## Bandit Level 7
**Objetivo:**  
Encontrar la contraseña del siguiente nivel.
**Comandos utilizados:**
```bash
ls -alps
strings data.txt | grep "millionth"
```

## Explicación:
Se analizó un archivo de gran tamaño para extraer texto y se filtró la información hasta encontrar la línea que contenía la contraseña.

## Contraseña obtenida:
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

## Bandit Level 8
**Objetivo:**  
Encontrar la contraseña del siguiente nivel.
**Comandos utilizados:**
```bash

```

## Explicación:
Se analizó un archivo con muchas líneas repetidas y se identificó la única línea que aparecía una sola vez, la cual es la que contenía la contraseña.

## Contraseña obtenida:
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM