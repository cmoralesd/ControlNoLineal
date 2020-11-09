# ControlNoLineal
Control de un sistema Brazo-Hélice mediante métodos discretos <br>
En esta serie de actividades utilizaremos modelos discretos mediante ecuaciones de diferencias lineales para controlar un sistema no lineal compuesto por un brazo móvil impulsado por una hélice.<br>
El detalle de las actividades se encuentra en la serie de videos del canal de Youtube Robótica con Python, en la serie "Control de sistemas no lineales": https://www.youtube.com/playlist?list=PLOxPNrO-_c2i4ByVJ-0y5mXAbx1ZlGqvo<br>
<br>

<n>Instrucciones para instalar el servidor web en localhost cuando hay conflicto de versiones con Python</n><br>
El script server.py crea un servidor local que se comunica con la interfaz de Arduino mediante puerto serial. La comunicación se realiza mediante un socket que se crea localmente en el mismo computador.<br>
Para funcionar requiere de varias librerías adicionales:<br>
- flask<br>
- flask-socketio<br>
- pyserial<br>
- eventlet<br>
Este script fue creado para Python en versión 3.4 y se ha observado que hay algunas incompatibilidades con el paquete eventlet en las versiones de Python superiores a 3.6.<br>
Si observa errores en la instalación o, aún cuando la instalación termina sin errores, el servidor local no se levanta correctamente (esto es, no es posible enlazar a la dirección localhost:3000), entonces proceda de la siguiente manera:<br>
1. Desinstale su versión actual de Anaconda Python desde el Panel de Control → Desinstalar Programas. Tras la desinstalación, revise su carpeta de usuario y verifique que se ha eliminado la carpeta Anaconda3, si sigue allí, elimínela manualmente.<br>
2. Instale la versión de Anaconda Python 4.2.0, la cual incluye la versión de Python 3 que funciona correctamente con el script. Los enlaces de descarga directa son:<br>
Para Windows de 32 bits: Anaconda3-4.2.0-Windows-x86.exe<br>
Para Windows de 64 bits: Anaconda3-4.2.0-Windows-x86_64.exe<br>
Utilice todas las opciones por defecto para la instalación.<br>
3. Desde la consola de Anaconda (Anaconda Promt) y NO la consola de Windows (CMD), ejecute los siguientes comandos para instalar las librerías requeridas:<br>
> pip install flask<br>
> pip install flask-socketio<br>
> pip install pyserial<br>
> pip install eventlet<br>
4. Siga a continuación las siguientes instrucciones tal como están descritas en el video de configuración de software y ajustes, a excepción que los comandos deben ejecutarse desde la consola de Anaconda (Anaconda Promt), y no desde la consola de Windows (CMD).<br>
