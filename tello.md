### Controlando drones con python

Ejemplo: si queremos instalar un módulo python para controlar los drones de DJI Tello Edu, basta con que [busquemos en la página pypi.org "dji tello edu"](https://pypi.org/search/?q=dji+tello+edu&o=)

Mirando el detalle del primer resultado DJITelloPy

![pip DJITelloPy](./images/pip_DJITelloPy.png)

Vemos:

* Actualizado a python >=3.6
* Última versión del 27 de enero de 2021
* El repositorio de github tiene 370 estrellas
* Y se han realizado 163 fork ([proyectos derivados])

Además vemos que tiene un excelente [página de documentación](https://djitellopy.readthedocs.io/en/latest/) y [ejemplos](https://github.com/damiafuentes/DJITelloPy/tree/master/examples/) en la misma página de pip

```python
from djitellopy import Tello

tello = Tello()

tello.connect()
tello.takeoff()

tello.move_left(100)
tello.rotate_counter_clockwise(90)
tello.move_forward(100)

tello.land()
```

Si lo instalamos en nuestro pc con linux 
```sh
pip3 install djitellopy2
```

![InstalacionDJITelloPip.png](./images/InstalacionDJITelloPip.png)


Si ahora lo instalamos en una Raspberry

![InstalacionDJITelloPipRaspi](./images/InstalacionDJITelloPipRaspi.png)

Vemos que instala los mismos paquetes pero usa versiones diferentes