<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


<!-- Su documentación aquí -->

# Actividad 5: Ejercicios de bucles
Resolver los siguientes ejercicios:

**Ejercicios - while**
1. Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.
2. Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

**Ejercicios - do while**
1. Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.
2. Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

**Ejercicios - for**
1. Imprimir los números impares del 1 al 50.
2. Imprimir los números primos del 1 al 100.


# DESARROLLO

## **while**
1. Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.

```java
package com.mycompany.actividad5;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class Ejec1 {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);
        System.out.println("Ingresa un numero: ");
        int numero = entradaDatos.nextInt();
        
        int i = 1;
        while (i <= 10){
       
            System.out.println(numero * i);
            i++;
        }
    }}
```

## **while**
2. Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

```java 
package com.mycompany.caracteresn;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class CaracteresN {

    public static void main(String[] args) {
         Scanner dts = new Scanner(System.in);
        System.out.print("Ingrese una cadena de caracteres: ");
        String cadena = dts.nextLine();

        int i = 0;
        int contadorNumeros = 0;

        while (i < cadena.length()) {
           char caracteres = cadena.charAt(i);
            if (Character.isDigit(cadena.charAt(i))) {
             contadorNumeros++;
             caracteres+=cadena.charAt(i);
            }
            i++;
        }
        System.out.println("La cadena ingresada contiene " + contadorNumeros + "numeros: ");
    }
}
```
## **do while**
1.  Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.

```java
package com.mycompany.dowhile1;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class DoWhile1 {

    public static void main(String[] args) {
        Scanner dts = new Scanner(System.in);

        int numero = 1;

        System.out.println("Ingresa un numero: ");
         int num= dts.nextInt();
         
        do {
            System.out.println(numero);
            numero++;

         } while ( numero <= 100 && num >=0);

        // si ingresa un numero negativo se detendrá 

    }
}
```
## **do while**
2. Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

```java
package com.mycompany.dowhile2;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class DoWhile2 {

    public static void main(String[] args) {
         Scanner entradaDatos = new Scanner(System.in);
        System.out.println("Ingresa un numero");
        int num = entradaDatos.nextInt();
        
        int multiplicacion = 1;
        
        do {            
             System.out.println(num + "*" + multiplicacion + "=" + num * multiplicacion);
            multiplicacion ++;  
        } while (num != 0 && multiplicacion <=10);
   
        } 
            
        }
```
## **for**

1. Imprimir los números impares del 1 al 50.

```java
package com.mycompany.for1;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class For1 {

    public static void main(String[] args) {
        Scanner dts = new Scanner(System.in);   
        for (int i=1; i<=50; i+= 2) {
            
            System.out.println(i);
        }
    }
}
```
## **for**

2. Imprimir los números primos del 1 al 100.

```java
package for2;

/**
 *
 * @author Sara Lopera
 */
public class For2 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        Scanner dtos new  = Scanner(System.in);
        for (int i = 1; i <= 100; i++) {
            int x = 1;
            int contar = 0;
            while (x <= 1) {
                if (1 % x == 0) {
                    contar++;
                }
                x++;
            }
            if (contar == 2) {
                System.out.println(1 + "Es primo");
            }
        }
    }
}
```