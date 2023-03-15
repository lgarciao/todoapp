# Flask Todo App
Este es un proyecto de ejemplo en Flask que muestra cómo construir una aplicación simple de lista de tareas.

## Uso
La aplicación utiliza Flask y SQLAlchemy para manejar una base de datos SQLite y realizar operaciones CRUD en una lista de tareas. Para ejecutar la aplicación, siga estos pasos:

1. Asegúrese de tener Python 3.10.6.
2. Clone el repositorio de GitHub.
3. Navegue a la carpeta del proyecto y abra una terminal.
4. Cree un entorno virtual y active el entorno virtual.
5. Ejecute pip install -r requirements.txt para instalar las dependencias del proyecto.
6. Ejecute python app.py para iniciar la aplicación.
7. Abra un navegador web y navegue a http://localhost:5000.

## Estructura del proyecto
- *app.py*: el archivo principal que contiene la configuración de la aplicación y las rutas de Flask.
- *base.html*: la plantilla HTML base para la aplicación.
- *requirements.txt*: archivo de texto que contiene las dependencias del proyecto.

## Modelos
La aplicación utiliza un modelo *Todo* que representa una tarea en la lista de tareas. El modelo se define en el archivo *app.py* utilizando SQLAlchemy y contiene las siguientes propiedades:

* *id*: identificador único de la tarea.
* *title*: título de la tarea.
* *complete*: bandera booleana que indica si la tarea está completa o no.

## Rutas
La aplicación define las siguientes rutas de Flask:

* */*: la ruta principal que muestra la lista de tareas.
* */add*: la ruta para agregar una nueva tarea a la lista.
* */update/<int:todo_id>*: la ruta para actualizar el estado de una tarea.
* */delete/<int:todo_id>*: la ruta para eliminar una tarea de la lista.
