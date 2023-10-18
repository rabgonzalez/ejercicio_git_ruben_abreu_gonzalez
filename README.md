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
 [main ce8b298] traemos los cambios de la rama develop  a la rama main
 1 file changed, 65 insertions(+)
```
</details>

- git push
<details>
<summary>salida</summary>

```code
Username for 'https://github.com': rabgonzalez
Password for 'https://rabgonzalez@github.com': 
Enumerando objetos: 12, listo.
Contando objetos: 100% (12/12), listo.
Compresión delta usando hasta 4 hilos
Comprimiendo objetos: 100% (8/8), listo.
Escribiendo objetos: 100% (8/8), 1.62 KiB | 1.62 MiB/s, listo.
Total 8 (delta 1), reusados 0 (delta 0), pack-reusados 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
   a9f0ec2..ce8b298  main -> main
```
</details>

13. Muestra todos los cambios realizados.
- git diff
<details>
<summary>salida</summary>

```code
    diff --git a/README.md b/README.md
    index 82bae28..b6b672e 100644
    --- a/README.md
    +++ b/README.md
    @@ -198,6 +198,8 @@
    <summary>salida</summary>
    
    ```code
    + [main ce8b298] traemos los cambios de la rama develop  a la rama main
    + 1 file changed, 65 insertions(+)
    ```
    </details>
    
    @@ -205,6 +207,26 @@
    <details>
    <summary>salida</summary>
    
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Enumerando objetos: 12, listo.
    +Contando objetos: 100% (12/12), listo.
    +Compresión delta usando hasta 4 hilos
    +Comprimiendo objetos: 100% (8/8), listo.
    +Escribiendo objetos: 100% (8/8), 1.62 KiB | 1.62 MiB/s, listo.
    +Total 8 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +   a9f0ec2..ce8b298  main -> main
    +```
    +</details>
    +
    +13. Muestra todos los cambios realizados.
    +- git diff
    +<details>
    +<summary>salida</summary>
    +
```
</details>

14. Lista ahora los últimos cambios que se han producido en el repositorio, es decir, los últimos commits que han realizado en el repositorio.
- git log
<details>
<summary>salida</summary>

```code
    commit ce8b2980d70366c05a4af8a1bb28b6e94458089c (HEAD -> main, origin/main)
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:32:00 2023 +0100

        traemos los cambios de la rama develop a la rama main

    commit 1ac2997985b24f091db7a1828231526053fb4747
    Merge: a9f0ec2 b1b7513
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:29:11 2023 +0100

        mezclamos las ramas Merge branch 'develop'

    commit a9f0ec2ce2514039a2afca48aedafd64f605b571
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:25:06 2023 +0100

        subimos los cambios

    commit b1b7513e00a5de250959875dc6cc3cc424f04459 (develop)
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:22:40 2023 +0100

        añadido hola.html

    commit b1d417305b7e0ffc30aa04ab29f0a0aee04039ae
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:21:33 2023 +0100

        añadido adios.html

    commit a000351cfa8b2d7e639439cf3b26c9d94023bb2b
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:20:53 2023 +0100

        añadido adios.html

    commit 0a9c838f20c5b8076f2d11dba4086b3df33dcfa1
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:05:10 2023 +0100

        creado el fichero README.md
```
</details>

15. Lista todos los tags(etiquetas que existan).
- git tag
<details>
<summary>salida</summary>

```
```
</details>

> Nota: todavía no hemos creado ningún tag, por lo que no sale información

16. Crea una nueva etiqueta (tag) de nombre v.1 y sube los cambios
- git tag v.1
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

- git commit -m "creado tag v.1"
<details>
<summary>salida</summary>

```code
 [main 18b708e] creado tag v.1
 1 file changed, 155 insertions(+)
```
</details>

- git push
<details>
<summary>salida</summary>

```code
    Username for 'https://github.com': rabgonzalez
    Password for 'https://rabgonzalez@github.com': 
    Enumerando objetos: 5, listo.
    Contando objetos: 100% (5/5), listo.
    Compresión delta usando hasta 4 hilos
    Comprimiendo objetos: 100% (3/3), listo.
    Escribiendo objetos: 100% (3/3), 2.38 KiB | 2.38 MiB/s, listo.
    Total 3 (delta 0), reusados 0 (delta 0), pack-reusados 0
    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    ce8b298..18b708e  main -> main
```
</details>

17. Crea la feature-2 y muevete a esta
- git branch Feature-2
<details>
<summary>salida</summary>

```
```
</details>

- git checkout Feature-2
<details>
<summary>salida</summary>

```code
 M	README.md
 Cambiado a rama 'feature-2'
```
</details>

- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
- nano Estamos_a_punto_de_terminar.html
<details>
<summary>salida</summary>

```
```
</details>

18. Realiza el commit y sube los cambios.
- git add .
<details>
<summary>salida</summary>

```
```
</details>

- git commit -m "creada rama Feature-2"
<details>
<summary>salida</summary>

```code
 [feature-2 aa2c345] creada rama feature-2
 2 files changed, 31 insertions(+), 2 deletions(-)
 create mode 100644 Estamos_a_punto_de_terminar.html
```
</details>

- git push origin Fueature-2
<details>
<summary>salida</summary>

```code
    Username for 'https://github.com': rabgonzalez
    Password for 'https://rabgonzalez@github.com': 
    Enumerando objetos: 6, listo.
    Contando objetos: 100% (6/6), listo.
    Compresión delta usando hasta 4 hilos
    Comprimiendo objetos: 100% (4/4), listo.
    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    remote: 
    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    remote: 
    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    * [new branch]      feature-2 -> feature-2
```
</details>

19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
- git checkout develop
<details>
<summary>salida</summary>

```code
 Cambiado a rama 'develop'
```
</details>

- git merge feature-2
<details>
<summary>salida</summary>

```code
 Actualizando b1b7513..aa2c345
 Fast-forward
 Estamos_a_punto_de_terminar.html |  11 ++
 README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
 adios.html                       |  10 ++
 3 files changed, 368 insertions(+), 1 deletion(-)
 create mode 100644 Estamos_a_punto_de_terminar.html
 create mode 100644 adios.html
```
</details>

20. Sube los cambios de la rama develop a Github.
- git add .
<details>
<summary>salida</summary>

```
```
</details>

- git commit -m "
<details>
<summary>salida</summary>

```code
 En la rama develop
 nada para hacer commit, el árbol de trabajo está limpio
```
</details>

- git push origin develop
<details>
<summary>salida</summary>

```code
Username for 'https://github.com': rabgonzalez
Password for 'https://rabgonzalez@github.com': 
Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
remote: 
remote: Create a pull request for 'develop' on GitHub by visiting:
remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
remote: 
To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
 * [new branch]      develop -> develop
```
</details>

21. Cambia a la rama principal, realiza la mezcla con la rama develop.
- git checkout main
<details>
<summary>salida</summary>

```code
 Cambiado a rama 'main'
 Tu rama está adelantada a 'origin/main' por 1 commit.
  (usa "git push" para publicar tus commits locales) 
```
</details>

- git merge develop
<details>
<summary>salida</summary>

```code
 Auto-fusionando README.md
```
</details>

22. Realiza el tag con el nombre v.2. y sube los cambios.
- git tag v.2
<details>
<ummary>salida</summary>

```
```
</details>

- git add .
<details>
<ummary>salida</summary>

```
```
</details>

- git commit -m "creado tag v.2"
<details>
<ummary>salida</summary>

```code
```
</details>

- git push
<details>
<ummary>salida</summary>

```code
```
</details>

23. Muestra todos los cambios realizados en el repositorio.


24. Muestra todos los commits realizados.

</div>
