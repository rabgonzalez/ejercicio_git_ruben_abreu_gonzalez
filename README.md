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
 [main 109a65c] creado tag v.2
 1 file changed, 45 insertions(+)
```
</details>

- git push
<details>
<ummary>salida</summary>

```code
    Username for 'https://github.com': rabgonzalez
    Password for 'https://rabgonzalez@github.com': 
    Enumerando objetos: 15, listo.
    Contando objetos: 100% (15/15), listo.
    Compresión delta usando hasta 4 hilos
    Comprimiendo objetos: 100% (11/11), listo.
    Escribiendo objetos: 100% (11/11), 2.07 KiB | 2.07 MiB/s, listo.
    Total 11 (delta 8), reusados 0 (delta 0), pack-reusados 0
    remote: Resolving deltas: 100% (8/8), completed with 2 local objects.
    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    18b708e..109a65c  main -> main
```
</details>

23. Muestra todos los cambios realizados en el repositorio.
- git diff 0a9c838f20c5b8076f2d11dba4086b3df33dcfa1..HEAD
<details>
<summary>salida</summary>

```code
    diff --git a/Estamos_a_punto_de_terminar.html b/Estamos_a_punto_de_terminar.html
    new file mode 100644
    index 0000000..195149b
    --- /dev/null
    +++ b/Estamos_a_punto_de_terminar.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Terminando </title>
    +</head>
    +<body>
    +<h1 align="center" >Apunto de terminar </h1>
    +<hr>
    +<p> Esto se esta acabando ruben_abreu </p>
    +</body>
    +</html>
    diff --git a/README.md b/README.md
    index e67ac5f..43af0a3 100644
    --- a/README.md
    +++ b/README.md
    @@ -1,3 +1,5 @@
    +<div textalign="justify">
    +
    # Ejercicio Práctico
    # Rubén Abreu González
    ---
    @@ -34,6 +36,535 @@
    <summary>salida</summary>
    
    ```code
    + [main (commit-raíz) 0a9c838] creado el fichero README.md
    + 1 file changed, 39 insertions(+)
    + create mode 100644 README.md
    +```
    +</details>
    +
    +4. Crear una rama con nombre develop.
    +- git branch develop
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +5. Lista las ramas actuales.
    +- git branch
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + develop
    + * main
    +```
    +</details>
    +
    +6. Moverse a la rama y crear el fichero: hola.html. - Añadir el siguiente contenido: 
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- nano hola.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "añadido hola.html"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [develop b1b7513] añadido hola.html
    + 1 file changed, 11 insertions(+)
    + create mode 100644 hola.html
    +```
    +</details>
    +
    +7. Moverse a la rama principal y crear el fichero adios.html > Sustituye nombre_alumno por tu nombre.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'main'
    + Tu rama está basada en 'origin/main', pero upstream ha  desaparecido.
    +  (usa "git branch --unset-upstream" para arreglar)
    +```
    +</details>
    +
    +- nano adios.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +8. Crea el commit con un mensaje descriptivo.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "añadido adios.html"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [main a000351] añadido adios.html
    + 2 files changed, 109 insertions(+), 1 deletion(-)
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +9. Sube los cambios a la rama actual.
    +- git push origin main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 13, listo.
    +    Contando objetos: 100% (13/13), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (12/12), listo.
    +    Escribiendo objetos: 100% (13/13), 2.10 KiB | 2.10 MiB/s, listo.
    +    Total 13 (delta 5), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (5/5), done.
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      main -> main
    +```
    +</details>
    +
    +10. Lista las ramas actuales.
    +- git branch
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +  develop
    + * main
    +```
    +</details>
    +
    +11. Realizar la mezcla en el repositorio principal.
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + hola.html | 11 +++++++++++
    + 1 file changed, 11 insertions(+)
    + create mode 100644 hola.html
    +```
    +</details>
    +
    +12. Sube los cambios al repositorio a tu cuenta de Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "traemos los cambios de la rama develop a la rama main"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [main ce8b298] traemos los cambios de la rama develop  a la rama main
    + 1 file changed, 65 insertions(+)
    +```
    +</details>
    +
    +- git push
    +<details>
    +<summary>salida</summary>
    +
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
    +```code
    +    diff --git a/README.md b/README.md
    +    index 82bae28..b6b672e 100644
    +    --- a/README.md
    +    +++ b/README.md
    +    @@ -198,6 +198,8 @@
    +    <summary>salida</summary>
    +    
    +    ```code
    +    + [main ce8b298] traemos los cambios de la rama develop  a la rama main
    +    + 1 file changed, 65 insertions(+)
    +    ```
    +    </details>
    +    
    +    @@ -205,6 +207,26 @@
    +    <details>
    +    <summary>salida</summary>
    +    
    +    +```code
    +    +Username for 'https://github.com': rabgonzalez
    +    +Password for 'https://rabgonzalez@github.com': 
    +    +Enumerando objetos: 12, listo.
    +    +Contando objetos: 100% (12/12), listo.
    +    +Compresión delta usando hasta 4 hilos
    +    +Comprimiendo objetos: 100% (8/8), listo.
    +    +Escribiendo objetos: 100% (8/8), 1.62 KiB | 1.62 MiB/s, listo.
    +    +Total 8 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    +remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    +   a9f0ec2..ce8b298  main -> main
    +    +```
    +    +</details>
    +    +
    +    +13. Muestra todos los cambios realizados.
    +    +- git diff
    +    +<details>
    +    +<summary>salida</summary>
    +    +
    +```
    +</details>
    +
    +14. Lista ahora los últimos cambios que se han producido en el repositorio, es decir, los últimos commits que han realizado en el repositorio.
    +- git log
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    commit ce8b2980d70366c05a4af8a1bb28b6e94458089c (HEAD -> main, origin/main)
    +    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    +    Date:   Wed Oct 18 15:32:00 2023 +0100
    +
    +        traemos los cambios de la rama develop a la rama main
    +
    +    commit 1ac2997985b24f091db7a1828231526053fb4747
    +    Merge: a9f0ec2 b1b7513
    +    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    +    Date:   Wed Oct 18 15:29:11 2023 +0100
    +
    +        mezclamos las ramas Merge branch 'develop'
    +
    +    commit a9f0ec2ce2514039a2afca48aedafd64f605b571
    +    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    +    Date:   Wed Oct 18 15:25:06 2023 +0100
    +
    +        subimos los cambios
    +
    +    commit b1b7513e00a5de250959875dc6cc3cc424f04459 (develop)
    +    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    +    Date:   Wed Oct 18 15:22:40 2023 +0100
    +
    +        añadido hola.html
    +
    +    commit b1d417305b7e0ffc30aa04ab29f0a0aee04039ae
    +    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    +    Date:   Wed Oct 18 15:21:33 2023 +0100
    +
    +        añadido adios.html
    +
    +    commit a000351cfa8b2d7e639439cf3b26c9d94023bb2b
    +    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    +    Date:   Wed Oct 18 15:20:53 2023 +0100
    +
    +        añadido adios.html
    +
    +    commit 0a9c838f20c5b8076f2d11dba4086b3df33dcfa1
    +    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    +    Date:   Wed Oct 18 15:05:10 2023 +0100
    +
    +        creado el fichero README.md
    +```
    +</details>
    +
    +15. Lista todos los tags(etiquetas que existan).
    +- git tag
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +> Nota: todavía no hemos creado ningún tag, por lo que no sale información
    +
    +16. Crea una nueva etiqueta (tag) de nombre v.1 y sube los cambios
    +- git tag v.1
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.1"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [main 18b708e] creado tag v.1
    + 1 file changed, 155 insertions(+)
    +```
    +</details>
    +
    +- git push
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 5, listo.
    +    Contando objetos: 100% (5/5), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (3/3), listo.
    +</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Estamos_a_punto_de_terminar.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +18. Realiza el commit y sube los cambios.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Actualizando b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +- git push
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +23. Muestra todos los cambios realizados en el repositorio.
    +
    +
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/null
    +++ b/adios.html
    @@ -0,0 +1,10 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Hola </title>
    +</head>
    +<body>
    +<h1 align="center" >Hola soy un título </h1>
    +<hr>
    +<p> Hola soy el alumno ruben_abreu </p>
    +</body>
    +</html>+    Escribiendo objetos: 100% (3/3), 2.38 KiB | 2.38 MiB/s, listo.
    +    Total 3 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    ce8b298..18b708e  main -> main
    +```
    +</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Es+</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Estamos_a_punto_de_terminar.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +18. Realiza el commit y sube los cambios.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Actualizando b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +- git push
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +23. Muestra todos los cambios realizados en el repositorio.
    +
    +
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/n+</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Estamos_a_punto_de_terminar.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +18. Realiza el commit y sube los cambios.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Actualizando b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +- git push
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +23. Muestra todos los cambios realizados en el repositorio.
    +
    +
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/null
    +++ b/adios.html
    @@ -0,0 +1,10 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Hola </title>
    +</head>
    +<body>
    +<h1 align="center" >Hola soy un título </h1>
    +<hr>
    +<p> Hola soy el alumno ruben_abreu </p>
    +</body>
    +</html>">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Hola </title>
    +</head>
    +<body>
    +<h1 align="center" >Hola soy un título </h1>
    +<hr>
    +<p> Hola soy el alumno ruben_abreu </p>
    +</body>
    +</html>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    ++</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Estamos_a_punto_de_terminar.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +18. Realiza el commit y sube los cambios.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Actualizando b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +- git push
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +23. Muestra todos los cambios realizados en el repositorio.
    +
    +
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/null
    +++ b/adios.html
    @@ -0,0 +1,10 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Hola </title>
    +</head>
    +<body>
    +<h1 align="center" >Hola soy un título </h1>
    +<hr>
    +<p> Hola soy el alumno ruben_abreu </p>
    +</body>
    +</html>ndo b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    ++</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Estamos_a_punto_de_terminar.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +18. Realiza el commit y sube los cambios.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Actualizando b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +- git push
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +23. Muestra todos los cambios realizados en el repositorio.
    +
    +
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/null
    +++ b/adios.html
    @@ -0,0 +1,10 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Hola </title>
    +</head>
    +<body>
    +<h1 align="center" >Hola soy un título </h1>
    +<hr>
    +<p> Hola soy el alumno ruben_abreu </p>
    +</body>
    +</html>
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>+</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Estamos_a_punto_de_terminar.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +18. Realiza el commit y sube los cambios.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Actualizando b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +- git push
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +23. Muestra todos los cambios realizados en el repositorio.
    +
    +
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/null
    +++ b/adios.html
    @@ -0,0 +1,10 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.ht+</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Estamos_a_punto_de_terminar.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +18. Realiza el commit y sube los cambios.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Actualizando b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +- git push
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +23. Muestra todos los cambios realizados en el repositorio.
    +
    +
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/null
    +++ b/adios.html
    @@ -0,0 +1,10 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Hola </title>
    +</head>
    +<body>
    +<h1 align="center" >Hola soy un título </h1>
    +<hr>
    +<p> Hola soy el alumno ruben_abreu </p>
    +</body>
    +</html>
    +<head>
    +<title>Hola </title>
    +</head>
    +<body>
    +<h1 align="center" >Hola soy un título </h1>
    +<hr>
    +<p> Hola soy el alumno ruben_abreu </p>
    +</body>
    +</html>
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/null
    +++ b/adios.html
    @@ -0,0 +1,10 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Hola+</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Estamos_a_punto_de_terminar.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +18. Realiza el commit y sube los cambios.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Actualizando b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +- git push
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +23. Muestra todos los cambios realizados en el repositorio.
    +
    +
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/null
    +++ b/adios.html
    @@ -0,0 +1,10 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE H+</details>
    +
    +17. Crea la feature-2 y muevete a esta
    +- git branch Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git checkout Feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + M     README.md
    + Cambiado a rama 'feature-2'
    +```
    +</details>
    +
    +- Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:
    +- nano Estamos_a_punto_de_terminar.html
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +18. Realiza el commit y sube los cambios.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creada rama Feature-2"
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + [feature-2 aa2c345] creada rama feature-2
    + 2 files changed, 31 insertions(+), 2 deletions(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    +```
    +</details>
    
    +- git push origin Fueature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +    Username for 'https://github.com': rabgonzalez
    +    Password for 'https://rabgonzalez@github.com': 
    +    Enumerando objetos: 6, listo.
    +    Contando objetos: 100% (6/6), listo.
    +    Compresión delta usando hasta 4 hilos
    +    Comprimiendo objetos: 100% (4/4), listo.
    +    Escribiendo objetos: 100% (4/4), 871 bytes | 871.00 KiB/s, listo.
    +    Total 4 (delta 1), reusados 0 (delta 0), pack-reusados 0
    +    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    +    remote: 
    +    remote: Create a pull request for 'feature-2' on GitHub by visiting:
    +    remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/feature-2
    +    remote: 
    +    To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    +    * [new branch]      feature-2 -> feature-2
    ```
    -</details>
    \ No newline at end of file
    +</details>
    +
    +19. Muevete a la rama develop, y realiza la mezcla con la rama feature-2.
    +- git checkout develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'develop'
    +```
    +</details>
    +
    +- git merge feature-2
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Actualizando b1b7513..aa2c345
    + Fast-forward
    + Estamos_a_punto_de_terminar.html |  11 ++
    + README.md                        | 348 ++++++++++++++++++++++++++++++++++++++-
    + adios.html                       |  10 ++
    + 3 files changed, 368 insertions(+), 1 deletion(-)
    + create mode 100644 Estamos_a_punto_de_terminar.html
    + create mode 100644 adios.html
    +```
    +</details>
    +
    +20. Sube los cambios de la rama develop a Github.
    +- git add .
    +<details>
    +<summary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + En la rama develop
    + nada para hacer commit, el árbol de trabajo está limpio
    +```
    +</details>
    +
    +- git push origin develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    +Username for 'https://github.com': rabgonzalez
    +Password for 'https://rabgonzalez@github.com': 
    +Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
    +remote: 
    +remote: Create a pull request for 'develop' on GitHub by visiting:
    +remote:      https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez/pull/new/develop
    +remote: 
    +To https://github.com/rabgonzalez/ejercicio_git_ruben_abreu_gonzalez
    + * [new branch]      develop -> develop
    +```
    +</details>
    +
    +21. Cambia a la rama principal, realiza la mezcla con la rama develop.
    +- git checkout main
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Cambiado a rama 'main'
    + Tu rama está adelantada a 'origin/main' por 1 commit.
    +  (usa "git push" para publicar tus commits locales) 
    +```
    +</details>
    +
    +- git merge develop
    +<details>
    +<summary>salida</summary>
    +
    +```code
    + Auto-fusionando README.md
    +```
    +</details>
    +
    +22. Realiza el tag con el nombre v.2. y sube los cambios.
    +- git tag v.2
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git add .
    +<details>
    +<ummary>salida</summary>
    +
    +```
    +```
    +</details>
    +
    +- git commit -m "creado tag v.2"
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +- git push
    +<details>
    +<ummary>salida</summary>
    +
    +```code
    +```
    +</details>
    +
    +23. Muestra todos los cambios realizados en el repositorio.
    +
    +
    +24. Muestra todos los commits realizados.
    +
    +</div>
    diff --git a/adios.html b/adios.html
    new file mode 100644
    index 0000000..a088504
    --- /dev/null
    +++ b/adios.html
    @@ -0,0 +1,10 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Adios </title>
    +</head>
    +<body>
    +<h1 align="center" >Adios soy un título </h1>
    +<hr>
    +<p> Adios soy el alumno ruben_abreu </p>
    +</body>
    diff --git a/hola.html b/hola.html
    new file mode 100644
    index 0000000..cb50374
    --- /dev/null
    +++ b/hola.html
    @@ -0,0 +1,11 @@
    +<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    +<html>
    +<head>
    +<title>Hola </title>
    +</head>
    +<body>
    +<h1 align="center" >Hola soy un título </h1>
    +<hr>
    +<p> Hola soy el alumno ruben_abreu </p>
    +</body>
    +</html>
```
</details>

24. Muestra todos los commits realizados.
<details>
<summary>salida</summary>

```code
    commit 109a65c1837d1c23462d9cc4a94c3a31bcf9a675 (HEAD -> main, origin/main)
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 16:05:50 2023 +0100

        creado tag v.2

    commit 78de99ff237175dc3665c745b9fa772b9ca4fff2 (tag: v.2)
    Merge: c6cc878 aa2c345
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 16:02:46 2023 +0100

        ejercicio 21

    commit c6cc87847506513f759c70fe9ce473206e625612
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:59:15 2023 +0100

        traemos develop

    commit b15af47a59aa0fd83ec70c46bf9c42a9401c2889
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:52:12 2023 +0100

        rama feature-2 y html

    commit aa2c345cb134ec52361f53948febb728c5fbb2dd (origin/feature-2, origin/develop, feature-2, develop)
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:45:30 2023 +0100

        creada rama feature-2

    commit 18b708ea1c3060b572516c66056a6614595d469f
    Author: rabgonzalez <rubalba.rag@gmail.comgit config --global user.name rabgonzalez>
    Date:   Wed Oct 18 15:40:38 2023 +0100

        creado tag v.1

    commit ce8b2980d70366c05a4af8a1bb28b6e94458089c (tag: v.1)
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

    commit b1b7513e00a5de250959875dc6cc3cc424f04459
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