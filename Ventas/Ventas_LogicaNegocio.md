# Ventas

## Listado de entidades

### Clientes **(ED)**

- cliente_id **(PK)**
- nombre
- apellidos
- telefono
- email
- direccion
- cp
- ciudad
- pais **(FK)**

### productos **(ED)**

- producto_id **(PK)**
- nombre
- descripcion
- foto
- precio
- cantidad

### ventas

- venta_id **(PK)**
- cliente_id **(FK)**
- fecha
- monto

### articulos_x_venta **(EP)**

- articulo_id **(PK)**
- venta_id **(FK)**
- producto_id **(FK)**

### pais **EC**

- pais_id
- nombre
- dominio
