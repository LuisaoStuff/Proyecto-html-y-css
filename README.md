[<img src="https://i.imgur.com/UzSGgtN.png">](http://tarantino.ddns.net)

Esta página consistirá en una biografía y filmografía del director, productor y actor Quentin Tarantino, así como las diversas curiosidades y anécdotas sobre su carrera. La plantilla utilizada ha sido descargada de la página [***Template Monster***](https://www.templatemonster.com/). Las capturas de pantalla de los diferentes html y sus respectivas validaciones, podrás encontrarlas [**aquí**](https://mega.nz/#F!7E9VDCpa!i5QSPFBQmvsR4mgIaXLrSA).

# Hosting
Podría haber utilizado una página de hosting gratuito como *000webhost*, pero en lugar de eso he utilizado una raspberry pi zero. Al ser una página bastante ligera y tener un tráfico casi nulo no he necesitado usar un modelo con prestaciones superiores. Esta raspberry lleva instalado *raspbian lite strech* junto con el paquete *apache2*.

## Desarrollo y publicación de la página
Tanto para desarrollar como para publicar la página he usado la *raspberry*, solo que mientras la desarrollaba, no estaba pública y para acceder a ella usaba la ip privada de mi red. En las dos fases he usado github, clonando el repositorio en la máquina de desarrollo con ssh, es decir usando `git clone git@github.com***` y en la *raspberry* clonándolo con https, es decir, usando `git clone https://github.com/LuisaoStuff/Proyecto-html-y-css.git` y actualizándola con `git pull`.
Una vez terminado el proceso de desarrollo, **publico** la página dándole un **dns dinámico** a la raspberry.

## ¿Cómo he hecho accesible esta raspberry?

Para conseguir que fuese accesible, he tenido que seguir una serie de pasos.
##### 1. Asignarle una **ip estática** por **dhcp** dentro de mi red privada.
![Imgur](https://i.imgur.com/5sfrQey.png)
##### 2. Configurar el **Port Forwarding** abriendo el **puerto 80** para la ip de mi raspberry.
![Imgur](https://i.imgur.com/o4iNXyY.png)
##### 3. Registrarme en la página *NO-IP* para conseguir un **dns dinámico**.
##### 4. Asociar el **dns dinámico** a mi **ip pública**.
![Imgur](https://i.imgur.com/5oZWBnc.png)
##### 5. Activar en mi router el *dns dinámico* y vincular mi cuenta.
![Imgur](https://i.imgur.com/S44R2s6.png)
##### 6. Descargar el **paquete ofrecido por NO-IP** en la raspberry **para que el dns** sea realmente dinámico y si cambia mi ip pública, **se actualice automáticamente**.





