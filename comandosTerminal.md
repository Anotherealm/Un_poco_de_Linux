
------------------------------------------------------------------------------------------------------
   __________  __  ______    _   ______  ____  _____    ________________  __  ________   _____    __ 
  / ____/ __ \/  |/  /   |  / | / / __ \/ __ \/ ___/   /_  __/ ____/ __ \/  |/  /  _/ | / /   |  / / 
 / /   / / / / /|_/ / /| | /  |/ / / / / / / /\__ \     / / / __/ / /_/ / /|_/ // //  |/ / /| | / /  
/ /___/ /_/ / /  / / ___ |/ /|  / /_/ / /_/ /___/ /    / / / /___/ _, _/ /  / // // /|  / ___ |/ /___
\____/\____/_/  /_/_/  |_/_/ |_/_____/\____//____/    /_/ /_____/_/ |_/_/  /_/___/_/ |_/_/  |_/_____/

-----------------------------------------------------------------------------------------------------


whoami 
: Permite conocer el usuario que se esta utilizando.
	|SINTAXIS| whoami

pwd 
	|DESCRIPCION| Muestra en pantalla la ruta del directorio de trabajo actual.
	|SINTAXIS| pwd [option] 
	|OPTIONS|
		-L : Muestra el directorio actual con enlace simbólico.
	 	-P : Muestra la dirección real (?).

uname 
	|DESCRIPCIÓN| Muestra en pantalla el nombre del sistema operativo.
	|SINTAXIS| uname [option]
	|OPTIONS|
		-a: Muestra en pantallla el sistema operativo y la arquitectura del sistema.

ls 
	|DESCRIPCIÓN| Permite listar el contenido de un directorio.
	|SINTAXIS| ls [option] <directorio-a-listar>
	|OPTIONS|
		-l Permite el formato de listado largo, mostrando información de los contenidos del directorio
		-a Permite listar los archivos ocultos del directorio. Los nombres de los directorios ocultos comienzan con un "."
		-h Permite una lectura más sencilla para conocer el espacio ocupado por los contenidos del directorio
		-r Invierte el orden del listado
		-i Muestra el número 		

cd
	|DESCRIPCIÓN| Permite cambiar el directorio de trabajo actual, por el directorio indicado.
	|SINTAXIS| cd [option] <directorio-a-cambiar>
	1. Si se utiliza cd sin un indicar un directorio-a-cambiar, redirige al directorio HOME.
	2. Si se utiliza cd <..>, el directorio de trabajo se dirije al directorio superior de la jerarquía.
	3. Si se utiliza cd <->, el directorio de trabajo se redirije al anterior fichero ingresado ($OLDPWD).
	4. Para especificar un directorio puede ocuparse RUTAS ABSOLUTAS o RUTAS RELATIVAS.
	5. Utilizar cd </> dirigira al directorio raiz.

-------------------------------------------CREAR ARCHIVOS--------------------------------------------------
Existen varias formas de crear archivos a través de la línea de comandos, como por ejemplo:
	-COMANDO cat-
 	Permite crear y fusionar (concatenar) texto, además de imprimir por pantalla el contenido de uno.
	|SINTAXIS| cat > <archivo.txt>
		*Permite ingresar texto de forma inmediata
		*Para salir de la edición del archivo se debe pulsar las teclas CTRL+D

	-COMANDO touch-
	Si es utilizado sin ningún parámetro, este creará uno o múltiples archivos de texto vacío.
	|SINTAXIS| touch <archivo.txt>
		   touch <archivo.txt> <archivo.txt> <archivo.txt>
		*Para crear múltiples archivos se deben separar por espacios.
	*Para agregar contenido al archivo creado puede utilizarse editores de texto.

	-Símbolo de redirección-
	Puede utilizarse el símbolo de redireccionamiento estándar para redirigir la salida de un comando a 
	un nuevo archivo.
	|SINTAXIS| > <archivo.txt>
		*Permite ingresar texto de forma inmediata.
		*Para salir de la edición se debe pulsar las teclas CTRL+D

	-CREACIÓN DE ARCHIVOS OCULTOS-
	Puede crearse archivos ocultos con las opciones mencionadas con anterioridad. Solo debe agregarse un 
	punto antes del nombre del archivo a crear.
	|SINTAXIS| touch .<nombre-archivo.txt>
		*También pueden crearse archivos ocultos dentro de un archivo llamado .hidden.
---------------------------------------------------------------------------------------------------------------

mkdir 
|DESCRIPCIÓN| Permite crear uno o varios nuevos directorios.
	|SINTAXIS| mkdir [option] <nuevo-directorio>
	1. Pueden crearse varios directorios independientes, utilizando espacios entre los nombres de los nuevos directorios.
		mkdir <nuevo-directorio1> <nuevo-directorio2> <nuevo-directorio3>
	2. mkdir ~: Crea un directorio en el directorio de inicio (HOME).
	3. mkdir .: Crea un directorio en el directorio actual (pwd).
	4. mkdir ..: Crea un directorio en el directorio superior.
	
	[OPTIONS]
		-p Permite crear subdirectorios

rm
	|DESCRIPCIÓN| Permite borrar archivos y directorios.
	|SINTAXIS| rm [option] <archivo-a-borrar>
	1. Por defecto, el comando rm no permite eliminar directorios. Para esto se utiliza la opción -r.
	2. Si se desea borrar un directorio vacío puede utilizarse el COMANDO rmdir.
	3. Pueden eliminarse varios archivos a la vez.
		rm <archivo1> <archivo2> <archivo3>
	[OPTIONS]
		-r Permite eliminar directorios de forma recursiva
		-f Fuerza la eliminación de un archivo o directorio.

cp
	|DESCRIPCIÓN| Permite copiar archivos o directorios.
	|SINTAXIS| cp [option] <archivos-original> <copia>
	1. Si se desea copiar el archivo en el mismo directorio de trabajo, solo debe indicarse el archivo-original y el nombre de la copia.
	2. Si se desea copiar el archivo en otro directorio, se debe indicar la ruta y nombre de la copia.
	[OPTIONS]
		-r Permite copiar de forma recursiva un directorio.

mv
	|DESCRIPCIÓN| Permite mover archivos o directorios de ubicación
	|SINTAXIS| mv <directorio/archivo-a-mover> <ruta-nueva-ubicación>

mv
	|DESCRIPCIÓN| Permite cambiar el nombre a un archivo o directorio.
	|SINTAXIS| mv <directorio-archivo> <nuevo-nombre>


----------------------------------------------------------------------------------------------------
			   __                 ______        __     
			  / /  ___ ___ ____  /_  __/____ __/ /____ 
			 / /__/ -_) -_) __/   / / / -_) \ / __/ _ \
			/____/\__/\__/_/     /_/  \__/_\_\\__/\___/
----------------------------------------------------------------------------------------------------                                          
----------------------------------------------------------------------------------------------------

less 
	|DESCRIPCIÓN| Programa de visualización de archivos de texto. Permite navegar por el 
		   archivo de manera interactiva, línea por línea o página por página.
	~Búsqueda de palabra: Presionar tecla "/" seguido de la palabra que se quiere buscar.
			      Presionar Enter para iniciar la búsqueda.
			      Presionar "n" para navegar entre las palabras encontradas.
			      Presionar "N" para navegar a la palabra anterior.

	~Salir del visor:     Presionar tecla "q"



more
	|DESCRIPCIÓN| Programa de visualización de texto. A diferencia de less, more imprime el 
	archivo de texto en pantalla y no lo borra al salir del visualizador.
	~ Salir del visor:    Presionar tecla "q"



head
	|DESCRIPCIÓN| Herramienta que permite leer las primeras líneas de un archivo de texto.
		      Por defecto, head imprime las primeras 10 líneas de texto.
	|SINTAXIS| head [archivo.txt]
	|OPCIONES|
		-n [número] : Muestra el número de líneas indicado.

tail
	|DESCRIPCIÓN| Herramienta que permite leer las últimas líneas de un archivo de texto.
		      Por defecto tail muestra las últimas 10 líneas de texto.
	|SINTAXIS| tail [archivo.txt]
	|OPCIONES|
		-n [número] : Muestra el número de líneas indicado.

sort
	|DESCRIPCIÓN| Permite ordenar líneas de texto en orden alfabético o numérico.
		      Por defecto, sort ordena las líneas en orden alfabético.
	|SINTAXIS| sort [archivo.txt]
	|OPCIONES|
		-r : Ordena las líneas en orden inverso
		-n : Ordena las líneas en orden númerico
		-f : Ignora las diferencias entre mayúsculas y minúsculas
		-u : Muestra sólo las líneas únicas

grep
	|DESCRIPCIÓN| Herramienta de búsqueda utilizada para buscar patrones especificos en un 
		      archivo de texto.
		      También, puede utilizarse para buscar patrones en la salida de otro comando.

	|Sintaxis| grep [OPCION] [PATRÓN] [archivo/s.txt]
	|OPCIONES|
		-v : Muestra las líneas que no coinciden con el patrón buscado
		-r : Busca de manera recursiva en los subdirectorios
		-l : Muestra sólo los nombres de los archivos que contienen el patrón
		-e : Especifica múltiples patrones para buscar
		-i : Ignora la diferencias entre mayúsculas y minúsculas
		-c : Muestra el número de veces que se encontró el patrón
		-n : Muestra el número de líneas en la que se encontró el patrón
		--exclude : Permite excluir ciertos archivos o tipos de archivos de la búsqueda
		-E : Habilita la utilización de expresiones regulares
cut
	|DESCRIPCIÓN| Herramienta que se utiliza para extraer o cortar secciones específicas de
		      líneas o columnas en un archivo de texto (output), o de la salida de 
		      otro comando.
		      'cut' recorta o separa una o varias columnas de texto utilizando un 
		      delimitador. Por defecto utiliza el carácter '\t' como delimitador.
	|SINTAXIS| cut [OPTION] [ARCHIVO.txt] 
	|OPCIONES|
		-d : Permite especificar el delimitador a utilizar (ej: cut -d ",")
		-f : Indica el campo o columna a extraer (ej: cut -f2 {extrae la 2da columna})
		-s : Suprime las líneas que no contienen el delimitador específicado.
		--complement : Extrae todas las columnas excepto las especificadas.

tr
	|DESCRIPCIÓN| Herramienta que permite traducir o transformar caracteres de entrada y 
		      reemplazarlos por otro conjunto de caracteres de salida.
		      Por ejemplo, 'tr' permite cambiar todas las letras minúsculas de una
		      cadena de texto a mayúsculas, o eliminar ciertos caracteres de una cadena 
		      de texto.
	|SINTAXIS| tr [OPCIONES] "caracteres-de-entrada" "caracteres-de-salida" 
	|OPCIONES|
		-d : Elimina los caracteres especificados del conjunto de entrada

column
	|DESCRIPCIÓN| Herramienta utilizada para formatear la salida de texto en columnas.
		      Su función principal es tomar una secuencia de entrada y distribuirla en
		      columnas, con un separador especificado.
	|SINTAXIS| column [OPCION] [ARCHIVO.txt]
	|OPCIONES|
		-t : Utiliza la primera fila como emcabezados de la tabla
		-s : Especifica el separador de columnas
		-o : Especifica el separador de salida

awk
	|DESCRIPCIÓN| Herramienta utilizada para procesar y manipular datos de texto. 
		      
		      Permite  buscar información específica, filtrar datos, manipular el 
		      formato de los datos y realizar calculos y estadísticas en ellos
	|SINTAXIS| awk [OPCION] 'patrón {acción}' archivo.txt
	|OPCIONES|
		-F : Especificar el delimitar de campo
		-v : Define una variable que puede utilizarse en el script de "awk"

sed
	|DESCRIPCION| Herramienta que se utiliza para manipular y transformar archivos de 
		      texto. 
		      Los cambios pueden ser realizados sin la necesidad de utilizar un editor 
		      de texto.
		      Pueden realizarse cambios en varios archivos a la vez, o automatizar un 
		      proceso de edición de archivos de texto.

	|SINTAXIS| sed [opciones] [comando] [archivo(s)]
	|OPCIONES| 
		-i : Modifica el archivo de entrada directamente. Los cambios realizados  se 
		     guardarán en el archivo original
		-e : Permite especificar varias líneas de comandos separador por (;)
		|COMANDOS|
			‘s’ : Sirve para sustituir una cadena de texto.
			‘d’ : Elimina la línea actual del archivo.
			‘p’ : Imprime la línea actual del archivo.
			‘a\texto_a_agregar’ : Agrega el ‘texto_a_agregar’ después de la línea actual.
			‘g’ : se utiliza para realizar el remplazo de forma recursiva.
			‘i’ : Inserta una nueva línea antes de la línea actual.
			‘c’ : Reemplaza la línea actual con una nueva línea.
			‘y’ : Realiza una traducción de caracteres.

wc
	|DESCRIPCION| Herramienta utilizada para contar el número de líneas palabras y 
		      caracteres en un archivo de texto.

	|SINTAXIS| wc [opciones] [archivo(s)]

	|OPCIONES|  
		-l : Sólo cuenta el número líneas.
		-w : Sólo cuenta el número de palabras.
		-c : Sólo cuenta el número de caracteres.
		-m : Sólo cuenta el número de caracteres de ancho de bytes.
		-L : Muestra la longitud de la línea más larga del archivo.

