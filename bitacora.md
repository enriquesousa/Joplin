18/09/2023 09:38
* * *
- Estoy planeando cambio de Sistema Operativo a MX Linux
- Estoy haciendo Backup de mis Archivos del External HD Toshiba es de 1TB tiene dos particiones, BU_Drive(200GB) TOSHIBA EXt(800GB) esta partición no la puedo utilizar con Linux, pero si la puedo copiar, no mover!. voy a respaldar para poder re formatearlo!


TOSHIBA 1TB
- Películas (149.8 GB)

19/09/2023 09:52
* * *
- Particionar Yoga en 2 discos de 250GB cada uno, usando utilitaria rescatux iso con ventoy en usb 16GB con Bandera de Mexico
- instale Mx Linux 23 a Yoga
- Estoy en el proceso de configuración
- Estoy Sincronizando Insync 
- Estoy Sincronizando DropBox

PCloudDrive

Folders:
- Backups			- 60.6 GB
- My Pictures 		- 13.4 GB
- Vandana HD Share	- 9.5 GB
- luckyBackup		- 7.5 GB
- Insync2021		- 5.9 GB
- My Videos 		- 4.5 GB
- My Music 			- 4.4 GB
- My Downloads	    - 343.6 MB
- py-uia 	        - 134.9 MB
- My Documents	    - 55.6 MB
- Joplin-BackUp  	- 20.7 MB	
- IconsData 		-  6.8 MB 


20/09/2023 06:21
* * *

- Install Docker-Desktop Debian on Mx Linux Yoga
- Tematize por completo Mx Linux Yoga!
- Instael Lando
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