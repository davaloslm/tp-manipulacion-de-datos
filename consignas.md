# Consignas
---

## Micro desafío - Paso 1:

Para la construcción de esta versión del sitio web, el cliente espera contar con la posibilidad de acceso a las siguientes URLs:

 - /movies/add (GET)
    - Muestra el formulario para la creación de una película.

 - /movies/create (POST)
    - Recibe los datos del formulario anterior y escribe la información en la base de datos.
    - El controlador deberá utilizar la conexión a la base de datos y el modelo de Película ya creado. Luego, el método create permitirá la creación del registro. Finalmente, el controlador debe redirigir al listado de películas.

---

## Micro desafío - Paso 2:

Actualizar una película indicada en la URL según el ID:

 - /movies/edit/:id (GET)
    - Muestra un formulario ya completo con los datos de la película según el id que indica la URL.
    - Previamente debe agregarse en el detalle de la película un botón de editar que envíe a esta URL. El controlador recupera el id de la URL mediante req.params.
 - /movies/update/:id (POST) --- Idealmente PUT
    - Recibe información del formulario mencionado anteriormente y en conjunto con el id que indica la URL actualiza la información de la película.
    - Recibe información del formulario mencionado anteriormente recuperable mediante req.body. El controlador deberá utilizar la conexión a la base de datos y el modelo de Película ya creado. Mediante el método update se modifica la información de la base de datos. Luego, el controlador debe redirigir al listado de películas.

---

## Micro desafío - Paso 3:

Elimina la película indicada en la URL según el ID:

 - /movies/delete/:id (POST) --- Idealmente DELETE
    - Previamente debe agregarse en el detalle de la película un botón de borrado que envíe a esta URL. El controlador recupera el id de la URL mediante req.params. El controlador deberá utilizar la conexión a la base de datos y el modelo de Película ya creado. Mediante el método destroy se elimina el registro y luego se redirige al listado de películas.
    - Probemos de eliminar varias películas, ¿funciona siempre bien?