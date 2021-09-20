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
Yo en este caso ya lo tengo instalado pero en consola os debería salir algo como una barra de carga algo así:

**██████░░░░** 20mB / 100mB

Al terminar la instalacion toca el paso más complicado.

## Ajustes de pantalla
Aqui voy a poner el codigo del programa para ver algunas cosas que hay que alterar:

```python
import pyautogui as p
import time

#----------------------------------------------------------------
# Created by: Alextellar (Alextellar#3622 in discord)
# Pag web require = zeftoy.com
#

x, y = p.position()
print(x, ",", y)

loc = (176 , 567)
col = (230, 189, 190)
searchBtn = (618 , 521)
midBtn = (438 , 574)

while True:
    a = p.screenshot()
    if a.getpixel(loc) != col:
        print("yes!")
        p.moveTo(searchBtn[0], searchBtn[1])
        time.sleep(0.1)
        p.click()
        time.sleep(2.5)
        p.moveTo(midBtn[0], midBtn[1])
        time.sleep(0.1)
        p.click()
        time.sleep(3)

    else:
        print("No :(")
    time.sleep(1)
```

En el codigo deberían ver algo que pone:
```python
loc = (176 , 567)
col = (230, 189, 190)
searchBtn = (618 , 521)
midBtn = (438 , 574)
```
Aqui se declaran las variables, y voy a explicar para que es cada una

```python
loc = (176 , 567) # Esta es la posicion del checker, es decir que cuando algo cambie en esa posicion se activa el programa 
col = (230, 189, 190) # Este es solo el color, no hay que cambiar nada
searchBtn = (618 , 521) # este es el botón de buscar o como pone en la página web "search"
midBtn = (438 , 574) # y por ultimo este es el botón que esta en el medio en el que sale El num de likes, segs, compartidas, vistas, ...
```
Ya sabiendo para que es cada variable toca cambiarlas.
primero la que pone ***loc***
como saben al iniciar *Zefoy* **https://zefoy.com/**
sale un contador en el que pone lo siguiente: ***Please wait 0 minute(s) 22 seconds for your next submit!***

Pues nos centraremos en la ***P*** de ***Please*** ahí estara nuestro checker.
Basicamente las cordenadas de la variable ***loc*** estaran situadas **JUSTO** en la ***P***.

Al saber eso veremos como ver las cordenadas de la pantalla.

#### Codenadas de pantalla
