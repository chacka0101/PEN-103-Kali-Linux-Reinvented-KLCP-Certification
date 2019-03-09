KLCP_Certification - Kali_Linux: Kali Linux Certified Professional - 2019
==

Kali Linux es una distribución de Linux para auditoría de seguridad lista para la empresa basada en Debian GNU / Linux. 
Kali está dirigido a profesionales de la seguridad y administradores de TI, lo que les permite realizar pruebas avanzadas
de penetración, análisis forense y auditorías de seguridad.

Prerrequisitos
--
https://www.edx.org/course/introduction-to-linux

Arquitecturas Diponibles para Kali:
amd64, i386, armel, armhf, arm64

Recursos
--
- WEB: https://kali.training
- Book: https://kali.training/downloads/Kali-Linux-Revealed-1st-edition.pdf
- Training: https://kali.training/lessons/introduction/
- Foros: https://forums.kali.org/
- Blog: https://www.kali.org/blog/-
- Docs: https://docs.kali.org/ 
- Dojo: https://www.kali.org/kali-linux-dojo-workshop/
- Mirror List: http://cdimage.kali.org/README.mirrorlist
- Generar Passwords Robustas: https://www.pwdgen.org/

El Sistema Operativo de KALI LINUX es DEBIAN
--

- Debian Handbook: https://debian-handbook.info/browse/es-ES/stable/
- https://www.debian.org/doc/manuals/debian-reference/debian-reference.es.pdf

Sistemas ARM en Kali Linux
--
- http://docs.kali.org/category/kali-on-arm

Hackers Data Base:
--

- https://www.securityfocus.com/
- https://packetstormsecurity.com/
- https://www.exploit-db.com/
- https://github.com/rapid7/metasploit-framework/tree/master/modules
 
Linea de tiempo de las Distros de Hacking:
-- 
- KNOPIX - WhoppiX (2004)
- SLAX - WHAX (2005)
- SLAX - BackTrack (2006)
- UBUNTU - BackTrack 4 (2009)
- UBUNTU - BackTrack R1, R2, R3 (2010-2012)
- DEBIAN - Kali Linux 1.0 (2013)
- DEBIAN - Kali Linux 2.0 (2015-2016)
- DEBIAN - Kali Linux 2019.1 (2019)

Comprimir o descomprimir:
--
* Archivos .tar.xz:
  * Comprimir: tar -Jcvf paquete.tar.xz /carpeta/a/empaquetar/
  * Descomprimir: tar -Jxvf paquete.tar.xz

* Archivos .tar.gz:
  * Comprimir: tar -czvf paquete.tar.gz /carpeta/a/empaquetar/
  * Descomprimir: tar -xzvf paquete.tar.gz

* Archivos .tar:
  * Empaquetar: tar -cvf paquete.tar /dir/a/comprimir/
  * Desempaquetar: tar -xvf paquete.tar

* Archivos .gz:
  * Comprimir: gzip -9 index.php
  * Descomprimir: gzip -d index.php.gz

* Archivos .zip:
  * Comprimir: zip archivo.zip carpeta
  * Descomprimir: unzip archivo.zip

* Archivos .xz:
  * Comprimir: xz archivo.xz
  * Descomprimir: unxz archivo.xz

GNOME es el entorno de escritorio predeterminado de Kali Linux
--
- root@hacker:~# gnome-shell --version  (Versión del Gnome)
- root@hacker:~# gnome-shell --replace  (Lanzar una nueva gnome por shell)

Respositorios o Paquetes
--
- Kali Linux Git Repositories: http://git.kali.org/gitweb/
- Kali Linux Package Tracker: http://pkg.kali.org/
- Mirror original: http.kali.org

Soporte de ARM
--
Debian soporta de manera completa tres adaptaciones a distintos sabores de hardware ARM little-endian:
La adaptación ARM EABI (armel) está enfocada hacia dispositivos ARM antiguos de 32 bits, en particular, aquellos usados en hardware NAS y una variedad de ordenadores *plug.
La adaptación más nueva ARM hard-float (armhf) soporta dispositivos más nuevos, y más potentes, de 32 bits, usando la versión 7 de la especificación de la arquitectura ARM.
La adaptación ARM de 64 bits (arm64) soporta los últimos dispositivos ARM de 64 bits.

COMMANDS
--
https://wiki.debian.org/ShellCommands#Z

- root@chacka0101:~# pwd (Directorio actual)
- root@hchacka0101:~# d (change directory)
- root@chacka0101:~# ls (list file or directory contents)
- root@chacka0101:~# mkdir (make directory)
- root@chacka0101:~# rmdir (remove directory)
- root@chacka0101:~# mv, rm, and cp (move, remove or copy file or directory respectively)
- root@chacka0101:~# cat (concatenate or show file)
- root@chacka0101:~# less/more (show files a page at a time)
- root@chacka0101:~# uname --all (Identificación de Arquitectura de Procesador)
Linux hacker 4.18.0-kali2-amd64 #1 SMP Debian 4.18.10-2kali1 (2018-10-09) x86_64 GNU/Linux
- root@chacka0101:~# uname -r (Versión del Kernel)
- root@chacka0101:~# apt update (Actualizar)
- root@chacka0101:~# apt list --upgradable (Actualizar)
- root@chacka0101~# sha256sum kali-linux-2016.2-amd64.iso (Comando para verificar la integridad del ISO)
  * 1d90432e6d5c6f40dfe9589d9d0450a53b0add9a55f71371d601a5d454fa0431  kali-linux-2016.2-amd64.iso
- root@chacka0101:~# ls -l /dev/sd* (Identificar la USB)
- root@chacka0101:~# sudo rm archivo.xxx (Borrar archivo)
- root@chacka0101:~# sudo rm -rf directorio (Borrar directorio)
- root@chacka0101:~# sudo fdisk -l (Visualizar Disco Duro y Particiones)
- root@chacka0101:~# cat /proc/filesystems  (Tipos de sistemas de Archivos soportados por Kali)
  * Mas info: https://wiki.debian.org/FileSystem
- root@chacka0101:~# ls /etc/init.d  (Procesos Abiertos)
- root@chacka0101:~# sudo systemctl restart nombredelproceso (Reiniciar proceso)
- root@chacka0101:~# sudo killall nombredelproceso  (Matar proceso)
- root@chacka0101:~# kill %1  (Matar proceso segundo plano)
- root@chacka0101:~# top (Lista los procesos en tiempo real)
- root@chacka0101:~# top -b -n1 > /root/Desktop/process.log (Guardar procesos en un log)
- root@chacka0101:~# jobs -l  (Lista los procesos en segundo plano)
- root@chacka0101:~# echo $PATH  (Variable de entorno)
  * /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
- root@chacka0101:/etc # cat profile (Editar la Variable de Entorno)
- root@chacka0101:/etc # cat environment  (Definir variables de entorno no especificas)
- root@chacka0101:~# which ls  (Buscar la ubicación de los comandos)
- root@chacka0101:~# type rm (Muestra información de los comandos)
- root@chacka0101:~# type pwd (Tipo de cada comando)
- root@chacka0101:~# ls -al (Listar archivos ocultos en la Ubicación actual, Tenga en cuenta que los nombres de archivo que comienzan con un punto están ocultos por defecto.)
- root@chacka0101:~# cat archivo.txt  (Visualiza el contenido del archivo)
- root@chacka0101:~# ps axjf | less  (Lista todos los Procesos - PID)
  * A : Select all processes
  * u : Select all processes on a terminal, including those of other users
  * x : Select processes without controlling ttys

Search
--
- root@chacka0101:~# find / -name nombreexactodeloquebusco (Buscando archivos y dentro de archivos)
- root@chacka0101:~# find / -name "nombredeloquebusco*"  (Buscando archivos y dentro de archivos)
- root@chacka0101:~# grep -r "nombredeloquebusco" /    (Busqueda recursiva con Grep)
- root@chacka0101:~# find / -path /proc -prune -o -type f -perm +6000 -ls  (Buscar todos los ficheros con permisos SUID o SGID)
- root@chacka0101:~# find / -path /proc -prune -o -type f -perm +4000 -ls  (Buscar todos los ficheros con permisos solo SUID)
- root@chacka0101:~# find / -path /proc -prune -o -type f -perm +2000 -ls  (Buscar todos los ficheros con permisos solo SGID)
- root@chacka0101:~# locate "*rockyou.txt.gz*"

Permisos de los archivos y directorios - CHMOD
--
chmod(change permissions), chown (change owner), and chgrp (change group).
Setuid - suid "Set User ID"
Setgid - setgid "Set Group ID" 
- Son permisos de acceso que pueden asignarse a archivos o directorios. Se utilizan principalmente para permitir a los usuarios
del sistema ejecutar con privilegios elevados temporalmente para realizar una tarea específica. Si un fichero tiene activado
el bit "Setuid" se identifica con una “s” en un listado de la siguiente forma:
-rwsr-xr–x 1 root shadow 27920 ago 15 22:45 /usr/bin/passwd
- Visualizar Permisos:
root@chacka0101:~# ls -al /bin/ping
-rwxr-xr-x 1 root root 65272 Aug  3  2018 /bin/ping

- https://es.wikipedia.org/wiki/Chmod
- https://chmod-calculator.com
- El primer dígito establece el tipo de permiso deseado al dueño; el segundo al grupo; y el tercero al resto de los usuarios.
chmod 766 file.txt   # brinda acceso total al dueño
                     # y lectura y escritura a los demás
chmod 770 file.txt   # brinda acceso total al dueño y al grupo
                     # y elimina todos los permisos a los demás usuarios
chmod 635 file.txt   # Permite lectura y escritura al dueño, 
                     # escritura y ejecución al grupo,
                     # y lectura y ejecución al resto
HARD DISK
--
- Información de Disco Duro:
root@chacka0101:~# free -t -l --human
Información de Disco Duro:
root@chacka0101:~# df --all

- Información del usuario actual:
root@chacka0101:~# id
uid=0(root) gid=0(root) groups=0(root)

- Información de Logs:
root@chacka0101:~# journalctl --all
Información de Logs en especifico:
root@chacka0101:~# journalctl -u ssh.service
Información de los Logs del Kernel:
root@chacka0101:~# dmesg --human --kernel | more

INFORMACIÓN DE HARDWARE
--
root@chacka0101:~# lshw -short
- Drivers o Firmware:
root@hacker:/lib/firmware# ls -la
- Información de Hardware Detallada:
root@chacka0101:~# lspci -vv | less
- Información de la CPU:
root@chacka0101:~# dmesg | grep CPU0:
[    0.708219] smpboot: CPU0: Intel(R) Core(TM) i7-8550U CPU @ 1.80GHz (family: 0x6, model: 0x8e, stepping: 0xa)
- Información de Ethernet:
root@chacka0101:~# lspci | grep Ethernet
02:01.0 Ethernet controller: Intel Corporation 82545EM Gigabit Ethernet Controller (Copper) (rev 01)
- Información de Tarjeta de Video:
root@chacka0101:~# lspci -v -s `lspci | grep VGA | cut -f1 -d\ `
- Información de Hardware USB Detallada:
root@chacka0101:~# lsusb -vv | less
- Información de Hardware sencilla:
root@chacka0101:~# lspci
- Información de Hardware USB sencilla:
root@chacka0101:~# lsusb
- Instalar el lshw: root@chacka0101:~# sudo apt-get install lshw

Calcular el tiempo de ejecución de comandos:
--
root@chacka0101:~# time locate "*rockyou.txt.gz*"
/usr/share/wordlists/rockyou.txt.gz
real	0m0.369s
user	0m0.088s
sys	0m0.016s
root@chacka0101:~# time find / -name "*rockyou.txt.gz*"
find: ‘/run/user/130/gvfs’: Permission denied
/usr/share/wordlists/rockyou.txt.gz
real	0m2.965s
user	0m0.276s
sys	0m0.594s



MONTAR LA MEMORIA USB CON LA TERMINAL:
PENDIENTE...

Consideraciones de BIOS
--
Si bien las imágenes de Kali Linux se pueden iniciar en modo UEFI en el BIOS, no admiten el INICIO SEGURO. Debes deshabilitar 
esa característica en la configuración de BIOS.

KERNEL
--
- Seguridad de Kernel basada en anillos: https://es.wikipedia.org/wiki/Anillo_(seguridad_inform%C3%A1tica)
- El kernel exporta datos sobre el hardware detectado a través de los sistemas de archivos /proc/y /sys/virtuales.
- Las aplicaciones a menudo acceden a los dispositivos por medio de archivos creados dentro /dev/. 
- Los archivos específicos representan unidades de disco (por ejemplo, /dev/sda)
Particiones ( /dev/sda1)
Mouse ( /dev/input/mouse0)
Teclados ( /dev/input/event0)
Tarjetas de sonido ( /dev/snd/*)
Puertos Seriales ( /dev/ttyS*) y otros componentes.

- Tipos de Dispositivos "Device files" son dos (2):
(b)block: Tiene un tamaño finito y puede acceder a bytes en cualquier posición del bloque.
(c)character: Puede leer y escribir caracteres, pero no puede buscar una posición determinada y cambiar bytes arbitrarios.
Ejemplo de Tipo de Archivo en Bloque por que inicia con la letra (b) brw-rw y la comprobación se hace digitando # ls -l:
root@chacka0101:~# ls -l /dev/sda
brw-rw---- 1 root disk 8, 0 Feb 27 11:00 /dev/sda
The programming interface includes device-specific commands that can be invoked through the ioctl system call.
- Comprobar el tipo de dispositivo:
root@chacka0101:~# sudo file /dev/sda
/dev/sda: block special (8/0)
root@chacka0101:~# sudo file /dev/ttyS0
/dev/ttyS0: character special (4/64)

Gerarquia del Sistema de Archivos Filesystem Hierarchy Standard (FHS)
--
/bin/:	Programas basicos
/boot/:	El kernel Kali Linux y otros archivos necesarios para su proceso de arranque temprano
/dev/:	Archivos de dispositivo
/etc/:	Archivos de configuración
/home/:	Archivos personales del usuario
/lib/:	Bibliotecas básicas
/mnt/:	Punto de montaje temporal
/opt/:	Aplicaciones adicionales proporcionadas por terceros
/root/:	Archivos personales del administrador (raíz)
/run/:	Datos de tiempo de ejecución volátiles que no persisten en los reinicios (aún no incluidos en el FHS)
/sbin/:	Programas del sistema
/srv/:	Datos utilizados por los servidores alojados en este sistema
/tmp/:	Archivos temporales (este directorio a menudo se vacía en el arranque)
/var/:	Datos variables manejados por demonios. Esto incluye archivos de registro, colas, spools y cachés.
/proc/y /sys/: Son específicos para el kernel de Linux (y no son parte del FHS). Son utilizados por el núcleo para exportar
datos al espacio de usuario.
/usr/: Aplicaciones (este directorio es subdividen en bin, sbin, libde acuerdo con la misma lógica que en el directorio raíz)
Además, /usr/share/contiene los datos independientes de la arquitectura. El /usr/local/administrador debe utilizar el directorio
para instalar las aplicaciones manualmente sin sobrescribir los archivos que maneja el sistema de empaque ( dpkg).

NETWORK
--




Questions and Answers
--
1. What versions of Debian is Kali 1.0 ,2.0 and Rolling based on?
Kali 1.0 was based on Debian Wheezy. Kali 2.0 is based on Jessie.

2. What are the main differences between a Live boot instance of Kali, and an Installed instance?
Live mode boots to RAM, and an installed instance of Kali boots to a storage device.

3. What’s the difference between live and forensics mode?
Live mode boots to RAM, but may auto-mount disks. Forensics mode does not auto-mount drives.

4. How can we verify that forensics mode is working?
Use the mount command to verify that no disks are mounted. You can also md5 the system’s swap and disk devices, reboot into forensic mode and md5 again. The md5 hashes should match if forensics mode succeeded. Try this in a system you don’t care about “tainting”!

5. What’s the best way to get a tool included in Kali ?
The best way to request for a tool addition is to open a “New Tool Requests” ticket in the Kali Bug Tracker.

6. Name some of the cool features in Kali!
A live system, forensics mode, a custom linux kernel, completely customizable, a trusted operating system with default disabled network services, ARM support, preloaded security tools, penetration testing platform!

7. The most current version of Kali is:
A rolling distribution based on Debian testing

8. ¿En qué buenos ejemplos puedes pensar para arrancar Kali en vivo? ¿Qué pasa con los malos ejemplos?
Kali Live es genial cuando desea: mantener una copia portátil de Kali en su bolsillo; pruebe Kali Linux sin hacer ningún cambio en su computadora; Necesito activar el modo forense. Es una mala idea usar Kali live como cualquier tipo de instalación permanente, especialmente si está esperando guardar cambios (¡no persistir!) O si tiene memoria limitada en la máquina de arranque.

9. ¿Te parece extraño que puedas simplemente copiar una ISO en una llave USB y hacer que arranque?
El Kali (y Debian) ISO es un  isohíbrido . Cuando se crea la ISO, una utilidad syslinux ejecuta el comando isohybrid en la ISO, que agrega una tabla de partición a la ISO, a la vez que mantiene un archivo ISO válido.

10. Si tiene un escritorio Intel de 64 bits, ¿qué imagen de Kali arrancará en su máquina? Seleccione todas las que correspondan.
Kali de 32 bits
Kali de 64 bits

11. ¿Qué archivo virtual puede verificar para determinar si la CPU en su máquina Kali Linux es de 32 o 64 bits?
/ proc / cpuinfo

12. ¿Qué comando descargará e importará la clave pública de Kali a través de https?
gpg_import https://www.kali.org/archive-key.asc

13. Al instalar Kali Linux en una máquina virtual, ¿qué método de instalación producirá una instalación limpia?
Cargar imagen oficial, validada Kali VM.
 
14. Which character is used to represent the user’s home directory?
Usage of ~ for Home directory

15. Which tools can be used to get file information? Check all that apply.
type
which
 
16. Which of the following is not a block or character device?
drwxr-xr-x 2 root root 60 Mar 21 08:30 vfio
 
17. How can the file permissions -r—w—- be represented in octal notation?
420

18. Based on the following partial directory listing, what permissions does user have on the file test?
-r-x--x--- 1 user root 0 Mar 24 01:19 test
 Read, Execute
 
19. You have two jobs running in the background. How do you kill the first job you executed?
kill %1

20. Which command does not control the permissions or user attributes associated with a file?
chperm

21. Which command displays the identity of the user running the session along with the list of groups they belong to?
 id
 
22. Which command summarizes the PCI hardware through the /proc and /sys virtual filesystems?
lspci

23. According to the FHS, which directory contains log files, queues, spools and cache data handled by daemons?
 /var

24. What are the minimum required resources to a VM machine? 
2GB RAM, 20 GB disk space!

25. What technologies are used for encryption?
LUKS and Logical Volume Management (LVM)

26. Which is the recommended configuration for simple Intel-based Kali SSH server with no desktop (headless)?
 512 MB RAM / 2 GB hard drive free space / amd64 CPU

27. Generally speaking, which of these is not a minimum requirement for a Kali Linux desktop?
 512 MB RAM / 2 GB hard drive free space
 
 28. True or False: The Kali Linux installation will fail if you do not select a network mirror.
 False
 
 29. True or False: When booted from the mini.iso, the Kali Linux installation will fail if network hardware can not be detected.
 True
 
 30. Which partitioning scheme is most likely to be affected by user error?
 Manual
 
 31. Which partitioning method is preferred for servers and multi-user systems?
 Separate /home, /var, and /tmp partitions
 
32. Installing a modern version of Windows after a Kali installation will:
 Erase the boot loader and prevent Kali from booting

33. What is the purpose of preseed.cfg?
 Provide predetermined answers to installation questions

34. What is the simplest and most effective procedure for installing Kali on an ARM device?
 Boot from an official, validated Kali ARM image and log in with root/toor

34. Which method is not readily available for saving debug logs during a failed install?
 Save logs to Kali bug tracker
