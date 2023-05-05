	   ___           __                
	  / _ )___ ____ / /                
	 / _  / _ `(_-</ _ \               
	/____/\_,_/___/_//_/__  _          
	  / __/__________  / /_(_)__  ___ _
	 _\ \/ __/ __/ _ \/ __/ / _ \/ _ `/
	/___/\__/_/ / .__/\__/_/_//_/\_, / 
        	   /_/              /___/  

---
**Bash script** es un lenguaje de scripting que se utiliza para escribir scripts o secuencias 
de comandos en un shell basado en Unix. Permite escribir scripts sencillos para *automatizar tareas,
procesar datos, entre otros*. 

Los scripts pueden *contener variables, bucles, condicionales, funciones* y otros elementos que 
se encuentran en los lenguajes de programación tradicionales.

### Crear un Bash Script

Para crear un Bash Script primero debemos crear un archivo con formato *.sh*. El archivo puede 
ser editado con cualquier editor de texto que se desee.

Para iniciar, y respetando las buenas prácticas, se debe indicar la ruta completa del 
intérprete de comandos, antecedido por los caracteres *#!*. Para bash la ruta absoluta 
corresponde a **/bin/bash**. Esto se conoce como *shebang*

```bash

#! /bin/bash

```

### Ejecutar Script

Al crear un archivo.sh, por defecto, no se tendran los permisos para poder ejecutarlo.
Para esto debemos cambiar sus permisos por medio del comando **chmod**.

```bash

sudo chmod +x nombre_script.sh

```

El comando *chmod* permite cambiar los permisos a un archivo o directorio, el parámetro
*+u* indica que los permisos de ejecución son asignados al *archivo.sh*

Para ejecutar un script debemos situarnos en el directorio donde se ubica, para así 
ejecutar el siguiente comando.

```bash

./nombre_script.sh

```


### Comentarios en código   
        
Para añadir comentarios en Bash Script se debe utilizar el signo numeral **#** seguido del
comentario que se desea agregar.
        
```bash
# Esto es un comentario en Bash Script

```

Si se requiere añadir más comentarios, se puede insertar el comentario dentro de comillas
simples **'**, antecedido por el signo **:**

```bash

: '
Estas son múltiples
lineas de comentarios
en un script de Bash
'

echo "Hola Mundo"

```
Al ejecutar el script anterior solo se obtendrá la salida "Hola Mundo".



