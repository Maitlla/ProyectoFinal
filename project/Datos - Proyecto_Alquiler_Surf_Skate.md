> Integrantes del grupo: Angel, Brais, Chistian, Maite.

#
# Título

# **LuaWave**


#
# Descripción

Tienda online donde se alquilan pack para hacer surf y para practicar skate, (las tablas, neopreno para el surf, casco y otros accesorios necesarios).


#
# Mockups

        En construcción...

![Datos](./Home1.jpg)

![Datos](./Home2.jpg)

![Datos](./Home3.jpg)

![Datos](./Home4.jpg)

![Datos](./AlquilerSurf2.jpg)

![Datos](./AlquilerSurf1.jpg)

![Datos](./AlquilerSkate1.jpg)


#
# Datos

![Datos](./datos.jpg)

## Artículos

- Nombre
- Descripción
- Foto
- Stock 
- Precio del pack para alquilar con IVA incluido
- URL / Referencia - posible enlace con Amazon (si da tiempo)


## Stock

        .....(posibilidad de complicarlo más)


## Datos cliente

        Solo cuando compren pack para alquilar

- Id único
- Nombre, apellidos
- DNI / NIF
- Teléfono
- Dirección
- Código postal
- Carrito asociado a cliente, (productos comprados)


## Carrito

- Artículos (pack para alquilar)
- Cantidad
- Forma de pago
- Forma de envío
- Asociado a datos del cliente


## Staff

        .....(página externa)

- Login básico para el personal
- Jerarquia de acceso del personal (gestión de la base de datos)


#
# Endpoints

![Engranajes](./engranajes.jpg)

## Artículos

- GET

  Consultar artículos.

  - GET /articles/- Devuelve una lista de artículos
  - GET /article/10/- Devuelve un artículo específico

- POST

  Añadir artículos.

  - POST /article/- Crea un nuevo artículo

- PUT

  Hacer modificaciones de los artículos.

  - PUT /article/10/- Modifica el artículo #10

- PATCH

  Hacer modificaciones parciales o concretas de los artículos.

  (Probablemente no se utilice)

- DELETE 

  Eliminar artículos.

  - DELETE /article/10/- Elimina el artículo #10


## Carrito

- GET

  Devuelve una lista con los artículos añadidos al carrito.

    - GET /carrito/- Consultar el carrito.

- POST

  Crea un carrito inicial vacio, que se irá modificando con PUT.

  - POST /carrito/- Crear carrito vacío, que identifique al cliente. 

- PUT

  Modifica los artículos del carrito.

  PUT final: se envian los datos del cliente y del pack o packs en alquiler (artículos), cuando se pasa al pago del pack en alquiler.

  - PUT /carrito/- Actualizar el carrito.

- DELETE 

  Elimina los artículos del carrito.

  - DELETE /carrito/- Eliminar el carrito.


## Staff

        .....(página externa) planteandose

- GET
- POST
- PUT
- PATCH
- DELETE












