<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->

# Estructuras de control en Java
Las estructuras de control en Java son construcciones del lenguaje que permiten controlar el flujo de ejecución de un programa. Los principales tipos de estructuras de control en Java son:

- **Estructuras de selección:** permiten elegir entre varias opciones. Incluyen la sentencia if, la sentencia switch.

- **Estructuras repetitivas:** permiten repetir un bloque de código mientras se cumpla una condición. Incluyen los bucles for, while, do-- while.

- **Estructuras de salto:** permiten cambiar el flujo de ejecución, saltando parte del código. Incluyen las sentencias break, continue, return.

## Estructuras condicionales:
Las estructuras condicionales en Java permiten tomar decisiones y ejecutar ciertas partes de código dependiendo si se cumple o no una determinada condición.

Las principales estructuras condicionales son:

**1. if: Ejecuta un bloque de código si se cumple la condición.**
Sintaxis:
```java
if (condición) {
  // código a ejecutar 
}
```
**2. if - else: Ejecuta un bloque si se cumple la condición, y otro bloque distinto si no se cumple.**
Sintaxis:
```java
if (condición) {
  // código si se cumple
} else {
  // código si no se cumple
}
```
**3. if - else if - else: Permite evaluar múltiples condiciones. Se ejecuta el primer bloque donde se cumpla la condición.**
Sintaxis:
```java
if (condición 1) {
  // código si se cumple 1
} else if (condición 2) {
  // código si se cumple 2 
} else {
  // código si no se cumple ninguna
}
```
**4. Operador ternario**
El operador ternario en Java es una expresión que se utiliza para evaluar una condición y devolver uno de dos valores, dependiendo del resultado de la evaluación. La sintaxis del operador ternario es:

Sintaxis:
``` java
variable = (condicion) ? valor_si_verdadero : valor_si_falso;
```
**5. switch: Evalúa una variable o expresión y ejecuta el código del case que coincida con el valor.**
Sintaxis:
```java
switch(expresión) {
  case valor1: 
    //código
    break;
  case valor2: 
   //código
   break;
  default:
   //código por defecto  
}
```
Estas estructuras permiten controlar el flujo del programa ejecutando código de manera condicional. Son muy útiles para realizar selecciones y tomar decisiones en la lógica de un programa.

## **Ejemplos if:**
Estos ejemplos muestran diferentes formas de utilizar estructuras condicionales en Java para tomar decisiones basadas en ciertas condiciones.

**1. Comprobando si una variable es mayor que otra:**
```java
int x = 10;
int y = 5;

if (x > y) {
  System.out.println("x es mayor que y");
}
```
**2. Comprobando si una variable es diferente de un valor específico:**
```java
int edad = 18;

if (edad != 18) {
  System.out.println("La edad no es 18");
}
```
**3. Comprobando si una variable está dentro de un rango de valores:**
```java
int nota = 10;

if (nota >= 9 && nota <= 10) {
  System.out.println("La nota es excelente");
}
```
## **Ejemplos if else:**

**1. Comprobando si una variable es mayor que otra y, si no, imprimiendo un mensaje diferente:**
```java
int x = 10;
int y = 5;

if (x > y) {
  System.out.println("x es mayor que y");
} else {
  System.out.println("x es menor o igual que y");
}
```
**2. Comprobando si una variable es igual a un valor específico y, si no, imprimiendo un mensaje diferente:**
```java
String nombre = "Juan";

if (nombre.equals("Juan")) {
  System.out.println("El nombre es Juan");
} else {
  System.out.println("El nombre no es Juan");
}
```
**3. Comprobando si una variable está dentro de un rango de valores y, si no, imprimiendo un mensaje diferente:**
```java
int nota = 10;

if (nota >= 9 && nota <= 10) {
  System.out.println("La nota es excelente");
} else {
  System.out.println("La nota no es excelente");
}
```
## **Ejemplos else if:**

**1. Comprobando si una variable es mayor que otra, si no, si es igual y, si no, imprimiendo un mensaje diferente:**
```java
int x = 10;
int y = 5;

if (x > y) {
  System.out.println("x es mayor que y");
} else if (x == y) {
  System.out.println("x es igual a y");
} else {
  System.out.println("x es menor que y");
}
```
**2. Comprobando si una variable está dentro de un rango de valores, si no, si es mayor o si es menor y, si no, imprimiendo un mensaje diferente:**
```java
int nota = 10;

if (nota >= 9 && nota <= 10) {
  System.out.println("La nota es excelente");
} else if (nota > 10) {
  System.out.println("La nota es sobresaliente");
} else if (nota < 0) {
  System.out.println("La nota es inválida");
} else {
  System.out.println("La nota es buena");
}
```
**3. Comprobando si una variable está vacía o no, si no, si tiene una longitud específica y, si no, imprimiendo un mensaje diferente:**
```java
String cadena = "";

if (cadena.isEmpty()) {
  System.out.println("La cadena está vacía");
} else if (cadena.length() == 0) {
  System.out.println("La cadena es nula");
} else {
  System.out.println("La cadena no está vacía");
}
```
## **Ejemplos operador ternario:**
**1. Devuelve el valor máximo de dos números**
```java
int max = (a > b) ? a : b;
// Devuelve el texto "El número es positivo" si el número es mayor que 0,
// y el texto "El número es negativo" si el número es menor o igual a 0.
String texto = (numero > 0) ? "El número es positivo" : "El número es negativo";
```
**2. Devuelve el valor máximo de tres números**
```java
int max = (a > b) ? (a > c ? a : c) : (b > c ? b : c);

// Devuelve el texto "El número es positivo" si el número es mayor que 0,
// el texto "El número es cero" si el número es igual a 0,
// y el texto "El número es negativo" si el número es menor que 0.
String texto = (numero > 0) ? "El número es positivo" : (numero == 0 ? "El número es cero" : "El número es negativo");
```
**3. Devuelve el texto "El número es par" si el número es par, y el texto "El número es impar" si el número es impar.**
```java
String texto = (numero % 2 == 0) ? "El número es par" : "El número es impar";
```
## **Otros ejemplos**
**1. Comprobación del número par o impar:**
```java
int numero = 7;

if (numero % 2 == 0) {
    System.out.println("El número es par.");
} else {
    System.out.println("El número es impar.");
}
```
**2. Evaluación de la calificación de un estudiante:**
```java
int calificacion = 85;

if (calificacion >= 90) {
    System.out.println("Excelente");
} else if (calificacion >= 80) {
    System.out.println("Bueno");
} else if (calificacion >= 70) {
    System.out.println("Regular");
} else {
    System.out.println("Reprobado");
}
```
**3. Verificación de la elegibilidad para votar:**
```java
int edad = 17;

if (edad >= 18) {
    System.out.println("Eres elegible para votar.");
} else {
    System.out.println("No eres elegible para votar.");
}
```
**4. Determinar si un número es positivo, negativo o cero:**
```java
int numero = -3;

if (numero > 0) {
    System.out.println("El número es positivo.");
} else if (numero < 0) {
    System.out.println("El número es negativo.");
} else {
    System.out.println("El número es cero.");
}
```
**5. Validación de una contraseña:**
```java
String contraseña = "secreta123";

if (contraseña.equals("secreta123")) {
    System.out.println("Contraseña correcta. Acceso concedido.");
} else {
    System.out.println("Contraseña incorrecta. Acceso denegado.");
}
```
## **Ejemplos switch:**
**1. Escribe un programa que le pida al usuario que ingrese un día de la semana. El programa debe imprimir el número del día de la semana.**
```java
import java.util.Scanner;

public class DiaSemana {

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.println("Ingrese un día de la semana: ");
    String dia = sc.nextLine();

    switch (dia) {
      case "lunes":
        System.out.println("1");
        break;
      case "martes":
        System.out.println("2");
        break;
      case "miércoles":
        System.out.println("3");
        break;
      case "jueves":
        System.out.println("4");
        break;
      case "viernes":
        System.out.println("5");
        break;
      case "sábado":
        System.out.println("6");
        break;
      case "domingo":
        System.out.println("7");
        break;
      default:
        System.out.println("Día no válido");
    }
  }
}
```
**2. Escribe un programa que le pida al usuario que ingrese una calificación de 1 a 10. El programa debe imprimir la calificación en letras.**
```java
import java.util.Scanner;

public class Calificacion {

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.println("Ingrese una calificación de 1 a 10: ");
    int calificacion = sc.nextInt();

    switch (calificacion) {
      case 1:
        System.out.println("Insuficiente");
        break;
      case 2:
        System.out.println("Insuficiente");
        break;
      case 3:
        System.out.println("Insuficiente");
        break;
      case 4:
        System.out.println("Suficiente");
        break;
      case 5:
        System.out.println("Bien");
        break;
      case 6:
        System.out.println("Notable");
        break;
      case 7:
        System.out.println("Sobresaliente");
        break;
      case 8:
        System.out.println("Sobresaliente");
        break;
      case 9:
        System.out.println("Sobresaliente");
        break;
      case 10:
        System.out.println("Excelente");
        break;
      default:
        System.out.println("Calificación no válida");
    }
  }
}
```
**3. Escribe un programa que le pida al usuario que ingrese un número entero. El programa debe imprimir la estación del año correspondiente al número.**
```java
import java.util.Scanner;

public class Estacion {

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.println("Ingrese un número entero: ");
    int numero = sc.nextInt();

    switch (numero) {
      case 1:
      case 2:
      case 3:
        System.out.println("Invierno");
        break;
      case 4:
      case 5:
      case 6:
        System.out.println("Primavera");
        break;
      case 7:
      case 8:
      case 9:
        System.out.println("Verano");
        break;
      case 10:
      case 11:
      case 12:
        System.out.println("Otoño");
        break;
      default:
        System.out.println("Número no válido");
    }
  }
}
```
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