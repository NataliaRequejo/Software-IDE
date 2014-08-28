Scripts que descargan y preparan los componentes del instalador
===============================================================

Prerequisitos
-------------
 Windows 7 con powershell instalado o wget.exe en el mismo directorio de "prepare.bat"

Ejecute prepare.bat y espere a que termine.
Esto crear� las carpetas
 * local-repo Repo local donde se encuentran los paquetes requeridos para instalar cygwin
 * cygwin Directorio de instalaci�n de cygwin (debe habilitar la linea "rem cyg-install.bat" en el archivo prepare.bat)
 * eclipse-cdt conteniendo el JRE
 * arm-none-eabi-gcc desde launchpad
 * PHP compilado para cygwin

TODO
----
 - Bajar desde la pagina de freddy chopins (mantenedor del paquete compilado para win32)
 - O bajar el c�digo fuente y compilar a mano usando cygwin (recordar limpiar el entorno para posterior uso de NSIS)
 - Realizar un *.ini con los par�metros de eclipse correspondientes
 - Realizar un bat para ejecutar eclipse desde un acceso directo en el escritorio y/o en el men� inicio. Este debe realizar
    > Modificaci�n de PATH a�adiendo cygwin y arm-none-eabi como
    > workspace por defecto, perspectiva a usar -cdt-, etc.)
 - Realizar el script de NSIS (determinar layout para la instalaci�n)
 - Realizar *.ini de instalaci�n del driver
 - Realizar testcases de las herramientas luego de instalar
