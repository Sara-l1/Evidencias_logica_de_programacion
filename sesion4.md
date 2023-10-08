<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->

# Actividad 4: Ejercicios de control de flujo con expresiones compuestas
```java
// Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;
```
**Con la información anterior, implementa los siguientes ejercicios:**

1. Determinar si el estudiante es mayor de edad y tiene un estado activo.
2. Determinar si el estudiante tiene una beca o una carrera relacionada con el desarrollo de software.
3. Determinar si el estudiante está en el último semestre de su carrera y tiene un estado activo.
4. Determinar si el estudiante tiene una carrera relacionada con el desarrollo de software y un promedio superior a 4.0.
5. Mostrar toda la información del estudiante si está matriculado en el Cesde.
6. Asignar una beca del 50% si el estudiante está matriculado en el Cesde, tiene un promedio superior a 4.0 y está activo.
7. Determinar la cantidad de beca que recibe el estudiante según su promedio:
- 0.0 - 3.4: El estudiante no recibe beca.
- 3.5 - 3.9: El estudiante recibe una beca parcial del 25%.
- 4.0 - 4.4: El estudiante recibe una beca parcial del 50%.
- 4.5 - 5.0: El estudiante recibe una beca completa.

# DESARROLLO:

```java
package com.mycompany.expresionescompuestas;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class ExpresionesCompuestas {

    public static void main(String[] args) {

    

        String nombre = "Juan Pérez";
        String apellido = "González";
        String identificación = "1000000001";
        String correo = "juan.perez@ejemplo.com";
        String carrera = "Desarrollo de Software";
        String universidad = "Cesde";
        String Deporte = "basquetbol";

// Variable de tipo int
        int edad = 20;
        
// Variable de tipo boolean
        boolean esActivo = true;
        boolean becado = false;
// Variable de tipo char
        char género = 'M';
// Variable de tipo double
        double promedio = 4.5;
// Variable de tipo int
        int semestre = 2;

        if (edad >= 18) {
            System.out.println("Es mayor de edad !! ");
        } else {
            System.out.println("Es menor de edad !! ");
        }

        if (esActivo || becado && esActivo) {
            System.out.println("Esta activo ");
        } else {
            System.out.println("No esta activo ");
        }

        if (carrera.equals("Desarrollo de Software ") || becado) {
        } else {
            System.out.println("La carrera del estudiante es:  " + carrera);
        }

        if (semestre == 2 && esActivo) {
            System.out.println("El estudiante esta en el 2do semestre y tiene su estado activo ");
        } else {
            System.out.println("El estudiante no esta en el ultimo semestre y no esta activo: ");
        }
        
        if (carrera.equals("Desarrllo de Software") && promedio >= 4.5){
           System.out.println("El estudiante esta en la carrera de Dearrollo de Software con un promedio superior ");
        } else {
            System.out.println("El promedio del estudiante esta por debajo de 4.5 ");
        } 
        
        System.out.println("Estudiante matriculado en el CESDE " + nombre + " " + apellido + " " + "Con numero de documento" + " " + identificación + " " + "Género " + género);
        System.out.println("Correo electronico:" + " " + correo + " " + "Carrera:" + " " + carrera + " " + "Actualmente estudiando en la universidad " + universidad);
        
        if (universidad.equals("Cesde") && promedio >= 4.0 && esActivo){
           System.out.println("El estudiante tiene una beca del 50% por su buen promedio"); 
        } else{
            System.out.println("No es apto para la beca, no se encuentra activo");
        }
        
        if (promedio >= 0.0 && promedio <= 3.9){
            System.out.println("Estudiante no puede acceder a la beca ");
        } else {
        if (promedio >= 3.5 && promedio <= 3.9){
            System.out.println("Estudiate recibe beca parcial del 25% ");
        } else {
        if (promedio >= 4.0 && promedio <= 4.4){
            System.out.println("Estudiante recibe beca parcial del 50% "); 
        } else{
        if (promedio >= 4.5 && promedio <= 5.0){
            System.out.println("Estudiante recibe beca completa ");
        }    
        
        System.out.println("El estudiante practica como deporte: " + " " + Deporte);
        }
        }
        }
    }
}
```