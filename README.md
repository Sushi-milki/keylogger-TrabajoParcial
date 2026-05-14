# keylogger-TrabajoParcial
Este repositorio contiene un keylogger desarrollado en Python como parte de mi trabajo parcial de hacking ético. El objetivo de este proyecto es aprender sobre las técnicas de interceptación de teclas en sistemas y su uso en pruebas de penetración, siempre dentro de un entorno controlado y legal.

# Funcionalidad
El keylogger está diseñado para registrar todas las teclas pulsadas por el usuario y almacenarlas en un archivo de texto. El código también incluye un sistema para enviar los datos recopilados a un servidor remoto mediante un socket, lo que permite a un atacante recibir las pulsaciones de teclas en tiempo real.

# Características:
Captura de teclas: El keylogger utiliza la librería keyboard para interceptar y registrar las teclas presionadas por el usuario.
Almacenamiento de datos: Las palabras o frases completas se guardan en un archivo de texto llamado output.txt.
Envío remoto de datos: Al presionar la tecla 'Esc', los datos se envían a un servidor remoto mediante un socket en el puerto 443.
Script autodestructivo: Una vez que los datos son enviados, el archivo de salida se elimina automáticamente.

# Código:
Se utiliza la librería keyboard para detectar las pulsaciones de teclas.
Los datos se almacenan de manera segura en un archivo.
Al finalizar el proceso, el script envía el archivo al atacante y luego termina su ejecución.

# Recomendaciones de uso:
Este proyecto solo debe ser usado con fines educativos y en entornos controlados, como parte de pruebas de penetración autorizadas o investigaciones académicas. El uso no autorizado de este tipo de herramientas es ilegal y éticamente incorrecto.

# Uso:
Ejecuta el script.
Las teclas presionadas serán registradas en el archivo output.txt.
Al presionar Esc, los datos se enviarán al servidor remoto y el script terminará su ejecución.
