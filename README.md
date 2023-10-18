<div textalign="justify">

# Ejercicio Práctico
# Rubén Abreu González
---
1. Crea un repositorio en tu cuenta de Github con el siguiente nombre: ejercicio_git_nombre_alumno, donde nombre_alumno debe de ser tu nombre siguiendo el patrón nombre_apellido1_apellido2. No incluyas el fichero README.md.

2. Realiza la clonación del repositorio creado.
- git clone https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
<details>
<summary>salida</summary>

```
```
</details>

3. Añadir el archivo README al repositorio y realizar el primer commit.
- git touch "REAME.md"
<details>
<summary>salida</summary>

```
```
</details>

- git add .
<details>
<summary>salida</summary>

```
```
</details>

- git commit -m ___"creado el fichero README.md"___
<details>
<summary>salida</summary>

```code
 [main (commit-raíz) 0a9c838] creado el fichero README.md
 1 file changed, 39 insertions(+)
 create mode 100644 README.md
```
</details>

4. Crear una rama con nombre develop.
- git branch develop
<details>
<summary>salida</summary>

```
```
</details>

5. Lista las ramas actuales.
- git branch
<details>
<summary>salida</summary>

```code
 develop
 * main
```
</details>

6. Moverse a la rama y crear el fichero: hola.html. - Añadir el siguiente contenido: 
- git checkout develop
<details>
<summary>salida</summary>

```code
 M	README.md
 Cambiado a rama 'develop'
```
</details>

- nano hola.html
<details>
<summary>salida</summary>

```
```
</details>

- git add .
<details>
<summary>salida</summary>

```
```
</details>

- git commit -m "añadido hola.html"
<details>
<summary>salida</summary>

```code
 [develop b1b7513] añadido hola.html
 1 file changed, 11 insertions(+)
 create mode 100644 hola.html
```
</details>

7. Moverse a la rama principal y crear el fichero adios.html > Sustituye nombre_alumno por tu nombre.
- git checkout main
<details>
<summary>salida</summary>

```code
 M	README.md
 Cambiado a rama 'main'
 Tu rama está basada en 'origin/main', pero upstream ha  desaparecido.
  (usa "git branch --unset-upstream" para arreglar)
```
</details>

- nano adios.html
<details>
<summary>salida</summary>

```
```
</details>

8. Crea el commit con un mensaje descriptivo.
- git add .
<details>
<summary>salida</summary>

```
```
</details>

- git commit -m "añadido adios.html"
<details>
<summary>salida</summary>

```code
 [main a000351] añadido adios.html
 2 files changed, 109 insertions(+), 1 deletion(-)
 create mode 100644 adios.html
```
</details>

9. Sube los cambios a la rama actual.
- git push origin main
<details>
<summary>salida</summary>

```code
    Username for 'https://github.com': rabgonzalez
    Password for 'https://rabgonzalez@github.com': 
    Enumerando objetos: 13, listo.
    Contando objetos: 100% (13/13), listo.
    Compresión delta usando hasta 4 hilos
    Comprimiendo objetos: 100% (12/12), listo.
    Escribiendo objetos: 100% (13/13), 2.10 KiB | 2.10 MiB/s, listo.
    Total 13 (delta 5), reusados 0 (delta 0), pack-reusados 0
    remote: Resolving deltas: 100% (5/5), done.
    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    * [new branch]      main -> main
```
</details>

10. Lista las ramas actuales.
- git branch
<details>
<summary>salida</summary>

```code
  develop
 * main
```
</details>

11. Realizar la mezcla en el repositorio principal.
- git merge develop
<details>
<summary>salida</summary>

```code
 hola.html | 11 +++++++++++
 1 file changed, 11 insertions(+)
 create mode 100644 hola.html
```
</details>

12. Sube los cambios al repositorio a tu cuenta de Github.
- git add .
<details>
<summary>salida</summary>

```
```
</details>

- git commit -m "traemos los cambios de la rama develop a la rama main"
<details>
<summary>salida</summary>

```code
```
</details>

- git push
<details>
<summary>salida</summary>

```code
```
</details>

</div>
