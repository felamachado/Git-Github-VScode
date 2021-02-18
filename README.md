Configuración de un repositorio de Github en local.

OJO!: Si creo un repositorio local y luego quiero asociarlo a un repo remoto, hay que tener en cuenta que la rama principal git la llama master, y en github la llaman main. Por lo que si commiteo un local a remoto, me va a decir que en remoto, la rama master no existe, o me va a crear otra rama con el nombre master. 

1) Me posiciono en la carpeta donde quiero descargar la carpeta del repositorio remoto.
Y ejecuto el comando:

	git clone rutadelreporemoto

	se crea una carpeta con el nombre del repo remoto y descarga los archivos.
2) Pongo en esa carpeta nueva los archivos que quiero subir.

3)Entro en la carpeta creada y ejecuto
	
	git status

me va a mostrar todos los archivos que puse en rojo (porque no estan trackeados aun)

4) Para agregar todos los archivos al git local ejecuto:

	git add .

5) Commiteamos los cambios para todos los archivos.

	git commit -m "Mensaje para commit"

6) Puedo ver que no tengo archivos para comitear con:

	git status

7) Subo los archivos a remoto:

	gut push

Nota: para que no me pida nombre de usuario y contaseña, debo configurar previamente el acceso a github por ssh, y cuando hago gitclone, traigo la ruta con el acceso ssh.
