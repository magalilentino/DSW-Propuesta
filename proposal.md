# Propuesta TP DSW

## Grupo
### Integrantes
* 52234 - Corvi, Jerónimo
* 52109 - Lentino, Magali
* 52868 - Lupo, Valeria
* 53413 - Moramarco, Elias


### Repositorios
* [frontend app](https://github.com/magalilentino/DSW-Frontend)
* [backend app](https://github.com/magalilentino/DSW-Backend)


## Tema: software para peluquería
### Descripción
Sistema en el que los peluqueros registran las atenciones de cada cliente (fecha, servicio que se realizó, peluquero que lo realizó) y los clientes pueden acceder a estos y a un listado de los servicios con sus respectivos precios que se realizan en la peluquería. Además, por parte de los peluqueros, contarán con un registro de la fórmula utilizada para el color y los productos utilizados. 

### Modelo
![DER](https://github.com/user-attachments/assets/3591516c-a121-4617-a49f-e73a63e26d6d)



## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Perosna<br>2. CRUD Servicio<br>3. CRUD marca<br>4. CRUD Tono|
|CRUD dependiente|1. CRUD Producto {depende de} CRUD Marca<br>2. CRUD Precio {depende de} CRUD Servicio|
|Listado<br>+<br>detalle| 1. Listado de productos filtrado por marca y categoría, muestra id y descripcion => detalle CRUD Producto<br>2. Listado de servicios filtrado por rango de precio, muestra nombre, descipcion y precio=> detalle muestra datos completos de los servicios correspondientes al rango de precio con su precio.|
|CUU/Epic|1. registrar atencion de clientes<br>2. mostrar listado de atenciones realizadas al cliente|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Persona<br>2. CRUD Servicio<br>3. CRUD Marca<br>4. CRUD Tono<br>5. CRUD Categoria<br>6. CRUD Descuento<br>7. CRUD Producto<br>8. CRUD Atencion<br>9. CRUD Turno|
|CUU/Epic|1. Registrar atencion de clientes<br>2. Mostrar listado de atenciones realizadas al cliente<br>3. Desbloquear y mostrar un descuento<br>4. Resgitrar turno|


### Alcance Adicional Voluntario

|Req|Detalle|
|:-|:-|
|Listados |1. Clientes filtrados por turnos y deudas pendientes<br>2. Turnos filtrados por clientes que requieren color|
|CUU/Epic|1. cancelar turno<br>2. notificar descuento al cliente|
|Otros|1. envío de preparación previa a los clientes que realizan su primera visita y requieren color|

