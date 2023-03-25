{SPDX-License-Identifier: 1
SPDX-FileCopyrightText: 2023 Dylan chaves}
# Sistema Operativo Windows

> ### Temas abarcados

| Objetivo                              |        Objetivo del tema                                   |
|---------------------------------------|------------------------------------------------------------|
|   Historia de Windows                 |   Describa la historia del sistema operativo Windows.      |  
|  Arquitectura y operaciones de Windows|   Explique la arquitectura de Windows y su funcionamiento. | 
|  Seguridad de Windows                 | Explique cómo puede mantenerse seguro Windows.             |  
|  Configuracion y monitoreo de Windows                                     |    Explique como configurar y monitorear Windows.                                                        |

## Sistema operativo de disco <br> (DOS)
 Los primeros métodos de almacenamiento utilizaban tarjetas perforadas, cinta de papel, cinta magnética y hasta casetes de audio.
almacenamiento en disquete y disco duro requiere un software para leer, escribir y administrar los datos que se almacenan.

> #####   DOS provee un sistema de archivos que organiza los archivos en una forma especifica en el disco. 
> #####  MS-DOS utiliza una línea de comandos como interfaz para que las personas creen programas y manipulen archivos de datos

Con MS-DOS, la computadora tenía conocimientos básicos sobre cómo acceder a la unidad de disco y cargar los archivos del sistema operativo directamente desde el disco como parte del proceso de arranque. Cuando se cargaba, MS-DOS podía tener acceso al disco fácilmente porque estaba incorporado en el sistema operativo.

Windows consistían en un Interfaz Gráfica de Usuario (GUI) que se ejecuta sobre MS-DOS, iniciando con Windows 1.0 en 1985

 > Un sistema operativo moderno, como Windows 10, no se considera un sistema operativo de disco. Se basa en Windows NT ( new tecnologys ).
El Sistema operativo controla directamente la computadora y su hardware
compatible con múltiples procesos de usuario. __Esto es muy diferente al MS-DOS de un solo proceso y un solo usuario.__ 

# Versiones de Windows
Desde el año 1993 hubo más de 20 versiones de Windows basadas en el sistema operativo NT. La mayoría de estas versiones eran para uso del público general y las empresas.
Esto ocurrió porque muchas ediciones se diseñaron específicamente para estaciones de trabajo, profesionales, servidores, servidores avanzados y servidores de centro de datos,entre otros.
 > Windows XP, comenzó a estar disponible una edición de 64 bits. __El sistema operativo de 64 bits era una arquitectura totalmente nueva__
 
 Tenía un espacio para la dirección postal de 64 bits, en lugar de uno de 32 bits. Esto no significa solamente el doble de espacio, ya que estos bits son números binarios. Mientras que Windows de 32 bits tiene espacio para un poco menos de 4 GB de RAM, Windows de 64 bits puede tener, teóricamente, espacio para 16,8 millones de terabytes.
 
 - los sistemas operativos de 64 bits son compatibles con programas más antiguos de 32 bits, pero los programas de 64 bits no pueden ejecutarse en el hardware más antiguo de 32 bits.
 
| SO  | Versiones   |
|---|---|
| Windows 7 |  Starter, Home Basic, Home Premium, Professional, Enterprise, Ultimate |
| Windows Server  2008 | Foundation, Standard, Enterprise, Datacenter, Web Server, HPC Server y para sistemas con procesadores Itanium  |
| Windows Home Server 2011   |  No versiones |
| Windows 8  | Windows 8, Windows 8 Pro, Windows 8 Enterprise, Windows RT  |
| Windows Server 2012 | Foundation, Essentials, Standard, Datacenter |
|  Windows 8.1        | Windows 8.1, Windows 8.1 Pro, Windows 8.1 Enterprise, Windows RT 8.1
|   Windows Server 2012 R2    | Foundation, Essentials, Standard, Datacenter
|   Windows 10 | Home, Pro, Pro Education, Enterprise, Education, IoT Core, Mobile, Mobile Enterprise
|   Windows Server 2016            | Essentials, Standard, Datacenter, Multipoint Premium Server, Storage Server, Hyper-V Server

# GUI de Windows (Interfaz Gráfica de Usuario)

Para que los usuarios trabajen con software y archivos de datos. La interfaz gráfica de usuario tiene un área principal que es conocida como el Escritorio.

# Vulnerabilidades en el sistema operativo

Los sistemas operativos consisten en millones de líneas de código. El software instalado también puede contener millones de líneas de código. No hay sistema seguro.
Las vulnerabilidades son  una imperfección o debilidad que puede ser aprovechada por un atacante para reducir la viabilidad de la información de una computadora. Para aprovechar una vulnerabilidad de un sistema operativo, el atacante debe utilizar una técnica o herramienta para atacarla.

> $$  Recomendaciones..Comunes
 
-  ####  Proteccion contra virus o malware
   - Windows Defender ofrece un conjunto de herramientas de protección incorporado en el sistema. Windows lo utiliza de forma predeterminada
   - Hay muchos antivirus que pueden ser de utilidad.
   
- #### Servicios Desconocidos o no administrados
    - Existen muchos Servicios ejecutandose en segundo plano 
    - Identificar que todos los sean seguros

- #### Cifrado
  - Si los datos no estan cifrados pueden ser facilmente recolectados.
  
- #### Politicas 
  - Cumpliendo una buena politica de seguridad, puede prevenir futuros ataques.
  
# Modo usuario y modo Kernel
  Cualquier aplicacion instalada se ejecuta en el modo usuario, y el codigo del sistema operativo  lo hace en modo Kernel. 
El código del modo de núcleo también puede hacer referencia a cualquier dirección de la memoria directamente,un error detiene el funcionamiento de la pc. 
  Dado que suele estar reservado para las funciones más confiables del sistema operativo .Las aplicaciones de usuario se ejecutan en modo de usuario y no tienen acceso directo a ubicaciones de memoria o hardware,gracias a esto un error solamente afectaria a la aplicacion.
> Cuando se ejecuta código en el modo de usuario, el núcleo le otorga su propio espacio para la dirección postal limitado, junto con un proceso creado específicamente para la aplicación. Esto se hace, principalmente, para evitar que las aplicaciones cambien código del sistema operativo que se esté ejecutando al mismo tiempo.

# Inicio de Windows
 Hay dos elementos importantes del registro que se utilizan para iniciar automáticamente aplicaciones y Servicios
 > __HKEY_LOCAL_MACHINE = Configuración de Windows se almacenan en esta clave, incluida la información sobre los servicios que se inician con cada arranque.__
 > 
 > __HKEY_CURRENT_USER =  almacenan varios aspectos relacionados con el usuario que ha iniciado sesión, incluida la información sobre los servicios que se inician solo cuando el usuario inicia sesión en la computadora.__ 
>
usar la herramienta Msconfig.exe. Esta herramienta se utiliza para ver y cambiar todas las opciones de inicio de la computadora. 
Permite modificar que servicios se ejecuten,el modo de inicio,y muestra muchas herramientas del sistema.

# Procesos, subprocesos y servicios
- Una aplicación de Windows se compone de procesos. La aplicación puede tener uno o varios procesos exclusivos. Un proceso es cualquier programa que se esté ejecutando. Cada proceso en ejecución está compuesto de, al menos, un subproceso.

El procesador realiza los cálculos en el subproceso. Para configurar los procesos de Windows, existe el administrador de tareas.

  
> ![administrador de tareas](https://www.howtogeek.com/wp-content/uploads/2019/03/img_5c9aa895b7f8b.png?trim=1,1&bg-color=000&pad=1,1)

> Algunos de los procesos que ejecuta Windows son servicios. Son programas que se ejecutan en segundo plano para respaldar el funcionamiento del sistema operativo y de las aplicaciones. 


##### Servicios proporcionan funcionalidades de duración prolongada, como la conexión inalámbrica o el acceso a un servidor FTP. 
para configurar los servicios de Windows se utiliza la herramienta "servicios"

![Servicios](https://www.thewindowsclub.com/wp-content/uploads/2016/06/How-to-open-Windows-Services.png)

# El registro de Windows
Windows almacena toda la información sobre el hardware, las aplicaciones, los usuarios y la configuración del sistema en una extensa base de datos conocida como el Registro
| Colmena de registro. | Descripción |
|:---:|:---:|
| HKEY_CURRENT_USER (HKCU) | Contiene información sobre el usuario actualmente conectado. |
| HKEY_USERS (HKU) | Contiene información sobre todas las cuentas de usuario en el host. |
| HKEY_CLASSES_ROOT (HKCR) | Contiene  información sobre los registros de vinculación e incrustación de  objetos (OLE). OLE permite a los usuarios incrustar objetos de otras  aplicaciones (como una hoja de cálculo) en un solo documento (como un  documento de Word). |
| HKEY_LOCAL_MACHINE (HKLM) | Contiene información relacionada con el sistema. |
| HKEY_CURRENT_CONFIG (HKCC) | Contiene información sobre el perfil de hardware actual. |

# Configuración y monitoreo de Windows

### -  Ejecutar como administrador

Como mejor práctica de seguridad, no es recomendable iniciar sesión en Windows utilizando la cuenta de administrador o una cuenta con privilegios administrativos,ya que cualquier aplicacion cuando se ejecute hereda estos privilegios 

### - Usuarios y dominios locales
Al instalar Windows, el sistema solicita la creación de una cuenta de usuario. Esta se conoce como “usuario local”. Esta cuenta contiene todos los ajustes de personalización, los permisos de acceso, las ubicaciones de archivos y muchos otros datos específicos del usuario.
práctica de seguridad, no debe habilitarse la cuenta de administrador ni otorgarles privilegios administrativos a los usuarios estándar. Si un usuario necesita realizar cualquier función que requiera privilegios administrativos, el sistema solicitará la contraseña de administrador y permitirá realizar como administrador solamente la tarea específica. Windows utiliza grupos. Un grupo tendrá un nombre y un conjunto específico de permisos asociados con él.

Los usuarios y grupos locales se administran con el applet del panel de control lusrmgr.msc
sdfdf
![grupos_usuarios](https://renenyffenegger.ch/notes/Windows/dirs/Windows/System32/users.png)
Un dominio es un tipo de servicio de red en el que todos los usuarios, grupos, computadoras, periféricos y ajustes de seguridad se almacenan en una base de datos, que también los controla.

# CLI y Powershell
La interfaz de línea de comandos (Command Line Interface, CLI) de Windows se puede utilizar para ejecutar programas, navegar por el sistema de archivos y administrar archivos y carpetas.  denominada como [CMD.exe]

Se puede utilizar otro entorno, llamado Windows PowerShell, para crear script con el fin de automatizar tareas que la CLI común no puede crear. PowerShell también proporciona una CLI para iniciar comandos.

### - Comando net 

Windows tiene muchos comandos que se pueden introducir en la línea de comando. Un comando importante es el comando net, que se usa en la administración y el mantenimiento del sistema operativo. El comando net puede soportar muchos otros comandos, que siguen el net y puede combinarse con switches para concentrarse en resultados específicos.


|    Comando   |                                         Descripción                                        |
|:------------:|:------------------------------------------------------------------------------------------:|
| net accounts | Define los requisitos de contraseñas e inicio de sesión para los usuarios                  |
| net session  | Enumera o desconecta las sesiones entre una computadora y otras computadoras de la red     |
| net share    | Crea, elimina o administra recursos compartidos                                            |
| net start    | Inicia un servicio de red o enumera los servicios de red en ejecución                      |
| net stop     | Detiene un servicio de red                                                                 |
| net use      | Conecta, desconecta los recursos de red compartidos, y permite ver información sobre ellos |
| net view     | Muestra una lista de las computadoras y los dispositivos de red en la misma                |

# Windows Server
En centros de datos se utiliza principalmente otra versión de Windows: Windows Server.
Windows Server aloja muchos servicios diferentes y puede cumplir diferentes roles dentro de una empresa.

    - Servicios de red- DNS, DHCP, Terminal Services, controladora de red y virtualización de red en Hyper-V
    - Servicios de archivo- SMB, NFS y DFS
    - Servicios web- FTP, HTTP y HTTPS
    - Administración- política de grupo y control de servicios de dominio de Active Directory

# Visor de eventos
Visor de eventos de Windows registra el historial de eventos del sistema, de aplicaciones y de seguridad. Proporciona información necesaria para identificar un problema.
Windows incluye dos categorías de registros de eventos: registros de Windows y registros de aplicaciones y servicios.
 Los eventos que aparecen en estos registros tienen un nivel: información, advertencia, error o crítico. 
 
![visor_eventos](https://www.solvetic.com/uploads/monthly_01_2017/tutorials-9832-0-47630400-1483359267.png)

# Política de seguridad local
Política de seguridad es un conjunto de objetivos de seguridad que garantiza la seguridad de una red, los datos y los sistemas informáticos en una organización.
El administrador configura una política de seguridad de dominio que se aplica a todas las computadoras que se unen al dominio. Las políticas de cuentas se configuran automáticamente cuando un usuario inicia sesión en una computadora que es miembro de un dominio.

![politica_seguridad](https://directivasdeseguridadw7.files.wordpress.com/2013/06/ventana-d-directivas.jpg)

# Windows Defender
El malware incluye virus, gusanos, troyanos, registradores de teclado, spyware y adware. Estos están diseñados para invadir la privacidad, robar información y dañar la computadora o los datos.
Los siguientes tipos de software antimalware se encuentran disponibles

 - Protección antivirus - Este programa monitorea continuamente en busca de virus. Cuando se detecta un virus, se advierte al usuario y el programa intenta eliminar el virus o ponerlo en cuarentena.
 -   Protección contra adware - Este programa busca constantemente programas que muestran anuncios publicitarios en la computadora.
 -   Protección contra suplantación de identidad - Este programa bloquea las direcciones IP de sitios web conocidos por realizar suplantación de identidad y advierte al usuario acerca de sitios sospechosos.
 -   Protección contra spyware - Este programa analiza la computadora en busca de programas que registren claves y otro tipo de spyware.
 -   Fuentes confiables o no confiables - Este programa le advierte si está por instalar programas inseguros o visitar sitios web inseguros.

# Firewall de Windows Defender

firewall deniega selectivamente el tráfico a una PC o a un segmento de red. Los firewalls suelen actuar abriendo y cerrando los puertos que utilizan diversas aplicaciones. Al abrir solo los puertos requeridos en un firewall, se implementa una política de seguridad restrictiva. 
En cambio, una política de seguridad permisiva permite el acceso a través de todos los puertos, excepto aquellos que estén explícitamente denegados. 

![firewall](https://support.content.office.net/es-es/media/739c07da-e850-b2df-73fb-44d77c7fc0c0.png)

---
# Linux
>     $  ~: help linux   
¿Qué es Linux? 
 Linux es un sistema operativo creado en 1991. Linux es de código abierto, rápido, confiable y pequeño. Requiere muy pocos recursos de hardware para ejecutarse y tiene muchas opciones para ser personalizado.
 
Linux es que está diseñado para conectarse a la red, lo que facilita mucho la escritura y el uso de aplicaciones con base en la red. Dado que Linux es de código abierto, cualquier persona o empresa puede obtener el código fuente del kernel, examinarlo, modificarlo y volver a compilarlo cuando lo desean. También pueden redistribuir el programa con o sin costo.
Una distribución de Linux es el término que se utiliza para describir paquetes creados por distintas organizaciones

#### Linux es, a menudo, el sistema operativo elegido en el Centro de Operaciones de Seguridad (SOC)
La flexibilidad que proporciona Linux es una característica grandiosa para el SOC. Todo el sistema operativo se puede adaptar para convertirlo en la plataforma perfecta de análisis de seguridad. Por ejemplo, los administradores pueden agregar al sistema operativo solamente los paquetes necesarios para hacerlo rápido y eficiente.
 
### El Shell de Linux
El usuario se comunica con el sistema operativo mediante la CLI o GUI. Linux a menudo se inicia en la GUI de forma predeterminada. Esto oculta la CLI del usuario. Una manera de tener acceso a la CLI desde la GUI es mediante una aplicación de emulación de terminales. Estas aplicaciones permiten que el usuario tenga acceso a la CLI y, generalmente, se denominan con alguna variación de la palabra “terminal”. En Linux, los emuladores de terminal comunes son Terminator, eterm, xterm, konsole y gnome-terminal.

### Comandos basicos
Los comandos de Linux son programas creados para realizar una tarea específica. Usar el comando man (manual corto) para obtener documentación sobre los comandos. Por ejemplo, man ls proporciona documentación sobre el comando ls del manual del usuario.

cuando un usuario escribe un comando, el shell debe encontrarlo en el disco antes de poder ejecutarlo. El shell busca comandos escritos por el usuario en directorios específicos e intenta ejecutarlos. La lista de directorios en la que busca el shell se denomina ruta. 
| Comando 	| Descripcion 	|
|:---:	|:---:	|
| mv 	| Mueve o cambia el nombre de archivos y directorios 	|
| chmod 	| Modifica los permisos de archivos 	|
| chown 	| Cambia la propiedad de un archivo 	|
| dd 	| Copia datos de una entrada a un resultado 	|
| pwd 	| Muestra el nombre del directorio actual 	|
| ps 	| Enlista los procesos del sistema que están actualmente en ejecución 	|
| su 	| Simula un inicio de sesión como otro usuario o para convertirse en usuario avanzado 	|
| sudo 	| Ejecuta un comando como superusuario, de forma predeterminada, u otro usuario con nombre 	|
| grep 	| Se  utiliza para buscar cadenas de caracteres específicas dentro de un  archivo o de las salidas de otros comandos. Para buscar en el resultado  de un comando anterior, grep se debe anexar al final del comando anterior. 	|
| ifconfig 	| Se utiliza para mostrar o configurar la información relacionada con la tarjeta de red. Si se emite sin parámetros, ifconfig  mostrará la configuración actual de las tarjetas de red. Nota: Aunque  todavía está ampliamente en uso, este comando está en desuso. Utilice la  ip address en su lugar. 	|
| apt-get 	| Se utiliza para instalar, configurar y eliminar paquetes en Debian y sus derivados. Nota: apt-get es una línea de comando front-end fácil de usar para dpkg, Debian administrador de paquetes. La combinación de dpkg y apt-get es el sistema predeterminado del administrador de paquetes en todos los derivados de Debian Linux, incluido Raspbian. 	|
| iwconfig 	| Se utiliza para mostrar o configurar la información relacionada con la tarjeta de red inalámbrica. Al igual que ifconfig, iwconfig mostrará información de la conexión inalámbrica cuando se emita sin parámetros. 	|
| shutdown 	| Apaga el sistema, shutdown  puede recibir la orden de realizar diversas tareas relacionadas con el  apagar, incluido reiniciar, detener, suspender o expulsar de todos los  usuarios conectados actualmente. 	|
| passwd 	| Se utiliza para cambiar la contraseña. Si no se proporcionan parámetros, passwd cambia la contraseña del usuario actual. 	|
| cat 	| Se utiliza para enumerar el contenido de un archivo y espera el nombre de archivo como parámetro. El comando cat  suele utilizarse en los archivos de texto. 	|
| man 	| Se utiliza para mostrar la documentación para un comando específico. 	|

En Linux, todo se trata como un archivo. Esto incluye la memoria, los discos, el monitor y los directorios. Por ejemplo, desde el punto de vista del sistema operativo, mostrar información en pantalla significa escribir en el archivo que representa el dispositivo de pantalla. No debería sorprendernos que la propia computadora esté configurada mediante archivos. Estos archivos, conocidos como archivos de configuración, suelen ser archivos de texto utilizados para almacenar ajustes y configuraciones de aplicaciones o servicios específicos. prácticamente todo depende de archivos de configuración para funcionar. Algunos servicios no tienen solo uno, sino varios archivos de configuración.

### Servidores

Los servidores son computadoras con software instalado que les permite ofrecer servicios a los clientes a través de la red. Existen muchos tipos de servicios. Algunos proporcionan recursos externos a los clientes cuando lo solicitan, como archivos, mensajes de correo electrónico o páginas web. 

En orden para que una computadora pueda ser el servidor para múltiples servicios, se utilizan los puertos. Un puerto es un recurso de red reservado utilizado por un servicio. Se dice que un servidor “escucha” en un puerto cuando se asocia a dicho puerto.

| Puerto 	| Descripción 	|
|:---:	|:---:	|
| 20/21 	| Protocolo de transferencia de archivos (FTP)  	|
| 22 	| Secure Shell (SSH)  	|
| 23 	| Servicio de inicio de sesión remoto de Telnet  	|
| 25 	| Protocolo Simple de Transferencia de Correo (SMTP)  	|
| 53 	| Sistema de Nombres de Dominio (DNS)  	|
| 67/68 	| Protocolo de Configuración Dinámica de Host (DHCP) 	|
| 69 	| Protocolo Trivial de Transferencia de Archivos (TFTP) 	|
| 80 	| Protocolo de Transferencia de Hipertexto (HTTP)  	|
| 110 	| Protocolo de Oficina de Correos, versión 3 (POP3)  	|
| 123 	| Protocolo de Tiempo de Red (NTP)  	|
| 143 	| Protocolo de Acceso a Mensajes de Internet (IMAP)  	|
| 161/162 	| Protocolo Simple de Administración de Redes (SNMP)  	|
| 443 	| HTTP Seguro (HTTPS) 	|

### Clientes
Los clientes son programas o aplicaciones cuyo objetivo es comunicarse con un tipo de servidor específico.

Los Navegadores Web son clientes web utilizados para comunicarse con servidores web mediante el Protocolo de Transferencia Hyper (HTTP) en el Puerto 80. El cliente del Protocolo de Transferencia de Archivos (FTP) es un software utilizado para comunicarse con un servidor FTP.

### Configuracion de servicios
 Los servicios se administran por medio de archivos de configuración. Las opciones frecuentes en la configuración de archivos son números de puertos, localización de los recursos alojados y detalles de autorización del cliente. Cuando el servicio se inicia, busca sus archivos de configuración, los carga en la memoria y se ajusta conforme a la configuración presente en los archivos

### Monitoreo de registros de servicios

Todos los eventos del Kernel, los servicios y las aplicaciones se registran en los archivos de registro. Es muy importante que un administrador revise periódicamente los registros de una computadora para mantenerla libre de problemas. Mediante el monitoreo de archivos de registro de Linux

Se clasifican en 4 categorias:

    - Registros de aplicaciones
    - Registros de eventos
    - Registros de servicios
    - Registros del sistema

### Roles de Linux y Permisos de Archivo
Se trata a la mayoría de las entidades de sistema como archivos. Con el objetivo de organizar el sistema y reforzar los límites dentro de la computadora, Linux usa permisos de archivos. Los permisos de archivos están integrados en la estructura del sistema de archivos y proporcionan un mecanismo para definir los permisos de cada archivo. Cada archivo en Linux trae sus permisos de archivo, los cuales definen las acciones que el propietario, el grupo y otros puede hacer con el archivo. Los posibles permisos son leer, escribir y ejecutar. 

-  El guion (-) indica que se trata de un archivo. En el caso de los directorios, el primer guion se reemplazaría por una “d”.
 -   El  primer set de caracteres es para  permisos de usuario (rwx). , de quien es el  documento, can Read, Write and eXecute the file.
 - El segundo conjunto de caracteres es para permisos de grupo (rwx). El grupo, analista, propietario del archivo puede leer y ejecutar WX el archivo.
- El tercer conjunto de caracteres es para cualquier otro usuario o permiso de grupo (rwx). Cualquier otro usuario o grupo en la computadora solo puede analistaRWXejecutar el archivo.

### Enlaces físicos y enlaces simbólicos
Un enlace rígido es otro archivo que apunta a la misma ubicación que el archivo original. Usar el comando ln para crear un enlace rígido El primer argumento es el archivo existente y, el segundo, el archivo nuevo

Un enlace simbólico, también llamado enlace suave o symlink, es similar a un enlace físico en el sentido en que aplicar cambios a un enlace simbólico también cambia el archivo original.

### La GUI de linux
un sistema operativo no necesita una GUI para funcionar, las GUI se consideran más fáciles de usar que la CLI. El usuario puede reemplazar fácilmente la GUI de Linux en su totalidad. Como resultado de la gran cantidad de distribuciones de Linux

### Procesos y Bifurcaciones
Un proceso es una instancia en ejecución de un programa informático. Los sistemas operativos multitarea pueden ejecutar varios procesos al mismo tiempo.
El plegamiento es un método que utiliza el kernel para permitir que un proceso cree una copia de sí mismo. Los procesos necesitan una manera de crear nuevos procesos en los sistemas operativos multitarea. La bifurcación es la única manera de lograr esto en Linux.

Cuando un proceso solicita la bifurcación, el proceso que realiza la solicitud se convierte en el proceso principal, y el proceso recién creado se denomina subproceso. Después de la bifurcación, los procesos son, en cierta medida, independientes; tienen diferentes identificaciones, pero ejecutan el mismo código de programa.

### Malware en linux,existen? #no_system_is_safe
El malware de Linux incluye virus, troyanos, gusanos y otros tipos de malware que pueden afectar el sistema operativo. Debido a una serie de componentes del diseño, como la estructura del sistema de archivos, los permisos de archivos y las restricciones de las cuentas de usuario, es habitual considerar que los sistemas operativos Linux tienen mejor protección contra malware.

Está mejor protegido,pero  Linux no es inmune al malware. Se han encontrado y aprovechado muchas vulnerabilidades en Linux, desde vulnerabilidades en el software de servidor hasta vulnerabilidades en el kernel.Si se ejecuta un programa malicioso, causará daños, independientemente de la plataforma. Un vector de ataque común en Linux son sus servicios y procesos. 

### Comprobación de Rootkit

rootkit es un tipo de malware diseñado para aumentar los privilegios de un usuario no autorizado u otorgar acceso a partes del software que no suelen estar disponibles. Los rootkit también suelen usarse para asegurar el ingreso a una puerta trasera de una computadora atacada.

Un atacante puede instalarlo manualmente después de atacar una computadora. Un rootkit es destructivo porque cambia el código del kernel y sus módulos, lo que afecta las operaciones más fundamentales del sistema operativo propiamente dicho. Con un nivel tan profundo de ataque, los rootkits pueden ocultar la intrusión, eliminar cualquier rastro de su instalación e incluso manipular las herramientas de solución de problemas y diagnóstico para que oculten la presencia del rootkit en sus resultados. 

La detección de rootkits puede ser muy difícil. Los métodos de detección típicos suelen incluir arrancar la computadora desde medios confiables, como un CD con el sistema operativo de diagnóstico ejecutado en directo. Se monta la unidad afectada y, desde el conjunto seguro de herramientas del sistema, es posible iniciar herramientas de diagnóstico confiables para inspeccionar el sistema de archivos atacado. Los métodos de inspección incluyen métodos basados en el comportamiento, y análisis de firmas, diferencias y volcado de memoria.

### Comandos de tuberias
    [analyst@secOps ~]$ ls -l | grep file
    ls -l | grep [archivo]
     |  <- seria la tuberia(barra vertical)
    
Los dos comandos, ls y grep, se pueden canalizar juntos para filtrar la salida de ls. Esto se muestra en la salida del comando ls -l | grep host y el comando ls -l | grep file.
Es un procedimiento que consiste en vincular comandos entre sí, de manera que el resultado de un comando alimente la entrada de otro.
