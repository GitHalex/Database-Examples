# Universe

## list of entities

### galaxy

- name VARCHAR(30)
- id_galaxy **(PK)** SERIAL
- cantidad_planet INT
- id_star **(FG)** REFERENCES start

### star

- name VARCHAR(30)
- id_star **(PK)** SERIAL
- composicion VARCHAR(20)
- id_planet **(FG)** REFERENCES id_planet

### planet

- name VARCHAR(30)
- id_planet **(PK)** SERIAL
- Masa INT
- Diametro ecuatorial NUMERIC 11.2
- Tiene_Luna BOOLEAN
- id_moon **(FG)** REFERENCES mooon

### mooon **(EC)**

- name VARCHAR(30)
- id_moon **(PK)** SERIAL
- cantidad_moon INT
- Type

## Relaciones

1, una **carrera** _pertenece_ aun **tipode carrera** (_1 a 1_)

## Diagramas

### modelo entidad - relacion

![Modelo Entidad - Relacion] (./universeModeloe-R.png)

### Modelo Relacional de la BD

## Reglas de Negocio

### carreras

1. Crear el registro de una carrera
2. Leer el registro de una(s) carrera(s) dada una condicion en particular
3. Leer todos los registros de la entidad carreras.
4. Actualizar los datos de una carrera dada una condicion en particular
5. Eliminar los datos de una carrera dada una condicion en particular

### tipos_carreras **(EC)**

1. Crear el registro de un tipo de carrera
2. Leer el registro de uno(s) tipos de carrera(s) dada una condicion en particular
3. Leer todos los registros de la entidad tipos carreras.
4. Actualizar los datos de un tipo de carrera dada una condicion en particular
5. Eliminar los datos de una carrera dada una condicion en particular

### paises **(EC)**

1. Crear el registro de un pais
2. Leer el registro de un(os) paise(s) dada una condicion en particular
3. Leer todos los registros de la entidad paises.
4. Actualizar los datos de una pais dada una condicion en particular
5. Eliminar los datos de una pais dada una condicion en particular
