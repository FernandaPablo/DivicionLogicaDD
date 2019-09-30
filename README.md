# DivicionLogicaDD
ESTRUCTURA  LÓGICA DE UN DISCO DURO:
La estructura  lógica  de un disco duro está formado por:
	Sector de arranque.
	Espacio particionado.
	Espacio sin particionar.
Sector de arranque: Es el primer sector de un  disco duro en él se almacena la tabla de particiones y un  programa  pequeño llamado Master Boot. Este programa se encarga de  leer la tabla de particiones y ceder el control al sector de  arranque de la partición activa, en caso de que no  existiese partición activa mostraría un mensaje de  error.
Espacio particionado: Es el espacio del disco que  ha sido asignado a alguna partición.
Espacio sin particionar: Es el espacio del disco  que no ha sido asignado a ninguna partición.
A su vez la estructura lógica de los discos    duros internamente se pueden dividir en varios volúmenes    homogéneos dentro de cada volumen se    encuentran una estructura que bajo el sistema    operativo MS-DOS es el    siguiente:
Cada zona del volumen acoge estructuras de datos del  sistema de archivos y también los diferentes archivos y  subdirectorios. No es posible decir el tamaño de las  diferentes estructuras ya que se adaptan al tamaño del  volumen correspondiente.
A continuación vamos a definir cada una de las  estructuras mostrada en el cuadro.
1.-Sector de arranque (BOOT): En el sector de  arranque se encuentra la información acerca de la  estructura de volumen y sobre todo del BOOTSTRAP-LOADER, mediante  el cual se puede arrancar el PC desde el DOS. Al formatear un  volumen el BOOT se crea siempre como primer sector del volumen  para que sea fácil su localización por el  DOS.
2.-Tabla de asignación de ficheros (FAT): La FAT se encarga de informar al DOS que sectores del volumen  quedan libres, esto es por si el DOS quiere crear nuevos archivos  o ampliar archivos que ya existen. Cada entrada a la tabla se  corresponde con un número determinado de sectores que son  adyacentes lógicamente en el volumen.
3.-Uno o más copias de la FAT: El DOS  permite a los programas que  hacen el formateo crear una o varias copias idénticas de  la FAT, esto va a ofrecer la ventaja de que se pueda sustituir la  FAT primaria en caso de que una de sus copias este defectuosa y  así poder evitar la pérdida de datos.
4.-Directorio Raíz: El directorio  raíz representa una estructura de  datos estática,  es decir, no crece aún si se guardan más archivos o  subdirectorios. El tamaño del directorio raíz esta  en relación al volumen, es por eso que la cantidad  máxima de entradas se limita por el tamaño del  directorio raíz que se fija en el sector de  arranque.
5.-Zona de datos para archivos y subdirectorios: Es la parte del disco duro donde se almacenan los datos de un  archivo. Esta  zona depende casi en su totalidad de las interrelaciones entre  las estructuras de datos que forman el sistema de archivos del  DOS y del camino que se lleva desde la FAT hacia los diferentes  sectores de un archivo.

