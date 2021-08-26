---
layout: post
title: "¿Cómo crear una copia de seguridad en Linux con rsync?"
date: 2022-08-29 20:00:00 -0600
tagline: crear copias de seguridad en Linux
description: "Aprende a crear una copia de seguridad en Linux utilizando rsync"
category: Linux
comments: true
---

En esta entrada aprenderás cómo crear una copia de seguridad en Linux utilizando rsync y cron job.  

Hacer una copia de seguridad es fundamental. Nos puede salvar de perder días, meses, años de trabajo. Automatizarla nos permite ser más eficientes.  

## ¿Qué es rsync?

Rsync es un software para transferir y copiar archivos entre una computadora y un dispositivo externo o entre una red de computadoras a través de un algoritmo de diferenciación. Es una utilidad estandar en Linux y compatible con Microsoft y MacOs.  

## Systema de archivos  

Se recomienda que la unidad de respaldo tenga un sistema de archivos compatible con Linux como ext4 o exFAT.  

El sistema FAT de Windows no reconoce los atributos del sistema de archivos de Linux.  

ext4 es el sistema de archivos de Linux. Solo es compatible con sistemas Linux.  

exFAT es compatible con Linux, Windows y MacOs.  

FUSE (Filesystem in Userspace por sus siglas en inglés) o sistema de archivos en el espacio de usuraio es compatible con Windows, Mac y Linux.

Elige el sistema de archivos que se ajuste a tus necesidades. Si es necesario, formatea tu unidad de respaldo o crea una partición y asígnale el sistema de archivos que necesites.  

## Comandos  

Los comandos comandos pueden parecer intimidantes, pero en este caso los parámetros del comando no son tan complicados.  

ubicarme en root : cd / si voy a exlcuir carpetas.

``` bash
sudo rsync -aAXv --delete --dry-run /origen/ /destino/  
```

## Tabla de comandos  

| comando      | explicación                                                     |
|:-------------|:------------------                                              |
| sudo         | permisos de super usuario                                       |
| rsync        | es el nombre del programa                                       |
| -a           | modo ade hivo                                                   |
| -A           | Conserva la lista de acceso                                     |
| -X           | Conserva los atributos extendidos, es decir, conserva todos los atributos de los archivos |
| -v           | verbose: muestra el progreso de backup                          |
| --delete     | habilita un backup incremental                                  |
| --dry-run    | Simula el backup, solo sirve de prueba                          |
| --exclude    | Excluye carpetas y archivos del backup                          |
| /origen      | Define el origen de los arhivo a copiar                         |
| /Destino     | Ruta de destino donde quiero guardar mis archivos               |

`--delete` es opcional. Permite hacer copias incrementales. Esto es, si ya tienes una copia guardada, el respaldo solo guardará las diferencias entre el origen y el destino. Resumiendo, el parámetro incremental solo respaldará los archivos nuevos y modificados, y borrará de la copia de seguridad todos los archivos que fueron eliminados de tu sistema. Piensa si esto se ajusta a tus necesidades. Sé cuidadoso.  

`--dry run` sirve para probar el backup, lo simula y arroja información sobre el mismo: número de archivos, tamaño de la copia, etc.  

```bash
sudo rsync -aAXv --delete --dry-run --exclude=/dev/* --exclude=/proc/* --exclude=/sys/* --exclude=/tmp/* --exclude=/run/* --exclude=/mnt/* --exclude=/media/* --exclude="swapfile" --exclude="lost+found" --exclude=".cache" --exclude="Downloads" --exclude=".VirtualBoxVMs"--exclude=".ecryptfs" / /run/media/alu/ALU/


sudo rsync -aAXv --delete --dry-run /home/gilberto/Documents/ /media/gilberto/Elements/@UbuntuBackup/Documents/
sudo rsync -aAXv --delete --dry-run /home/gilberto/Music/ /media/gilberto/Elements/@UbuntuBackup/
sudo rsync -aAXv --delete --dry-run /home/gilberto/Pictures/ /media/gilberto/Elements/@UbuntuBackup/
sudo rsync -aAXv --delete --dry-run /home/gilberto/Videos/ /media/gilberto/Elements/@UbuntuBackup/Videos/

```

## Haciendo la copia de seguridad  

1. Ejecuta la simulación con `--dry run` para que recibas información de que lo que estás respaldando.
2. Remueve el parámetro `--dry run` y ejecuta rsync.
3. Verifica que los datos se copiaron en el destino.
4. Comprueba recuperando los datos.

## Recuperando los datos  

Recuperar tus archivos es esencial. Es el propósito de respaldarlos. Así pues, asegúrate de que puedes recuperarlos con frecuencia. De lo contrario, te puedes llevar una terrible sorpresa.  

El comando de recuperación es el mismo, solo cambias el origen y el destino. Aquí:  

Origen: será la copia de seguridad.  

Destino: el lugar donde quieres probar la recuperación de tus datos.

Formas de comprobar:

1. Recupera varios archivos individuales.
2. Recupera una versión antigua de un archivo.
3. Recupera una carpeta entera.
4. Recupera toda la unidad y compara el checksum con el del original.

## Alternativas gráficas a rsync  

Existen alternativas gráficas a rsync tales como: grsync, Bacula, SimpleBackupSuite, TimeVault, Deja Dup, LuckyBackup

## Conclusión  

Rsync es una herramienta poderosa para respaldar archivos utilizando la línea de comandos. Sus opciones le permiten ser una herramienta flexible para hacer tus copias de seguridad.  

Ahora ya sabes cómo crear una copia de seguridad. El siguiente paso es automatizarla para que no dependa de nosotros. Lee mi artículo [¿Cómo automatizar una copia de seguridad en Linux?]().

## Referencias  

https://help.ubuntu.com/community/BackupYourSystem  

https://www.lifewire.com/backup-ubuntu-4126286#:~:text=On%20the%20Ubuntu%20desktop%2C%20select,don't%20want%20to%20save.  

https://www.hostinger.es/tutoriales/cron-job  

https://en.wikipedia.org/wiki/Rsync  

https://averagelinuxuser.com/backup-and-restore-your-linux-system-with-rsync/  *** Este es el bueno ***

https://www.youtube.com/watch?v=zJVSzIy3ips&ab_channel=Ale9hack  

https://www.youtube.com/watch?v=yO5t-siWv3E&ab_channel=Carlo2366  

https://github.com/libfuse/libfuse

https://es.wikipedia.org/wiki/Sistema_de_archivos_en_el_espacio_de_usuario

https://www.xataka.com/basics/sistemas-de-archivo-como-saber-cual-elegir-al-formatear-tu-disco-duro-o-usb

## Sobre mi sistema operativo

Ubuntu LTS 18.04.05 x86-64 GNU/Linux.
