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
 * openOCD 0.8 desde el repositorio de freddy chopins
 * Testcase de compilacion de lina de comandos

TODO
----
 - Realizar un *.ini con los par�metros de eclipse correspondientes
 - workspace por defecto, perspectiva a usar -cdt-, etc.)
 - Realizar *.ini de instalaci�n del driver
 - Expandir testcases de las herramientas luego de instalar
