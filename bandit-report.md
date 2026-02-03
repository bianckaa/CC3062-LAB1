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