# bitacora de arranque sammmcv

**fecha:** 23/03/2026
**duracion estimada:** 15 minutos

## pasos ejecutados

1. ubique mi directorio de trabajo usando `pwd` y liste los archivos con `ls -lah`.
2. clone mi repositorio remoto ejecutando `git clone https://github.com/sammmcv/presentacion-tecnica-sam`.
3. ingrese a la carpeta del proyecto con `cd presentacion-tecnica-sam`.
4. cree una nueva rama para la tarea y me cambie a ella usando `git checkout -b semana2-arranque`.
5. abri el archivo `README.md` con el editor `nano` para agregar mi username y color favorito.
6. verifique el estado con `git status`, prepare el archivo con `git add README.md` y guarde los cambios con `git commit -m "update: se agrega username y color favorito al readme"`.
7. subi los cambios a mi repositorio remoto utilizando `git push origin semana2-arranque`.

## comandos destacados

| Comando | Qué hizo |
|---|---|
| `git checkout -b` | creo una nueva rama llamada semana2-arranque y me cambio a ella inmediatamente. |
| `git status` | me mostro que el archivo README.md estaba modificado pero aun no estaba agregado al staging area para el commit. |
| `git log --oneline` | me mostro el historial resumido de los commits, confirmando que mi nuevo commit estaba en la cabeza (HEAD) de mi rama. |

## problemas encontrados

**problema:** al intentar hacer el `git push origin semana2-arranque`, la terminal me pidio mi "Password" de GitHub. (github ya no acepta contraseñas tradicionales de cuenta para operaciones en la terminal).
**como lo resolvi:** fui a mi perfil de github en el navegador > settings > developer settings > personal access tokens > tokens (classic). y genere un nuevo token asegurandome de marcar la casilla de permisos "repo", lo copie y lo pegue en la terminal como si fuera mi contraseña para autorizar la subida.

## resultado de `git log --oneline`

```bash
04b2859 (HEAD -> semana2-arranque, origin/semana2-arranque) update: se agrega username y color favorito al readme
0ed2860 (origin/main, origin/HEAD, main) update: presentacion tecnica
396885f first commit
```

## higiene digital aplicada

genere y utilice un personal access token (classic) en github con permisos especificos para repositorios para poder realizar el push a mi rama de forma segura

# evidencia de la terminal

```bash
┬─[samcv@samcv-tp:~/E/C/entregable-2]─[22:59:21]
╰─>$ pwd
/home/samcv/ESCOM/Cidium Security/entregable-2
┬─[samcv@samcv-tp:~/E/C/entregable-2]─[22:59:23]
╰─>$ ls -lah
total 8.0K
drwxrwxr-x 2 samcv samcv 4.0K mar 23 22:44 ./
drwxrwxr-x 5 samcv samcv 4.0K mar 23 22:44 ../
┬─[samcv@samcv-tp:~/E/C/entregable-2]─[22:59:27]
╰─>$ git clone https://github.com/sammmcv/presentacion-tecnica-sam
Clonando en 'presentacion-tecnica-sam'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 6 (delta 0), reused 6 (delta 0), pack-reused 0 (from 0)
Recibiendo objetos: 100% (6/6), listo.
┬─[samcv@samcv-tp:~/E/C/entregable-2]─[23:00:35]
╰─>$ cd presentacion-tecnica-sam
┬─[samcv@samcv-tp:~/E/C/e/presentacion-tecnica-sam]─[23:01:20]─[G:main=]
╰─>$ git checkout -b semana2-arranque
Cambiado a nueva rama 'semana2-arranque'
┬─[samcv@samcv-tp:~/E/C/e/presentacion-tecnica-sam]─[23:01:27]─[G:semana2-arranque]
╰─>$ nano README.md
┬─[samcv@samcv-tp:~/E/C/e/presentacion-tecnica-sam]─[23:04:44]─[G:semana2-arranque]
╰─>$ git status
En la rama semana2-arranque
Cambios no rastreados para el commit:
  (usa "git add <archivo>..." para actualizar lo que será confirmado)
  (usa "git restore <archivo>..." para descartar los cambios en el directorio de trabajo)
	modificados:     README.md

sin cambios agregados al commit (usa "git add" y/o "git commit -a")
┬─[samcv@samcv-tp:~/E/C/e/presentacion-tecnica-sam]─[23:05:31]─[G:semana2-arranque]
╰─>$ git add README.md
┬─[samcv@samcv-tp:~/E/C/e/presentacion-tecnica-sam]─[23:05:54]─[G:semana2-arranque]
╰─>$ git commit -m "update: se agrega username y color favorito al readme"
[semana2-arranque 04b2859] update: se agrega username y color favorito al readme
 1 file changed, 6 insertions(+), 1 deletion(-)
┬─[samcv@samcv-tp:~/E/C/e/presentacion-tecnica-sam]─[23:06:20]─[G:semana2-arranque]
╰─>$ git push origin semana2-arranque
Username for 'https://github.com': sammmcv
Password for 'https://sammmcv@github.com': 
Enumerando objetos: 5, listo.
Contando objetos: 100% (5/5), listo.
Compresión delta usando hasta 8 hilos
Comprimiendo objetos: 100% (2/2), listo.
Escribiendo objetos: 100% (3/3), 359 bytes | 359.00 KiB/s, listo.
Total 3 (delta 1), reusados 0 (delta 0), pack-reusados 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'semana2-arranque' on GitHub by visiting:
remote:      https://github.com/sammmcv/presentacion-tecnica-sam/pull/new/semana2-arranque
remote: 
To https://github.com/sammmcv/presentacion-tecnica-sam
 * [new branch]      semana2-arranque -> semana2-arranque
┬─[samcv@samcv-tp:~/E/C/e/presentacion-tecnica-sam]─[23:06:45]─[G:semana2-arranque]
╰─>$ touch bitacora.md
┬─[samcv@samcv-tp:~/E/C/e/presentacion-tecnica-sam]─[23:08:10]─[G:semana2-arranque]
╰─>$ nano bitacora.md
┬─[samcv@samcv-tp:~/E/C/e/presentacion-tecnica-sam]─[23:08:45]─[G:semana2-arranque]
╰─>$ git log --oneline
04b2859 (HEAD -> semana2-arranque, origin/semana2-arranque) update: se agrega username y color favorito al readme
0ed2860 (origin/main, origin/HEAD, main) update: presentacion tecnica
396885f first commit
```
