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

Para crear un Bash Script primero debemos crear un archivo con formato *.sh*. Para esto, 
puede ocuparse el editor de texto que se desee.

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


### Condicionales

Las condicionales son estructuras de control que permiten que nuestro 
script tome diferentes caminos o acciones en base a una evaluación lógica.

La sintaxis básica de una condicional es la siguiente:

```bash
if [ condición-a-evaluar ]; 
then
  # Acciones a realizar si la condición es verdadera
fi
```
- **if** se utiliza para indicar el inicio de la condicional.
- Entre los corchetes es señalada la condición a evaluar.
- **then** es utilizado para iniciar el bloque de código a ejecutar, 
solo si la condición *if* es **verdadera**.
- **fi** indica el final de la estructura de control.
 
Puede indicarse otra condición, la cuál se ejecutará sólo si la
condición *if* resulte falsa. Para esto, se utiliza la palabra **else**

```bash
if [ condición ]; then
  # Acciones a realizar si la condición es verdadera
else
  # Acciones a realizar si la condición if es falsa
fi
```

Además, se puede utilizar varias condiciones, utilizando la 
palabra **elif**

```bash
if [ condición 1 ]; then
  # Acciones a realizar si la condición 1 es verdadera
elif [ condición 2 ]; then
  # Acciones a realizar si la condición 2 es verdadera
else
  # Acciones a realizar si todas las condiciones son falsas
fi
```

Es necesario aclarar que el script solo ejecutará la primera 
condición que resulte verdadera. Si todas las condiciones resultan
falsas, entonces sólo será ejecutado el bloque de código "else"
