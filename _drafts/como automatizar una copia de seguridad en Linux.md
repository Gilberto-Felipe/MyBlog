---
layout: post
title: "¿Cómo automatizar una copia de seguridad en Linux con rsync + cron?"
date: 2022-08-29 20:00:00 -0600
tagline: Automatizar copias de seguridad en Linux
description: "Aprende a automatizar una copia de seguridad en Linux utilizando rsync + cron"
category: Linux
comments: true
---

En esta entrada aprenderás cómo automatizar una copia de seguridad en Linux utilizando rsync y cron job.  

Hacer una copia de seguridad es fundamental, pero automatizarla nos permite ser más eficientes.  

Esta entrada va dirigida a usuarios de Linux novatos. No va dirigido a necesidades empresariales.  

## ¿Qué es rsync?

Rsync es un software para transferir y copiar archivos entre una computadora y un dispositivo externo o entre una red de computadoras. Es compatible con Linux, Microsoft y MacOs.  

Si quieres conocer más sobre rsync puedes leer mi entrada [¿Cómo crear una copia de seguridad en Linux con rsync?]().  

## ¿Qué es cron?  

Cron es el programador de tareas de Linux. Permite ejecutar comandos en un momento determinado: minutos, horas, días, semanas y meses. En pocas palabras, nos ayuda a automatizar tareas programado fecha y hora.  

Cron está instalado y configurado en todas las distros Debian.

## Pasos para automatizar mi copia de seguridad

Abre en terminal el archivo crontab como super usuario (root).

```bash
sudo nano /etc/crontab
```
![imagen]()

Añade el comando que quieres programar en una línea nueva al final. Por ejemplo:

```bash
0 22 * * * sudo gilberto rsync -aAXv --delete /home/gilberto/Documents/ /media/gilberto/Elements/@UbuntuBackup/Documents/
0 22 * * * sudo gilberto rsync -aAXv --delete  /home/gilberto/Music/ /media/gilberto/Elements/@UbuntuBackup/Music/
0 22 * * * sudo gilberto rsync -aAXv --delete /home/gilberto/Pictures/ /media/gilberto/Elements/@UbuntuBackup/Pictures/
0 22 * * * sudo gilberto rsync -aAXv --delete /home/gilberto/Videos/ /media/gilberto/Elements/@UbuntuBackup/Videos/
```

El archivo `crontab` explica el formato de programación. Las abreviaciones significan:

| m | h | dom | mon | dow | user | command |
| minuto | hora | día del mes | mes | día de la semana | usuario que agenda | comando a ejecutar |

Mi copia de seguridad está programada todos los días a las 22 horas (10 pm); sin embargo, tú puedes configurar la hora que necesites.  

Cada copia de seguridad va a sobre escribir la anterior. Ese es el comportamiento que espero.  

## Atención  

**Tu computadora debe estar encendida y tu unidad de recuperación debe estar conectada durante el tiempo programado para ejecutar la copia de respaldo**. De lo contrario, se perderá la tarea de respaldo. **Cron no ejecuta tareas perdidas**. Para ejecutar tareas perdidas, consulta el [anacron](https://linux.die.net/man/8/anacron).

Recuerda: **Nunca debes guardar tu copia de seguridad en el mismo disco duro donde se encuentra la información que pretendes respaldar**. Si se rompe el disco duro, perderás todos los datos.  

## Recuperando los datos  

Recuperar tus archivos es esencial. Es el propósito de respaldarlos. Así pues, asegúrate de que puedes recuperarlos con frecuencia. De lo contrario, te puedes llevar una terrible sorpresa.  

El comando de recuperación es el mismo, solo cambias el origen y el destino.  Aquí:  

Origen: será la copia de seguridad.  

Destino: el lugar donde quieres probar la recuperación de tus datos.

Formas de comprobar:

1. Recupera varios archivos individuales.
2. Recupera una versión antigua de un archivo.
3. Recupera una carpeta entera.
4. Recupera toda la unidad y compara el checksum con el del original.

## Conclusión  

En conclusión, agendar tus copias de seguridad usando cron jobs te ayudan a automatizar tus copias de seguridad. Esto te libera del trabajo manual y te puede salvar los datos un día. Así que, ¡ve y automatiza tus copias de seguridad!

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

cron job

minuto hora dia_mes mes dia_semana + comando

0 22 * * * 

