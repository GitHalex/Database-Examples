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

### mooon

- name VARCHAR(30)
- id_moon **(PK)** SERIAL
- cantidad_moon INT
- Type

### cometa

- hoa
