# drf-vue
Este repositorio está basado en un tutorial de [@marcelorobin](https://github.com/marcelorobin). Link al repositorio del proyecto original: [drf-vue](https://github.com/marcelorobin/drf-vue)

Para empezar el proyecto debemos tener instalado Python en nuestro sistema.

Link a la web de descargas de Python: https://www.python.org/downloads/

Es una buena práctica crear un entorno virtual para instalar ahí, de forma aíslada nuestros paquetes de Python.
Para ello podemos emplear el siguiente comando:

**Windows:**
```
python -m venv <nombre_del_entorno_virtual>
```
Una vez hayamos creado el entorno virtual y lo veamos en nuestro directorio podemos acceder a él con el siguiente comando:

```
.\venv\Scripts\activate
```
Ahora en nuestra consola veremos que nos aparece algo así como (venv) C:\ ...
Seguidamente vamos a instalar los paquetes de Python necesarios, estos van a ser Django y Django Rest Framework

**Instalar Django:**
```
pip install Django
```

**Instalar Django Rest Framework:**
```
pip install djangorestfrawork
pip install markdown
pip install django-filter
```

**Creo que lo siguiente son los django-admin startproject y tal volver a ver el video**

**Importar decorators para el filtrado de datos** http://127.0.0.1:8000/api/products/by_category/?category=3