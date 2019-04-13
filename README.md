# Proyecto-html-y-css

Esta página consistirá en una biografía y filmografía del director, productor y actor Quentin Tarantino, así como las diversas curiosidades y anécdotas sobre su carrera.

[Link a la página!](http://tarantino.ddns.net)

### Página de descarga de la plantilla

[TemplateMonster](https://www.templatemonster.com/)

# Hosting
Podría haber utilizado una página de hosting gratuito como 000webhost, pero en lugar de eso he utilizado una raspberry pi zero. Al ser una página bastante ligera y tener un tráfico casi nulo no he necesitado usar un modelo con prestaciones superiores.
Esta raspberry lleva instalado *raspbian lite strech* junto con el paquete *apache2*.

## ¿Cómo he hecho accesible esta raspberry?

Para conseguir que fuese accesible, he tenido que seguir una serie de pasos.
- Asignarle una **ip estática** dentro de mi red privada
- Establecer una **DNAT** en mi router, asociando el **puerto 80** y la ip estática
- Registrarme en la página *NO-IP* para conseguir un **dns dinámico**
- Asociar el **dns dinámico** a mi **ip pública**
- Configurar en mi router el dns dinámico
- Descargar el *paquete ofrecido por NO-IP* en la raspberry *para que el dns* sea realmente dinámico y si cambia mi ip pública, *se actualice automáticamente*.


