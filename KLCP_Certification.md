KLCP_Certification - Kali_Linux: Kali Linux Certified Professional - 2019
==

Kali Linux es una distribución de Linux para auditoría de seguridad lista para la empresa basada en Debian GNU / Linux. 
Kali está dirigido a profesionales de la seguridad y administradores de TI, lo que les permite realizar pruebas avanzadas
de penetración, análisis forense y auditorías de seguridad.

Prerrequisitos
--
https://www.edx.org/course/introduction-to-linux

* Arquitecturas Diponibles para Kali:
  * amd64, i386, armel, armhf, arm64

* Consideraciones de BIOS
  * Si bien las imágenes de Kali Linux se pueden iniciar en modo UEFI en el BIOS, no admiten el INICIO SEGURO. Debes deshabilitar esa característica en la configuración de BIOS.

Recursos
--
- WEB: https://kali.training
- Book: https://kali.training/downloads/Kali-Linux-Revealed-1st-edition.pdf
- Training: https://kali.training/lessons/introduction/
- Foros: https://forums.kali.org/
- Blog: https://www.kali.org/blog/-
- Documentación de Kali Linux: https://docs.kali.org/ 
- Dojo: https://www.kali.org/kali-linux-dojo-workshop/
- Tools de Kali Linux: https://tools.kali.org/
- Mirror List: http://cdimage.kali.org/README.mirrorlist
- Generar Passwords Robustas: https://www.pwdgen.org/
- GitHub de Unix Ninja: https://github.com/unix-ninja
- Blog de g0tmi1k: https://blog.g0tmi1k.com/
- Github de Offensive Security: https://github.com/offensive-security

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
- https://wpvulndb.com/wordpresses
- https://tools.kali.org/
 
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
 - root@chacka0101:~# passwd root  (Cambiar password de Usuario root)

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
* Tipos de Permisos
  * chmod (change permissions)
  * chown (change owner)
  * chgrp (change group).
  * Setuid - suid "Set User ID"
  * Setgid - setgid "Set Group ID" 

* Son permisos de acceso que pueden asignarse a archivos o directorios. Se utilizan principalmente para permitir a los usuarios
del sistema ejecutar con privilegios elevados temporalmente para realizar una tarea específica. Si un fichero tiene activado
el bit "Setuid" se identifica con una “s” en un listado de la siguiente forma:
  * -rwsr-xr–x 1 root shadow 27920 ago 15 22:45 /usr/bin/passwd

- root@chacka0101:~# ls -al /bin/ping (Visualizar Permisos)
-rwxr-xr-x 1 root root 65272 Aug  3  2018 /bin/ping
* Algunos Recursos:
  * https://es.wikipedia.org/wiki/Chmod
  * https://chmod-calculator.com
* El primer dígito establece el tipo de permiso deseado al dueño; el segundo al grupo; y el tercero al resto de los usuarios.
  * chmod 766 file.txt 
   > brinda acceso total al dueño y lectura y escritura a los demás
  * chmod 770 file.txt    
   > brinda acceso total al dueño y al grupo y elimina todos los permisos a los demás usuarios
  * chmod 635 file.txt
   > Permite lectura y escritura al dueño, escritura y ejecución al grupo, y lectura y ejecución al resto
   
HARD DISK
--
- root@chacka0101:~# free -t -l --human   (Información de Disco Duro)
- root@chacka0101:~# df --all  (Información de Disco Duro)
- root@chacka0101:~# id   (Información del usuario actual)
  * uid=0(root) gid=0(root) groups=0(root)
- root@chacka0101:~# journalctl --all  (Información de Logs)
- root@chacka0101:~# journalctl -u ssh.service  (Información de Logs en especifico)
- root@chacka0101:~# dmesg --human --kernel | more   (Información de los Logs del Kernel)

INFORMACIÓN DE HARDWARE
--
- root@hacker:/lib/firmware# ls -la (Drivers o Firmware)
- root@chacka0101:~# lshw -short (Información de Hardware)
- root@chacka0101:~# lspci -vv | less  (Información de Hardware Detallada)
- root@chacka0101:~# dmesg | grep CPU0:    (Información de la CPU)
  * [    0.708219] smpboot: CPU0: Intel(R) Core(TM) i7-8550U CPU @ 1.80GHz (family: 0x6, model: 0x8e, stepping: 0xa)
- root@chacka0101:~# lspci | grep Ethernet    (Información de Ethernet)
  * 02:01.0 Ethernet controller: Intel Corporation 82545EM Gigabit Ethernet Controller (Copper) (rev 01)
- root@chacka0101:~# lspci -v -s `lspci | grep VGA | cut -f1 -d\ `  (Información de Tarjeta de Video)
- root@chacka0101:~# lsusb -vv | less  (Información de Hardware USB Detallada)
- root@chacka0101:~# lspci   (Información de Hardware sencilla)
- root@chacka0101:~# lsusb    (Información de Hardware USB sencilla)
- root@chacka0101:~# sudo apt-get install lshw   (Instalar el lshw)

Calcular el tiempo de ejecución de comandos:
--
- root@chacka0101:~# time locate "*rockyou.txt.gz*"
```
/usr/share/wordlists/rockyou.txt.gz
   > real	0m0.369s
   > user	0m0.088s
   > sys	0m0.016s
```
- root@chacka0101:~# time find / -name "*rockyou.txt.gz*"
```
find: ‘/run/user/130/gvfs’: Permission denied
  * /usr/share/wordlists/rockyou.txt.gz
   > real	0m2.965s
   > user	0m0.276s
   > sys	0m0.594s
```
KERNEL
--
-  Seguridad de Kernel basada en anillos: https://es.wikipedia.org/wiki/Anillo_(seguridad_inform%C3%A1tica)
 * El kernel exporta datos sobre el hardware detectado a través de los sistemas de archivos /proc/y /sys/virtuales.
 * Las aplicaciones a menudo acceden a los dispositivos por medio de archivos creados dentro /dev/. 
- Los archivos específicos representan unidades de disco (por ejemplo, /dev/sda)
  * Particiones ( /dev/sda1)
  * Mouse ( /dev/input/mouse0)
  * Teclados ( /dev/input/event0)
  * Tarjetas de sonido ( /dev/snd/*)
  * Puertos Seriales ( /dev/ttyS*) y otros componentes.

- Tipos de Dispositivos "Device files" son dos (2):
  * (b)block: Tiene un tamaño finito y puede acceder a bytes en cualquier posición del bloque.
  * (c)character: Puede leer y escribir caracteres, pero no puede buscar una posición determinada y cambiar bytes arbitrarios.

- Ejemplo de Tipo de Archivo en Bloque por que inicia con la letra (b) brw-rw y la comprobación se hace digitando # ls -l:
- root@chacka0101:~# ls -l /dev/sda
  * brw-rw---- 1 root disk 8, 0 Feb 27 11:00 /dev/sda
- root@chacka0101:~# sudo file /dev/sda   (Comprobar el tipo de dispositivo)
  * /dev/sda: block special (8/0)
- root@chacka0101:~# sudo file /dev/ttyS0
  * /dev/ttyS0: character special (4/64)

Gerarquia del Sistema de Archivos Filesystem Hierarchy Standard (FHS)
--
- /bin/:	Programas basicos
- /boot/:	El kernel Kali Linux y otros archivos necesarios para su proceso de arranque temprano
- /dev/:	Archivos de dispositivo
- /etc/:	Archivos de configuración
- /home/:	Archivos personales del usuario
- /lib/:	Bibliotecas básicas
- /mnt/:	Punto de montaje temporal
- /opt/:	Aplicaciones adicionales proporcionadas por terceros
- /root/:	Archivos personales del administrador (raíz)
- /run/:	Datos de tiempo de ejecución volátiles que no persisten en los reinicios (aún no incluidos en el FHS)
- /sbin/:	Programas del sistema
- /srv/:	Datos utilizados por los servidores alojados en este sistema
- /tmp/:	Archivos temporales (este directorio a menudo se vacía en el arranque)
- /var/:	Datos variables manejados por demonios. Esto incluye archivos de registro, colas, spools y cachés.
- /proc/y /sys/: Son específicos para el kernel de Linux (y no son parte del FHS). Son utilizados por el núcleo para exportar
datos al espacio de usuario.
- /usr/: Aplicaciones (este directorio es subdividen en bin, sbin, libde acuerdo con la misma lógica que en el directorio raíz)
Además, /usr/share/contiene los datos independientes de la arquitectura. El /usr/local/administrador debe utilizar el directorio
para instalar las aplicaciones manualmente sin sobrescribir los archivos que maneja el sistema de empaque ( dpkg).

NETWORKING
--
Command | Descripción
------------ | -------------
ifconfig | muestra el enlace y el estado de la dirección de los interfaces activos
ip addr show | muestra el enlace y el estado de la dirección de los interfaces activos
route -n | muestra la tabla de encaminamiento al completo en direcciones numéricas
ip route show | muestra la tabla de encaminamiento al completo en direcciones numéricas
arp | muestra el contenido actual de la tabla de caché ARP
ip neigh | muestra el contenido actual de la tabla de caché ARP
plog | display ppp daemon log
ping | theeaglelabs.com	comprueba la conexión de Internet con «theeaglelabs.com»
whois theeaglelabs.com | comprueba quién registro «theeaglelabs.com» en la base de datos de dominios
traceroute theeaglelabs.com | sigue la conexión a Internet hasta «theeaglelabs.com»
tracepath theeaglelabs.com | sigue la conexión a Internet hasta «theeaglelabs.com»
mtr theeaglelabs.com | sigue la conexión a Internet hasta «theeaglelabs.com» (de forma repetida)
dig [@dns-server.com] example.com [{a|mx|any}] | comprueba lso registros DNS de «example.com» por «dns-server.com» para los registros «a», «mx», u «any»
iptables -L -n | comprueba el filtrado de paquetes
netstat -a | encuentra todos los puertos abiertos
netstat -l --inet | encuentra los puertos que están escuchando
netstat -ln --tcp | encuentra los puertos (numéricos) TCP que están escuchando
dlint example.com | comprueba la información DNS de la zona «example.com»

- Configurar la red WIFI por interfaz gráfica:
![Alt Text](https://kali.training/wp-content/uploads/2017/02/16_network_manager-1024x768.png)
Imágen tomada de Kali Training.
- Comandos de red importantes:
  * root@chacka0101:~# ifconfig -a  (Lista todas las interfaces de red)
  * root@chacka0101:~# sudo dhclient eth0 (Activar el DHCP)
  * root@chacka0101:~# sudo service networking restart (Reiniciar el Servicio de red)
  * root@chacka0101:~# sudo service networking stop (Parar el Servicio de red)
  * root@chacka0101:~# sudo service networking start (Iniciar el Servicio de red)
  * root@chacka0101:~# ifconfig eth0 up  (Activar tarjeta de red)
  * root@chacka0101:~# ifconfig eth0 down  (Desactivar tarjeta de red)
  * root@chacka0101:~# sudo ifconfig eth0 192.168.2.5 netmask 255.255.255.0 broadcast 192.168.2.7    (Configurar Manualmente la red)
- Más información: https://www.debian.org/doc/manuals/debian-reference/ch05.es.html

Gestión de Usuario y Grupos
--
- USUARIOS:
- root@chacka0101:/etc# cat passwd (lista de usuarios)
- root@chacka0101:/etc# cat shadow (contraseñas cifradas de los usuarios)
- root@chacka0101:/etc# getent hosts (Información de Bases de Datos, passwd, group, hosts, services, protocols, o networks).
- root@chacka0101:~# adduser chacka0101 (Adicionar un usuario)
- root@chacka0101:~# passwd chacka0101 (Establecer contraseña para un usuario)
- root@chacka0101:~# adduser user group (Adicionar un usuario a un grupo)
- root@chacka0101:/etc# cat adduser.conf  (Configuraciones de Usuarios)
- root@chacka0101:~# passwd -l user (Bloquear un usuario)
- root@chacka0101:~# passwd -l olduser (Suspender un usuario)
- root@chacka0101:~# passwd -u user (Desbloqeuar un usuario)
- root@chacka0101:/# id  (Usuario Actual, Grupo Principal Actual, Lista de Grupos)
  * uid=0(root) gid=0(root) groups=0(root)
- usermode Options:
  * -c = We can add comment field for the useraccount.
  * -d = To modify the directory for any existing user account.
  * -e = Using this option we can make the account expiry in specific period.
  * -g = Change the primary group for a User.
  * -G = To add a supplementary groups.
  * -a = To add anyone of the group to a secondary group.
  * -l = To change the login name from tecmint to tecmint_admin.
  * -L = To lock the user account. This will lock the password so we can’t use the account.
  * -m = moving the contents of the home directory from existing home dir to new dir.
  * -p = To Use un-encrypted password for the new password. (NOT Secured).
  * -s = Create a Specified shell for new accounts.
  * -u = Used to Assigned UID for the user account between 0 to 999.
  * -U = To unlock the user accounts. This will remove the password lock and allow us to use the user account.
  * root@chacka0101:/# usermod -a -G sudo usuario1
  * root@chacka0101:/# chsh -s /bin/bash usuario1 (chsh define la shell de login de un usuario)


- GRUPOS:
- root@chacka0101:/etc# cat group (listar los grupos)
- root@chacka0101:/etc# cat gshadow (contraseñas cifradas de grupos)
- root@chacka0101:/# delgroup grupo (Eliminar un grupo)
- root@chacka0101:/# addgroup grupo (Adicionar un grupo)
- root@chacka0101:/# groupmod grupo (Modificar un grupo)
- root@chacka0101:/# gpasswd grupo (Cambiar password de un grupo)
- root@chacka0101:/# gpasswd -r grupo  (Remover la contraseña del grupo)

Configuración de Software o Package
--
- root@chacka0101:/# dpkg -s paquete (Resumen de información del paquete)
- root@chacka0101:/# cat /usr/share/doc/paquete/README.md  (Documentación de un Paquete)
- root@chacka0101:/# dpkg -L paquete (Lista de archivos incluidos en el paquete)
- root@chacka0101:/# cat /usr/share/doc/paquete/examples/ (Ejemplos de archivos de configuración en el directorio)
- Averiguar la última versión de un paquete: http://pkg.kali.org/pkg/nmap

SSH
--
- root@chacka0101:/# systemctl start ssh (Iniciar el servicio de SSH)
- root@chacka0101:/# systemctl enable ssh (Iniciar el servicio de SSH desde el arranque del OS)
   > El servicio de SSH está desactivado por defecto, es importante configurarlo.
- root@chacka0101:/# ssh -V (Versión del SSH)
- root@chacka0101:/# cat /etc/ssh/sshd_config | more (Archivo de configuración del SSH)
- root@chacka0101:/# nano /etc/ssh/sshd_config (Editar el archivo de configuración)
  > Editar la opción de "PermitRootLogin to yes" para que el usuario root pueda utilizar el servicio.
- root@chacka0101:/# systemctl reload ssh (Recargar el servicio de SSH)
- root@chacka0101:/etc/ssh# service ssh status  (Estado del servicio)
- Generando nuevas claves de host SSH
  > Cada servidor SSH tiene sus propias claves criptográficas; se denominan "claves de host SSH" y se almacenan en /etc/ssh/ssh_host_*. Deben mantenerse en privado si desea confidencialidad y no deben ser compartidas por varias máquinas.
- root@chacka0101:/etc/ssh# rm /etc/ssh/ssh_host_*     (Eliminación KEYS)
- root@chacka0101:/etc/ssh# dpkg-reconfigure openssh-server   (Creación de nuevas KEYS)
> Creating SSH2 RSA key; this may take some time ...
2048 SHA256:9TMrDGlKjhYHTqVcTEn617pynWwYkyiEY/p4VEhc/7c root@chacka0101 (RSA)
Creating SSH2 ECDSA key; this may take some time ...
256 SHA256:3kTZYldZ2HHh8+BJRQRwXpgl+eePFGLfHJK8CMw2vbs root@chacka0101 (ECDSA)
Creating SSH2 ED25519 key; this may take some time ...
256 SHA256:jHzsoF5JaUkK5/7UFZTSzilAgTJKxJvC//fUhNa0Mtw root@chacka0101 (ED25519)
rescue-ssh.target is a disabled or a static unit, not starting it.
- root@chacka0101:/etc/ssh# service ssh restart   (Reiniciar el servicio de SSH)
- root@chacka0101:/etc/ssh# service ssh status  (Estado del servicio)

PostgreSQL
--
- root@chacka0101:/# systemctl start postgresql  (Iniciar el servicio de postgresql)
- root@chacka0101:/# systemctl enable postgresql (Iniciar el servicio de SSH desde el arranque del OS)
- root@chacka0101:/etc/postgresql# psql --version  (Versión del postgresql, en este caso es la 11 y el directorio es 11)
  * psql (PostgreSQL) 11.1 (Debian 11.1-2)
- root@chacka0101:/# cat /etc/postgresql/11/main/postgresql.conf | more (Archivo de configuración del SSH)  
- root@chacka0101:/etc/postgresql/11/main# service postgresql status  (Estado del servicio)
- root@chacka0101:/# systemctl reload postgresql (Recargar el servicio de postgresql)
- root@chacka0101:/# service postgresql status  (Estado del servicio)
- root@chacka0101:/etc/postgresql/11/main# ls   (Directorio del postgresql)
  * conf.d  environment  pg_ctl.conf  pg_hba.conf  pg_ident.conf  postgresql.conf  start.conf
- El usuario se llama postgresql, root@chacka0101:/etc/postgresql# cat /etc/passwd
> postgres: x :113:117:PostgreSQL administrator,,,:/var/lib/postgresql:/bin/bash

* Comandos de Postgres:
  *  root@chacka0101:/# su - postgres
  >  (Comandos; createuser, dropuser, createdb, dropdb)
  *  postgres@chacka0101:~$ createuser -P usuariodechacka
  *  Enter password for new role: 
  *  Enter it again: 
  *  postgres@chacka0101:~$ createdb -T template0 -E UTF-8 -O usuariodechacka usuariodechacka
  *  postgres@chacka0101:~$ exit

* INGRESAR A LA BASE DE DATOS:
  *  root@chacka0101:/# sudo -u postgres psql
  *  psql (11.1 (Debian 11.1-2))
  *  Type "help" for help.
  *   
  *  postgres=# \?   (Listar comandos)
  *  postgres=# \l   (Lista las bases de datos y usuarios)

* Con las teclas (ctrl+z) puede salir de la ventana de comandos

* CONECTARSE A LA BASE DE DATOS:
  *  root@chacka0101:/# psql -h localhost -U usuariodechacka usuariodechacka
  *  Password for user usuariodechacka: 
  *  psql (11.1 (Debian 11.1-2))
  *  SSL connection (protocol: TLSv1.3, cipher: TLS_AES_256_GCM_SHA384, bits: 256, compression: off)
  *  Type "help" for help.
  *   
  *  usuariodechacka=> \help
  
* Mas informacion: https://wiki.debian.org/es/PostgreSql

APACHE
--
* Nombre del paquete "apache2"
- root@chacka0101:/# systemctl start apache2 (Iniciar el servicio Apache)
- root@chacka0101:/# systemctl enable apache2 (Iniciar el servicio de Apache desde el arranque del OS)
   > El servicio de APACHE está desactivado por defecto, es importante configurarlo.
- root@chacka0101:/# apache2 -V (Versión del Apache)
* Archivo de configuración de Apache2
  * root@chacka0101:/etc/apache2/sites-enabled# ls
  * 000-default.conf
  * root@chacka0101:/etc/apache2/sites-enabled# cat 000-default.conf 

* HOST VIRTUALES
  * Cada host virtual adicional se describe a continuación mediante un archivo almacenado en /etc/apache2/sites-available/. Por lo general, el archivo recibe el nombre del nombre de host del sitio web seguido de un .confsufijo (por ejemplo:) www.chacka0101.com.conf.

* root@chacka0101:~# dpkg -l apache2    (Verificar si el paguete de apache2 está funcionando)
* root@chacka0101:~# systemctl enable apache2    (Habilitar el servicio de apache2)
* root@chacka0101:~# systemctl status apache2    (Verificar e servicio de apache2)
* root@chacka0101:~# mkdir -p /var/www/html/chacka0101.com    (Crear el directorio que contiene la página web)
* root@chacka0101:~# cd /var/www/html/chacka0101.com
* root@chacka0101:/var/www/html/chacka0101.com# nano index.html     (Crear la página web)
```
<html>
   <head>
     <title>Welcome to CHackA - Colombia Hack Agent</title>
   </head>
   <body>
    <h1>CHackA - Colombia Hack Agent</h1>
     Hacked by CHackA!
   </body>
</html>
```
* root@chacka0101:/var/www/html/chacka0101.com# chown -R www-data: /var/www/html     (Establecer privilegios para el directorio)
* root@chacka0101:/var/www/html/chacka0101.com# nano /etc/apache2/sites-available/chacka0101.com.conf  (Configurar el virtual Host)
```
<VirtualHost *:80>
   ServerAdmin admin@chacka0101.com
   ServerName chacka0101.com
   ServerAlias www.chacka0101.com
   DocumentRoot /var/www/html/chacka0101.com
   ErrorLog ${APACHE_LOG_DIR}/chacka0101.com_error.log
   CustomLog ${APACHE_LOG_DIR}/chacka0101.com_access.log combined
  </VirtualHost>
```
* root@chacka0101:/etc/apache2/sites-available# sudo a2dissite 000-default    (Desactivar el default)
* root@chacka0101:/var/www/html/chacka0101.com# sudo a2ensite chacka0101.com   (Activar el virtual Host)
  *        Site chacka0101.com already enabled
* root@chacka0101:/var/www/html/chacka0101.com# sudo service apache2 restart    (Reiniciar el servicio de apache) 
* Abrimos un navegador y digitamos: localhost
![Alt Text](https://github.com/chacka0101/Kali_Linux_Certified_Professional/blob/master/chackavirtualhost.png?raw=true)

- .htaccess
1. Habilitar el .htaccess
  * root@chacka0101:/# sudo a2enmod rewrite
  * Enabling module rewrite.
  * root@chacka0101:/# sudo nano /etc/apache2/apache2.conf
 ```
 AccessFileName .htaccess (Descomentar la linea (remueve el simbolo #))
 
 <Directory /var/www/>
     Options Indexes FollowSymLinks
     AllowOverride All           (Reemplaza “None” por “All”: AllowOverride All)
     Require all granted
</Directory>
 ```
  * root@chacka0101:/# sudo service apache2 restart

2. Crear un directorio que quiera proteger por el .htaccess:
    * root@chacka0101:/var/www/html/chacka0101.com# mkdir privado   (Creamos un directorio privado)
    * root@chacka0101:/var/www/html/chacka0101.com# cd privado/
    * root@chacka0101:/var/www/html/chacka0101.com/privado# nano .htaccess    (Copiamos el siguiente codigo)
 ```
AuthName "Acceso solo usuarios autorizados"
AuthType Basic
require valid-user
AuthUserFile /etc/apache2/authfile/htpasswd-private
 ```
3. Crear un usuario y contraseña de acceso al .htaccess
    * root@chacka0101:/etc/apache2# mkdir authfiles
    * root@chacka0101:/etc/apache2# cd authfiles/
    * root@chacka0101:/etc/apache2/authfiles# nano htpasswd-private
    * root@chacka0101:/etc/apache2/authfiles# htpasswd /etc/apache2/authfiles/htpasswd-private root
    * New password: 
    * Re-type new password: 
    * Adding password for user root
    * root@chacka0101:/etc/apache2/authfiles# cat htpasswd-private
    * root:$apr1$DyqDCKm8$7Dk6m3Pe1qHN.xT5kvwfr0

4. Por último creamos un index.html en el directorio privado que aseguramos con .htaccess
 ```
 <html>
  <head>
    <title>Welcome to CHackA - Colombia Hack Agent</title>
  </head>
  <body>
    <h1>ACCESO PRIVADO de CHackA - Colombia Hack Agent</h1>
    Comprobando la seguridad del .htaccess!
  </body>
</html>
 ```
 5. Ingresamos al directorio privado:
 ![Alt Text](https://github.com/chacka0101/Kali_Linux_Certified_Professional/blob/master/chackahtaccess1.png?raw=true)
 - Acceso al área Privada
 ![Alt Text](https://github.com/chacka0101/Kali_Linux_Certified_Professional/blob/master/chackahtaccess2.png?raw=true)
 
Service Management
---
* Para ver una lista de todas las unidades activas que systemd conoce, podemos usar el comando list-units:
  * root@chacka0101:~# systemctl list-units
  * UNIT: El nombre de la unidad systemd.
  * LOAD: Si systemd ha analizado la configuración de la unidad. La configuración de las unidades cargadas se mantiene en la memoria.
  * ACTIVE: Un estado de resumen sobre si la unidad está activa. Esta suele ser una forma bastante básica de saber si la unidad se ha iniciado con éxito o no.
  * SUB: Este es un estado de nivel inferior que indica información más detallada sobre la unidad. Esto a menudo varía según el tipo de unidad, el estado y el método real en el que se ejecuta la unidad.
  * DESCRIPTION: Una breve descripción textual de lo que es / hace la unidad.
  * root@chacka0101:~# sudo systemctl start application.service
  * root@chacka0101:~# sudo systemctl stop application.service
  * root@chacka0101:~# sudo systemctl restart application.service
  * root@chacka0101:~# sudo systemctl reload application.service
  * root@chacka0101:~# sudo systemctl enable application.service
  * root@chacka0101:~# sudo systemctl disable application.service
  * root@chacka0101:~# systemctl status application.service
  * root@chacka0101:~# systemctl is-active application.service
  * root@chacka0101:~# systemctl is-enabled application.service
  * root@chacka0101:~# systemctl is-failed application.service
  * root@chacka0101:~# systemctl list-dependencies sshd.service   (Listar todas las depedependencias de un servicio)
  * root@chacka0101:~# systemctl show sshd.service (Listar todas las propiedades de un servicio)
- Systemd también tiene la capacidad de marcar una unidad como completamente inestable, automática o manualmente, al vincularla a /dev/null. Esto se denomina enmascarar la unidad, y es posible con el comando de máscara:
  * root@chacka0101:~# sudo systemctl mask sshd.service
  * root@chacka0101:~# sudo systemctl unmask sshd.service
  * root@chacka0101:~# systemctl list-unit-files   (Listar el estado)
- Más información: https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units


HELP - BUGS - ERRORES
--
  * root@chacka0101:~# man ls  (Manual para el comando ls)
  * root@chacka0101:~# apropos "copy file"  (Busca la palabra copy file dentro de Manuales y lista donde están contenidos)
  * root@chacka0101:~# yelp (Gnome Help)
  * root@chacka0101:~# apt install pinfo (Instalar pinfo)
  * root@chacka0101:~# pinfo (Interfaz gráfica de información de comandos)
  * root@chacka0101:~# cat /usr/share/doc/sqlmap/README.pdf  (Manual de paquete sqlmap, puede venir en diferentes formatos)
  * root@chacka0101:/# reportbug (Reportar un BUG)
  * root@chacka0101:/# reportbug sqlmap  (Reportar un BUG con un paquete en especifico)
  * root@chacka0101:/# dpkg -s sparta | grep ^Homepage:  (Página web oficial del paquete, ejemplo: sparta)
  * Homepage: https://github.com/SECFORCE/sparta
  * root@chacka0101:~# cat /usr/share/doc/paquete/copyright   (Buscar la página web oficial del paquete)
- Si el software devuelve un mensaje de error muy específico, ingréselo en un motor de búsqueda (entre comillas dobles, para buscar la frase completa, en lugar de las palabras clave individuales). En la mayoría de los casos, los primeros enlaces devueltos contendrán la respuesta que necesita.
  * Documentación específica de KALI LINUX: http://docs.kali.org/
  * kali-linux IRC Channel en Freenode
  * Foro Oficial de Kali Linux: https://forums.kali.org/
  * Página Oficial de Bugs de Kali Linux - Bug Tracker: http://bugs.kali.org 
  * Página Oficial de Bugs de Debian - Debbug: https://debbugs.gnu.org/
  * Los errores asociados a paquetes en Debian se pueden consultar tambien en: https://tracker.debian.org/pkg/sqlmap
- Un Fe de errata, se conoce como la publicación de errores posteriorES a la publicación final.
  * Rporte de Bugs en Github: https://help.github.com/en/articles/creating-an-issue
  * Averiguar la última versión de un paquete: http://pkg.kali.org/pkg/nmap

SECURITY - MONITORING
---
- fail2ban Bloquea la IP fuente de ataques despues de determinado número de intentos de ataques.
  * root@chacka0101:/# apt install fail2ban
- lnav Analiza los registros de eventos de Linux.
  * root@chacka0101:/# apt install lnav
  * root@chacka0101:/# service fail2ban stop
  * root@chacka0101:/# service fail2ban status
  * root@chacka0101:/# service fail2ban start
  * root@chacka0101:/# nano /etc/fail2ban/jail.conf
```
bantime = 10m (Tiempo de 10 minutos en que se va a tener una IP banneada)
findtime = 10m (Tiempo de 10 minutos en que se va a tener una IP banneada despues del numer de maxretry)
maxretry = 5  (Máximo numero de intentos en lo que bannea una IP)
Entre otras configuraciones como las de envío de alertas al correo.
```
  * root@chacka0101:/# lvan /var/log/fail2ban.log   (Iniciar el Analizador de Logs)
  
  root@chacka0101:~# apt install logcheck

  

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
 
35. You can use GNOME’s control center to graphically set network options with which tool?
NetworkManager

36. The interfaces file is an important part of command-line network configuration. What directory is it in?
/etc/network

37. What is the name of a command-line package typically used in Kali to configure the network from the command line?
ifupdown

38. When configuring a network from the command line (say with ifup or ifdown) which line will begin the section for a manual network configuration?
  * iface eth0 inet static

39. Which methods can be used to configure network devices in Kali Linux? Choose all that apply:
  * Graphically with NetworkManager
  * On the command line with .network files in the /etc/systemd/network directory
  * On the command line via the /etc/network/interfaces file
  * On the command line with systemd-networkd
  * On the command line with ifupdown

40. Which file contains encrypted user passwords?
/etc/shadow

41. Which command is used to add users to the system?
adduser

42. Which command will suspend a user account?
passwd -l olduser

43. Which is true of the SSH service on a default Kali install? Select all that apply.
  * The SSH service is disabled by default
  * The SSH service is installed by default
  * The default keys from a live image are pre-generated

44. Which command is commonly used to start services like ssh and postgresql?
systemctl

45. Which command can used to create a new postgresql database?
createdb

46. Which command is not a postgresql command?
pg_createuser

47. Which command will create a postgres database name db_new?
createdb -T template0 -E UTF-8 -O dbuser db_new

48. Which of the following are not associated with Apache2? Choose one.
systemctl start apache

49. Which of the following are not associated with Apache2?
apachectl

50. In Kali, what is responsible for the boot sequence, but also permanently acts as a full featured service manager, starting and monitoring services?
systemd

51. Which command will inspect the current status of the postgresql service?
systemctl status postgresql

52. Which command will determine if nmap has been modified by Kali?
All of the above

53. Which command is used to report a bug to the Debian developers?
reportbug

54. Which of these actions can be used to submit a bug to the Debian developers?
  * Use the official Debian bug tracker at https://bugs.debian.org
  * Send an email (with a special syntax) to submit@bugs.debian.org
  * Submit the bug to the official Kali bug tracker at https://bugs.kali.org and mark the issue for an upstream Debian patch.


  ---
© 2010 - 2019 - Jairo A. Garcia H. - GNU GPL. 
