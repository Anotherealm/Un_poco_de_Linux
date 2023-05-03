# System Logs
## Registros de sistema
---
Los registros de sistema son una serie de archivos que contienen información relacionada con 
eventos y errores que ocurren en el sistema operativo.

\_Importancia de los registros de sistema\_

- Permiten monitorear y solucionar problemas del sistema.
- Proporcionan información acerca del comportamineto del sistema, la actividad de las 
aplicaciones y eventos de seguridad.
- El análisis de registros permite identificar potenciales riesgos de seguridad y responder 
ante eventos de manera rápida.

Linux posee diferentes tipos de registros de sistema, incluyendo:

### Kernel Logs
Son registros sobre la actividad del **Kernel** del sistema operativo. 

- Se almacenan en el archivo **kern.log**, alojado en la ruta */var/log/kern.log*
- Errores de hardware y del sistema de archivos.
- Actividad de la red, como conexiones entrantes y salientes, y errores de red.
- Procesos del sistema operativo
- Información sobre los controladores de hardware, las "llamadas al sistema" (system 
calls) y los eventos del Kernel

Además del archivo "kern-log", puede leerse y analizar los kernel logs por medio del comando 
"**dmesg**". Este comando permite analizar o controlar el "**kernel ring buffer**", una 
estructura de datos circular que almacena los mensajes del kernel.

- System Logs
- Authentication Logs
- Application Logs
- security Logs
