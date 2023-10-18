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

```
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
```
</details>

</div>
