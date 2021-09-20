# TikTokBots
Aquí hay una guía en español para descargar TikTokBots sin errores.

## Instalacion de python
Este programa esta creado con python para descargarlo es tan facil como meterse en su
página oficial y descargarlo aqui habra un link que sera una descarga directa: https://www.python.org/ftp/python/3.9.7/python-3.9.7-amd64.exe
Este enlace te descargara python.

**Es importante aclarar que en la instalacion tienen que seleccionar "añadir pip al path" si no lo hicieron ahora veran como añadirlo**

## Añadir el comando PIP al path
primero es comprobar si no lo tiene configuraro para verlo abre la **cmd** con Wind+R y escriba *"cmd"*
En la **cmd** escriba el siguiente comando:

```
pip --version
```

Si al ponerlo te sale algo como esto:

```
C:\Users\UserName>pip --version
pip 21.2.4 from c:\users\UserName\appdata\local\programs\python\python39\lib\site-packages\pip (python 3.9)

C:\Users\UserName>
```

Significa que esta añadido y puedes ir Directamente a los siguientes pasos

si sale lo siguiente:

```
 C:\Users\UserName>pip --version
"pip" no se reconoce como un comando interno o externo,
programa o archivo por lotes ejecutable.

C:\Users\UserName>
```

Siga los siguientes pasos.

**1.** Encontrar la carpeta de PIP.
       para encontrar la carpeta no es muy difícil,
       en la lupa de windows ***Que Se encuentra en la barra de tareas*** solo tienes que escribir lo siguiente "` pip `"
       y te deberia salir un programa llamado **pip** con el icono
       de *python*. Si es así dale al boton que pone: *Abrir ubicación del archivo*

**2.** Añadir la carpeta al path.
Actualmente deberias tener el explorador de windows con una carpeta en el que hay varios archivos,
y uno de ellos deberia ser *pip.exe* si es asi haz lo siguiente.
Copia la ruta de la carpeta **Si no sabes copiar la ruta te doy un enlace que te enseña a copiarla**

https://www.pchardwarepro.com/como-copiar-la-ruta-de-un-archivo-o-una-carpeta-en-windows-10-8-7/

Ya copiada te diriges a la lupa de windows ***Que Se encuentra en la barra de tareas*** y escribes lo siguiente "`Variables de entorno`"
y te deberia salir algo como *Editar variables de Entorno*, dale click.

Al hacerlo deberia salirte una ventana, Solo tienes que darle a "***Variables de entorno...***"
Al darle se te abrira otra ventana, ahí estan las variables como 'comúnes' y las 'propias' en este caso
cambiaremos las comúnes asi que en el cuadrado de abajo 
buscaremos la variable ***path*** aunque puede estar en mayusculas o minusculas pero tiene que salir ese texto

Si la encontrais la clickeais 1 vez solo esto es **Para seleccionarla**
y le dais al botón que pone ***Editar...***

Se abrira otra ventana vosotros le dais al botón que pone ***Nuevo*** y poneis la ruta de la carpeta

Luego le dais a todas las pestañas ***Aceptar*** y estaria añadido al path.

En la **cmd** escriba el siguiente comando:
```
pip --version
```

Y Deberia salir ahora si esto:

```
C:\Users\UserName>pip --version
pip 21.2.4 from c:\users\UserName\appdata\local\programs\python\python39\lib\site-packages\pip (python 3.9)

C:\Users\UserName>
```

## Instalacion de librerias
Este paso es muy cortito y facíl.
en el **cmd** tendrás que poner lo siguiente: 
```python
pip install pyautogui
```

Esto lo que hara sera añadir al ordenador la libreria necesaria para que funcione el programa.
Yo en este caso ya lo tengo instalado pero en consola os debería salir algo como una barra de carga asgo así:

**██████░░░░** 20mB / 100mB
