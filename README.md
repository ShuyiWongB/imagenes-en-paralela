# Imagenes en Paralela

Trabajo de imagenes en computacion paralela

### Lenguaje y Librerias necesarias

#### Lenguaje

* C++

#### Librerias

* Openmpi

```
sudo apt-get install openmpi-bin openmpi-common openssh-client openssh-server libopenmpi1.3 libopenmpi-dbg libopenmpi-dev
```

* Opencv

```
sudo apt-get install libopencv-dev
```

* Phthreats

### ANTES de activar el programa

* Agregar las ip de las maquinas a utilizar en el archivo ```maquinas.txt```
* Definir dentro del codigo la ruta en la que se guardaran las imagenes ya editadas en PathDest

### Pasos para activar el programa

* Ejecutar el archivo Makefile con los comandos ```make clean && make```

#### Difuminado Gaussiano

* Para ejecutar esta funcion debe realizar el siguiente llamado
```
mpirun --hostfile maquinas.txt ./dist/programa 1 <ruta de su imagen original>
```

#### Escala de Grises

* Para ejecutar esta funcion debe realizar el siguiente llamado
```
mpirun --hostfile maquinas.txt ./dist/programa 2 <ruta de su imagen original>
```

#### Escala la imagen sin perder la calidad

* Para ejecutar esta funcion debe realizar el siguiente llamado
```
mpirun --hostfile maquinas.txt ./dist/programa 3 <ruta de su imagen original>
```

### Autores
* Sion-jei Mamani
* Janira Navarro
* Shu-yi Wong
