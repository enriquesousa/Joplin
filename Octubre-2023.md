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

# 08/10/2023 8:01 AM - Domingo 
- Instale Insync en Yoga
- Configuración de Virt-Manager ver [Share Folder](:/263cc546a6c24b949a0c4bd00b074923)

# 09/10/2023 18:47 - Lunes
- Arregle mi setup de musica area de la sala
![4fddfc54925bbf20ddc46601c9218698.png](:/649b6e8f9ef64acd945557d21b8988b4)
La anterior la hize con copy paste.

Las fotos es mejor con [liga](https://photos.app.goo.gl/ZWftEFY4R95Ha9G18) para poder verlas en todas las maquinas!

Si queremos copiar la imagen 4fddfc54925bbf20ddc46601c9218698.png a:
`/home/enrique/.config/joplin-desktop/resources`

Voy crear una carpeta en `home/enrique/pCloudDrive/Joplin-BackUp/Imagenes` para hacer backups de las imagenes que estan en:
`/home/enrique/.config/joplin-desktop/resources`

Insertar Imagen dede HD con la opcion de menu Edit/Attacch File

![4fddfc54925bbf20ddc46601c9218698.png](:/ac4b4a6192c94d9881634ae1a5061adb)


# 10/10/2023 10:12 - Martes
Fui a comprar a steren un USb de 32GB para pasar el MX OS personalizado snap shot que tome de Yoga son como 18 GB!


# 11/10/2023 10:13 - Miércoles

- En Zorin OS todavía
- Bajar Imágenes de:
- Peppermint OS Debian
- Manjaro OS
- Crear Ventoy USB en mi usb de 32 GB
- Copiar snapshot-20231008_0959.iso 
- Copiar PeppermintOS-Debian-64.iso
- Baje Vivalde mientras en mi Zorin OS
- Listo
- Ya tengo Mx Linux 23 en Latitude con todo y Virt Machine
- Tuve que des-instalar y volver a instalar Joplin de FlatPak para que funcionara.
- Vincule de nuevo DropBox
- Encendi temporalmente que inicie con start up Insync y DropBox para que syncromizen archivos
- Reinstale VsCode con Mx Linux Package Installer
- NO funciona VsCode lo voy a des instalar y volver a instalar con Mx Package Installer
- Lo voy a Instalar con Flatpak
```
This version is running inside a container and is therefore not able
to access SDKs on your host system!
To execute commands on the host system, run inside the sandbox:
  $ host-spawn <COMMAND>
To make the Integrated Terminal automatically use the host system's shell,
you can add this to the settings:
```
- Se va a complicar vs code con Flatpak
- Lo instalare normal del repositorio de MX Linux

## Problema con nueva version de VsCode 1.83
vscode 1.83.0 freezes on folder with git, debian bookworm 12
Voy a Instalarlo con estas [Instrucciones](https://code.visualstudio.com/docs/setup/linux): 
https://code.visualstudio.com/docs/setup/linux
Sigue Igual! :(

Lo voy a Instalar con snap 
Instalar snapd en Debian 12 [liga](https://linux.how2shout.com/setup-snap-and-snap-store-in-debian-12-bookworm-linux/)
`sudo apt install snapd`
First start and enable it:
`sudo systemctl start snapd`
`sudo systemctl enable snapd`
Now check the status:
`sudo systemctl status snapd`
After that also install the core files required by it.
`sudo snap install core`

For those who want to use its command syntax to install the various software, here is the that to follow:
`sudo snap install package-name`

Installing Snap Store for Debian 12
`sudo snap install snap-store`

In a few minutes, the installation will be completed, but you won’t find the icon of Snap Store by default in the Application menu. To get it, reboot your Debian 12 once.
`sudo reboot`

Con snap si funciona! y con la ultima version 1.83
```
Version: 1.83.0
Commit: e7e037083ff4455cf320e344325dacb480062c3c
Date: 2023-10-03T16:11:49.843Z
Electron: 25.8.4
ElectronBuildId: 24154031
Chromium: 114.0.5735.289
Node.js: 18.15.0
V8: 11.4.183.29-electron.0
OS: Linux x64 6.1.0-12-amd64 snap
```

-  Instale LMDE 6 en Optiplex

11/10/2023 8:01 PM
- Clone school en Latitude


## Pasos Resumen
1. Clonar repo con Git Kraken a una carpeta por ejemplo:
	`/home/enrique/Sites/`
2. Asegurarnos de tener `/home/enrique/Sites/phpMyAdmin/` todos los archivos unzip
3. `valet link`
4. Ver los links `valet links`
5. Crear una nueva base de datos, dentro de phpmyadmin: school
6. Importar la base de datos de: 	`/home/enrique/Sites/lando/school/database/school.sql` 
7. Colocarse en la nueva base de datos he importar base de datos
8. `composer install`
9. `npm install`
10. Create a copy of your .env file copiar de .env.example
11. Cuando Instale Mysql 
12. [Install MariaDB](:/cba15e118ff543dca80829075b8254d3)
13. El servidor quedo con:
14. DB_USERNAME=root
15. DB_PASSWORD=password
16. Datos en .env

```
APP_NAME=Laravel
APP_ENV=local
APP_KEY=base64:d40ASwzlQI7ibtIf9MYUcMbO6g1F/buwrQd/iQDHSx8=
APP_DEBUG=true
APP_URL=http://school.test

LOG_CHANNEL=stack
LOG_DEPRECATIONS_CHANNEL=null
LOG_LEVEL=debug

DB_CONNECTION=mysql
DB_HOST=localhost
DB_PORT=3306
DB_DATABASE=school
DB_USERNAME=root
DB_PASSWORD=password
```

	
17. Generate an app encryption key
18. `php artisan key:generate`
19. Storage Link
20. `php artisan storage:link`
21. `valet link`
22. Visitar Pagina: 
23. Listo!

# 12/10/2023 8:33 AM - Jueves
- Instale Pcloud a VM Rhino Linux, solo baje su app image se hace ejecutable y se corre directamente
- Instale Joplin en Rhino Linux con flatpak y sync con pcloud

En Yoga
- Reset de user y password a Mariabd [Install MariaDB](:/cba15e118ff543dca80829075b8254d3)
- Login a GitHub
- Instalar phpMyAdmin (En Vivaldi NO pude hacer Login) lo use con Firefox
- Clonar school
- crear correctamente el .env
- composer install
- npm isntall
- php artisan key:generate
- php artisan storage:link
- valet link

Listo!

# 13/10/2023 6:48 AM - Viernes

En Yoga:
- clone phpinfo
- clone realestate

# 16/10/2023 6:56 AM - Lunes

- En Latitude
- Clone hugoblog, realestate, phpinfo
- Inicie Proyecto Nuevo POS (Point of Sale)
- Hasta 107. Install Laravel Breeze


# 17/10/2023 11:01 AM - Martes

1. 108. Login with Name, email or Phone Part 1
2. 109. Login with Name, email or Phone Part 2
3. 110. Project Theme Overview
4. 111. Admin Template Setup
5. 112. Dashboard Page Segmentation






