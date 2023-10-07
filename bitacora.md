# Bitácora Git

Crear una carpeta en /home/enrique/Sites/Joplin
Donde voy a respaldar un backup de Joplin, File/Export All/Joplin Export File 
Y solo voy a copiar un archivo tipo texto que se llame BitacoraGit.md y solo este archivo es el que voy a sincronizar con mi Git para tener siempre una bitácora respaldado en GIT donde diga en pocas palabras en lo que estuve trabajando ese dia!

# 18/09/2023 09:38
- Estoy planeando cambio de Sistema Operativo a MX Linux
- Estoy haciendo Backup de mis Archivos del External HD Toshiba es de 1TB tiene dos particiones, BU_Drive(200GB) TOSHIBA EXt(800GB) esta partición no la puedo utilizar con linux, pero si la puedo copiar, no mover!. voy a respaldar para poder re formaterlo!


TOSHIBA 1TB
- Películas (149.8 GB)

# 19/09/2023 09:52
- Particionar Yoga en 2 discos de 250GB cada uno, usando utilitaria recatux iso con ventoy en usb 16GB con Bandera de Mexico
- instale Mx Linux 23 a Yoga
- Estoy en el proceso de configuración
- Estoy Sincronizando Insync 
- Estoy Sincronizando DropBox

PCloudDrive

Folders:
- Backups			-	60.6 GB
- My Pictures 		- 13.4 GB
- Vandana HD Share	- 9.5 GB
- luckyBackup		- 7.5 GB
- Insync2021		- 	5.9 GB
- My Videos 		- 4.5 GB
- My Music 			- 4.4 GB
- My Downloads	- 343.6 MB
- py-uia 				- 134.9 MB
- My Documents	- 55.6 MB
- Joplin-BackUp  	- 20.7 MB	
- IconsData 		-	6.8 MB 

# 20/09/2023 06:21

- Install Docker-Desktop Debian on Mx Linux Yoga
- Temática completo Mx Linux Yoga!
- Instale Lando
- Lando NO me funciono con Docker Desktop
- Voy desinstalar Docker

Para des-Instalar Docker:
**How To Completely Remove Docker From Your Debian Based Linux**
https://www.lokarithm.com/2020/05/31/how-to-completely-remove-docker-from-debian-ubuntu-or-your-raspberry-pi/

Identify which Docker package have you installed
```
dpkg -l | grep -i docker
sudo apt-get purge -y docker-ce docker-ce-cli
sudo apt-get autoremove -y --purge docker-ce docker-ce-cli
```

Remove the packages	
```
sudo apt-get purge -y docker-engine docker docker.io docker-ce docker-ce-cli

sudo apt-get autoremove -y --purge docker-engine docker docker.io docker-ce
``` 

Remove all the Docker related files
```
sudo rm -rf /var/lib/docker /etc/docker
sudo rm /etc/apparmor.d/docker
sudo groupdel docker
sudo rm -rf /var/run/docker.sock
```

- Volvi a Instalar Docker desde [aqui](https://docs.docker.com/engine/install/debian/#install-using-the-repository) con la instalcion normal en server con docker compose como plug in.
- Y el Docker Compose PlugIn desde [aqui](https://docs.docker.com/compose/install/linux/).
- Volvi a instalar Lando Dev desde su paquete .deb que baje
- Ya me funciono!

## Clone School
1. Clonar repo con Git Kraken a una carpeta por ejemplo:
	`/home/enrique/Sites/lando/`
2. Ver que exista el archivo de configuracion **.lando.yml**
3. Correr: lando start
4. Visitar phpmyadmin con la direccion que nos da lando info
5. Crear una nueva base de datos, dentro de phpmyadmin: school
6. Importar la base de datos de: 	/home/enrique/Sites/lando/school/database/school.sql 
7. Colocarse en la nueva base de datos he importar base de datos
8. lando composer install
9. lando npm install
10. Create a copy of your .env file copiar de .env.example
11. Datos en .env
	DB_CONNECTION=mysql
	DB_HOST=database
	DB_PORT=3306
	DB_DATABASE=school
	DB_USERNAME=root
	DB_PASSWORD=
12. Generate an app encryption key
13. lando php artisan key:generate
14. Storage Link
15. lando php artisan storage:link
16. Visitar Pagina
17. lando info
- Visitar pagina:
-  'http://school.lndo.site/', o
-  'https://school.lndo.site/' 
18. Listo!

# 21/09/2023 19:29
- Instale Rhino Linux En segunda particion de Lenovo Yoga
- Instale:
- Nala, App Image Launcher, Docker, Lando
- GitKraken
- Vscode

# 22/09/2023 14:06
- Voy a trabajar en Mx Linux es mucho mas Pro
- Instale VsCode
- Customizar VsCode con nuevo perfil "Laravel"

# 23/09/2023 07:41
- Seguir customizando VsCode 
- Para crear user snippets ctrl+shift+p User Snippets, Create New User Snippets
- ponerle un nombre por ejemplo "mysnippets", vscode crea un archivo global en `/home/enrique/.config/Code/User/profiles/-3302f02b/snippets/`
- En una instalacion nueva de vscode como este archivo es global no va a tener mis snippets, pro podemos copiarlos de backup que tengo aqui en `Joplin bajo Tools/Vscode/User Snippets`

Crear nuevo Profile en VScode
Settings/Profiles/Create New Profile
`Laravel`

## Extensiones
- community material theme (Equinusocio)
- Laravel artisan (Ryan Naddy)
- Laravel Blade Snippets (Winnie Lin)
- Laravel Blade Spacer (Austen Cameron)
- Laravel Extra Intellisense (amir)
- PHP Intelephense (Ben Mewburn)
- Laravel goto (Adrian)
- Laravel goto view (codingyu)
- Laravel snippets (Winnie Lin)
- PHP DocBlocker (Neil Brayfield) - Bloque de Comentarios
- PHPDoc Comment (Rex Shi) -Add phpdoc @param and @return tag for selected function signatures.
- PHP Namespace Resolver (Mehedi Hassan) - Import and expand php namespaces
- Beautify Blade (Apility AS) - Beautify blade, javascript, JSON, CSS, Sass, and HTML in Visual Studio Code.
- DotENV (mikestead) - Colores para archivo .env
- Paste JSON as Code (quicktype) - Copy JSON, paste as Go, TypeScript, C#, C++ and more.
- Tailwind CSS IntelliSense (Tailwind Labs) 
- VSCode Great Icons (Emmanuel Béziat) - Ver carpetas e icones en side panel
- Database Client (Weijan Chen) - Database manager for MySQL/MariaDB, SQLite, Redis and ElasticSearch.

## Instale en MX Linux
- PHP
- Compose
- Laravel
- Valet Cpriego (Instalo Nginx)
- MariaDB
- Mysql Workbench

# 24/09/2023 08:06
- Instale Vivaldi
- Instale phpMyAdmin de [liga](https://www.phpmyadmin.net/downloads/)
- Importe la Base de Datos school.sql de /home/enrique/Sites/school/database
- Instale php-mysql desde mx install packages para que pudiera funcionar phpMyAdmin

school
Para poder usar nginx local con la base de datos local y valet, cambiar el .env a:
```
APP_NAME=school
APP_ENV=local
APP_KEY=base64:0xsyOMuN+ffSaXCtRXKazgFJr+f7hCtVGBBgPMdOS3s=
APP_DEBUG=true
# APP_URL=http://school.lndo.site
APP_URL=http://school.test

LOG_CHANNEL=stack
LOG_DEPRECATIONS_CHANNEL=null
LOG_LEVEL=debug

# DB_CONNECTION=mysql
# DB_HOST=database
# DB_PORT=3306
# DB_DATABASE=school
# DB_USERNAME=root
# DB_PASSWORD=

DB_CONNECTION=mysql
DB_HOST=localhost
DB_PORT=3306
DB_DATABASE=school
DB_USERNAME=root
DB_PASSWORD=password

```

Ya me funciono todo local.
Siento que es mas eficiente con valet-cpriego que lando.
Pero tengo las dos opciones, si quiero puedo utilizar también lando

# 25/09/2023 17:34
- Me la pase configurando la maquina Optiplex Con Mx Linux
enrique@mx 
OS: MX x86_64 
Host: OptiPlex 9020 00 
Kernel: 6.1.0-12-amd64 
- Instale phpMyAdmin
- FishShell
- GitKraken
- Ulaucher
- Git
- Vscode
- MariaDB Local
	- user: root
	-pasw: password
- PHP
- Composer
- Laravel Installer
- Valet Cpriego
- Listo!

# 26/09/2023 11:11
Actualizar Documentación Joplin
- Nuevo Notebook Bitacora con sub-notebooks para cada Mes
- Septiembre 2023
- En Tools
- Notebook: Fish
- Notebook: Micro
- Notebook: Ranger

# 27/09/2023 13:58
- Instale Terminator 
- en .bashrc
```
# Mis PATHS
export PATH="$PATH:$HOME/.config/composer/vendor/bin"

# Mis Alias
alias r='ranger --choosedir=$HOME/.rangerdir; LASTDIR=`cat $HOME/.rangerdir`; cd "$LASTDIR"'

# Correr Fiash Shell
fish
```

# 28/09/2023 10:35

Quize prender la maquina YOGA! con mi mx linux tematizado y nose que paso que ya no corren los programas de mx tools!!!!!!

En cuention de desarrollo no tenia mucho!
Solo School!
Y este proyecto ya lo tengo actualizado aquí en esta maquina Optiplex que ya la deje funcionando al 100%.

Lo que voy hacer es restablecer el iso de esta optiplex a mi yoga!

- Format Lenovo Yoga con diferentes particiones
- Instale el iso de la maquina optiplex en la particion de 120GB que genere para mx linux 23

# 29/09/2023 10:01 AM

- Lenovo Yoga
- Instale Plank
- Monte el Drive DATA, ahí voy a tener toda mi informacion de:
	- Documents
	- Pictures
	- Downloads
	- Music
	- Videos
- Instale **Shutter** Screen Capture, un mejor screen capture!

# Symbolic link
A [symbolic link](https://linuxhandbook.com/symbolic-link-linux/), also known as a symlink or a soft link, is a special type of file that simply points to another file or directory just like shortcuts in Windows. Creating symbolic link is like creating alias to an actual file.

## How to create a symbolic link in Linux
To create a symbolic link to target file from link name, you can use the ln command with -s option like this:
`ln -s target_file link_name`

Para mi link de Sites
`ln -s /mnt/DATA/Sites Sites`


The -s option is important here. It determines that the link is soft link. If you don’t use it, it will create a hard link. I’ll explain the difference between soft links and hard links in a different article.

## How to follow a symbolic link
To know which real file the link actually points to, use the realpath command:
`realpath link_name`

## How to delete a symbolic link
There is no special command for deleting symlinks in Linux. You can use the same rm command that you use for deleting files and directories.
`rm link_name`
Deleting the link won't delete the source file it links to.
You can delete multiple symbolic links in one command as well:
`rm link1 link2`

# 30/09/2023 9:33 AM

## Crear los symbolic links a mis carpetas en DATA
Crear los links simbólicos para mis carpetas en la partición de DATA! 
- `cd ~`
- `ln -s /mnt/DATA/Sites Sites`
Le cambie los nombres a los links a español para poder usarlos directo, de otra manera genear el simlink dentro de la carpeta.
- `ln -s /mnt/DATA/Documents Documentos`
-  `ln -s /mnt/DATA/Downloads Descargas`
- `ln -s /mnt/DATA/Music Musica`
- `ln -s /mnt/DATA/Pictures Fotos`
- `ln -s /mnt/DATA/Videos Vids`

# Insync
Instalar Insync para [Debian Bookworm](https://www.insynchq.com/install-for-servers#deb-debian)

`cd Descargas`

Bajar el deb de [aquí](https://www.insynchq.com/downloads/linux):
**Debian - Bookworm**
Install:
- insync_3.8.6.50504-bookworm_amd64.deb

Despues de correr la instalacion, escoger la carpeta de descarga en:
`/home/enrique/Data/Insync`
Y Syncronizar solo carpeta de google drive `Insync2022`.

# Clonar Repo
- Clonar en Sites `hugoblog`

# Octubre 2023

# 01/10/2023 8:23 AM
## Domingo
Cumpleaños  peque!  
Desayunar en Cafe de la Flor Pacifico

# 02/10/2023 9:33 AM
## Lunes
- Format e Install Mx Linux 23 a Maquina de Junior de su Oficina


# 03/10/2023 07:29 - Martes
## Martes
- Lista Keyboard Shortcuts `Vivaldi`
- Instale Extension de [Bookmarks](https://github.com/alefragnani/vscode-bookmarks/#bookmarks) en vscode de Alessandro Fragnani
- Ajustar `Login cookie validity = 28800` en phpMyAdmin


# 04/10/2023 07:21 - Miércoles

Optiplex
- Al tratar de instalar mysql-workbench de un deb para ubuntu
- Y despues al querer instalarlo con el procedieminto para Debian como lo tengo aqui en Joplin.
- La maquina me pidio que hiciera un `Full Upgrade` y tardo mucho y con eso ya no pudo funcionar mi maquina, y como no tenia el time shift instalado no pude regresar.
- Encontré una mejor solución aqui en [dbdiagram](https://dbdiagram.io/d) para tener un diseño de la base de datos.
- Voy a generar un snapshot de mi maquina Yoga y la voy a instalar en Optiplex!
- snapshot-4-oct-23-MxLinux23-Yoga.iso
- Listo!

- Crear Time Shift en Partition DATA en Maquina ThinkPad Yoga
- Craer Time Shift para Optiplex
- Cambiar Teclado por Default en `Settings manager / Keyboard`
- Desinstalar Insync en Optiplex despues volver a 
- Instalar Insync en Optiplex
- Esto es para poder volver a asignarle una carpeta nueva local para que syncronice
- No voy a Instalar Insync, voy a tratar de usar solo Pcloud, cualquier informacion que necesite lo puedo copiar de un backaup que haga a Pcloud de mi maquina Yoga a luckybackup
- Optiplex: Instale `fzf` buscador de archivos
- Clonar con GitKraken
	- Joplin
	- school
	- hugoblog
	- realestate

# 06/10/2023 11:28 AM - Viernes

- Preparar mi Lenovo Yoga para Multi boot con una sola /home partition que van a compartir los sistemas operativos que instale
- Time shift en Yoga Ocupa como 18 GB, 2 a la semana y 1 al mes, mas otros 20 GB que deje para el sistema, me quedaría una partition de 40 GB
- Las demás particiones pueden ser de 32 GB cada una 
- Backup Insync/Insync2022 a ADATA USB en /media/enrique/ADATA/luckyBackups/Yoga/mxlinux23/Insync/insync2022
- Son solo 1.8 GB pero se tarda mucho porque son como 40,993 archivos!
- 
- Voy a borrar insync de Yoga
- `sudo apt remove insync`
- Voy a volver a Instalarlo y copiar los datos del backup 
![185291adc730b549920efa5733794ee1.png](:/0478e77fede646578791b9ecd3841922)
- Cambiar a ~/Insync (donde ya copie los datos del backup)
- para ver si Insync lo reconoce y se tarda menos en hacer el sync
- Dismmis los errors en errors 
- dar click en cloud sync
- y de inmediato reconoce y pone la flecha verde que todo esta sync!

- Voy a volver a desinstalar Insync
- Voy a generar priemero el iso de de YOGA
 
## Preparar el HDD

1. Installing Two Linux Distros on a single HDD with a shared Home. Part 1 - Prepping the Hard Drive
[liga](https://www.youtube.com/watch?v=T8ZTDzgmtoY)
2. How to Dualboot and Multiboot Linux (and Windows) [liga](https://www.youtube.com/watch?v=Crleyglb4mo)


# 07/10/2023 10:00 AM - Sábado
- Format Lenovo Yoga
- Instale Partition para:
- Home
- Rhino Linux
- Mx Linux 23
- Swap 8GB

- Instale Mx Linux 23 
- Instale Rhino Linux 2023.3

- con el grub de rhino no puedo entrar a Mx Linux!
- ?





