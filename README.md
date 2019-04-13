# Proyecto-html-y-css

Esta página consistirá en una biografía y filmografía del director, productor y actor Quentin Tarantino, así como las diversas curiosidades y anécdotas sobre su carrera.

### Link a la página

[<img src="https://i.imgur.com/UzSGgtN.png">](http://tarantino.ddns.net)

### 									>>> [Capturas de la página](https://mega.nz/#F!7E9VDCpa!i5QSPFBQmvsR4mgIaXLrSA)

### Página de descarga de la plantilla


[<img src="https://s.tmimgcdn.com/wp-content/uploads/2016/05/logo_tm_new.svg">](https://www.templatemonster.com/)

# Hosting
Podría haber utilizado una página de hosting gratuito como *000webhost*, pero en lugar de eso he utilizado una raspberry pi zero. Al ser una página bastante ligera y tener un tráfico casi nulo no he necesitado usar un modelo con prestaciones superiores.
Esta raspberry lleva instalado *raspbian lite strech* junto con el paquete *apache2*.

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






