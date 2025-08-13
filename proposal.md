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
![DER](https://github.com/user-attachments/assets/53f54897-8e3a-4ae3-8666-8d7306e2159b)



## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Perosna<br>2. CRUD Servicio<br>3. CRUD Marca<br>4. CRUD Categoria|
|CRUD dependiente|1. CRUD Producto {depende de} CRUD Marca<br>2. CRUD Formula {depende de} CRUD Tono y CRUD Producto|
|Listado<br>+<br>detalle| 1. Listado de productos filtrado por marca y categoría, muestra id y descripcion => detalle CRUD Producto<br>2. Listado de servicios filtrado por rango de precio, muestra nombre, descipcion y precio=> detalle muestra datos completos de los servicios correspondientes al rango de precio con su precio.|
|CUU/Epic|1. registrar atencion de clientes (registrar productos usados en la atencion y especificaciones) <br>2. solicitar turno|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Persona<br>2. CRUD Servicio<br>3. CRUD Marca<br>4. CRUD Tono<br>5. CRUD Categoria<br>6. CRUD Descuento<br>7. CRUD Producto<br>8. CRUD Atencion<br>9. CRUD Turno<br>10. CRUD Formula|
|CUU/Epic|1. Registrar atencion de clientes<br>2. Mostrar listado de atenciones realizadas al cliente<br>3. Desbloquear y mostrar un descuento<br>4. Resgitrar turno|


### Alcance Adicional Voluntario

|Req|Detalle|
|:-|:-|
|Listados |1. Atenciones filtradas por estado<br>2. Turnos filtrados por clientes que requieren color|
|CUU/Epic|1. seleccionar aplicar descuento en el proximo servicio <br>2. notificar descuento al cliente|
|Otros|1. envío de preparación previa a los clientes que realizan su primera visita y requieren color|