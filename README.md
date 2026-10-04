# Actividad 5 - Structs y Punteros

## Datos del proyecto

**Materia:** Laboratorio de Programación (LPR)
**Curso:** 5° Año
**Institución:** E.E.S.T. N° 1 "Eduardo Ader"
**Integrantes:** Martina Araujo, Thiago Goya y Sofia Salaberry

## Descripción

En esta actividad se realizó un programa en C++ para trabajar con `struct` y punteros.

Se creó una estructura llamada `EntidadProyecto`, que contiene tres datos: un ID, un nombre o descripción y una métrica.

```cpp
struct EntidadProyecto {
    int id;
    char nombre[50];
    float metrica;
};
```

La estructura sirve para tener todos los datos relacionados dentro de una misma variable.

## Funcionamiento

Primero se crea una variable llamada `miEntidad` y se le dan unos valores iniciales.

Después se llama a la función `cargarDatos()`:

```cpp
cargarDatos(&miEntidad);
```

El `&` se utiliza para obtener la dirección de memoria de `miEntidad`. Esa dirección se recibe en la función mediante el puntero `ptr`.

Dentro de la función se utiliza `->` para acceder a los datos:

```cpp
ptr->id
ptr->nombre
ptr->metrica
```

De esta forma, la función puede modificar directamente los datos de `miEntidad`.

## Ejemplo

Si se ingresan:

```text
ID: 10
Nombre: Sensor de temperatura
Metrica: 25.5
```

el programa muestra esos mismos datos al finalizar.

También muestra la dirección de memoria de `miEntidad`.

## Conceptos utilizados

* `struct`: permite agrupar varios datos relacionados.
* `puntero`: guarda la dirección de memoria de una variable.
* `&`: obtiene la dirección de memoria.
* `->`: permite acceder a los datos mediante un puntero.
* `cin` y `cout`: permiten ingresar y mostrar información.

## Conclusión

Con esta actividad entendí cómo se puede usar un `struct` para organizar datos y cómo un puntero puede acceder a una estructura mediante su dirección de memoria. También pude entender la diferencia entre usar `.` para una variable normal y `->` cuando se trabaja con un puntero.

