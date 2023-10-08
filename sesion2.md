<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 2


<!-- Su documentación aquí -->

# Actividad 2: Instalación de Entornos de Desarrollo para Java y ejercicios de programación básica.

### Instalación de Entornos de Desarrollo para Java
**Objetivo:**
Familiarizarse con la instalación de los entornos de desarrollo necesarios para programar en Java.

El proceso de instalación de los entornos de desarrollo para Java, NetBeans IDE e IntelliJ IDEA, se puede resumir en los siguientes pasos:

- Descargar NetBeans IDE desde el sitio web oficial de NetBeans.
- Ejecutar el archivo de instalación de NetBeans y seguir las instrucciones del asistente de instalación.
- Descargar IntelliJ IDEA desde el sitio web oficial de IntelliJ IDEA.
- Ejecutar el archivo de instalación de IntelliJ IDEA y seguir las instrucciones del asistente de instalación.
- Verificar la instalación abriendo cada IDE y creando un proyecto de Java.
- Explorar las características y funcionalidades de cada entorno de desarrollo.

**Prueba y ejecución de ejercicios de programación básica.**
En esta actividad, pondremos en práctica los conceptos aprendidos de programación básica mediante la ejecución y prueba de diversos ejercicios. Utilizaremos el lenguaje de programación Java para implementar los programas y comprobaremos su funcionamiento ingresando diferentes valores de entrada.

## DESARROLLO

### **1. Programa para calcular la hipotenusa de un triángulo rectángulo:**

```java
package com.mycompany.hipotenusa;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class Hipotenusa {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        
        try (Scanner scanner = new Scanner(System.in)){

        System.out.print("Ingrese el valor del primer cateto: ");
        double cateto1 = scanner.nextDouble();

        System.out.print("ingrese el alor del segundo cateto: ");
        double cateto2 = scanner.nextDouble();

        double hipotenusa = Math.sqrt(Math.pow(cateto1, 2) + Math.pow(cateto2, 2));
        System.out.println("La hipotenusa del triangulo es: " + hipotenusa);
        }
    }
}
```

### **2. Programa para determinar si un número es par o impar:**

```java
package com.mycompany.numeroparimpar;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */

public class NumeroParImpar {

    public static void main(String[] args) {
       try (Scanner scanner = new Scanner(System.in)){
           System.out.print("Ingrese el numero: ");
           int numero = scanner.nextInt();
           
           if (numero % 2 == 0){
               System.out.println("El numero es par.");
              } else {
           
               System.out.println("El numero es impar.");
         } 
    }
}
}
```
### **3. Programa para calcular el tercer ángulo de un triángulo:**

```java
package com.mycompany.rangulodetriangulo;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class App {

    public static void main(String[] args) {
        try(Scanner scanner = new Scanner(System.in)){
         System.out.print("Ingrese el valor del primer angulo: ");
         int angulo1 = scanner.nextInt();
        
         System.out.print("Ingrese el valor del segundo angulo: ");
         int angulo2 = scanner.nextInt();
         
         if (angulo1 > 0 && angulo1 < 180 && angulo2 > 0 && angulo2 < 180){
             int TercerAngulo = 180 - (angulo1 + angulo2);
             System.out.println("El valor del tercer angulo es: " + TercerAngulo);
         } else {
             System.out.println("Los valores ingresados no son angulos vlidos");
         }}
    }
}
```

### **4. Programa para calcular el promedio de tres números:**

```java
package com.mycompany.promediotresnumeros;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class PromedioTresNumeros {

    public static void main(String[] args) {
    
try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese el primer número: ");
            double numero1 = scanner.nextDouble();
            
            System.out.print("Ingrese el segundo número: ");
            double numero2 = scanner.nextDouble();
            
            System.out.print("Ingrese el tercer número: ");
            double numero3 = scanner.nextDouble();
            
            double promedio = (numero1 + numero2 + numero3) / 3;
            System.out.println("El promedio de los tres números es: " + promedio);
        }
    }
}
```

### **5. Programa para calcular la longitud de una cadena de texto:**

```java
package com.mycompany.longitudcadena;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class LongitudCadena {

    public static void main(String[] args) {
        try(Scanner scanner = new Scanner(System.in)){
            System.out.print("Ingrese una cadena de texto: ");
            String texto = scanner.nextLine();
            
            int longitud = texto.length();
            System.out.println("La longitud de la cadena es: " + longitud);
        }
    }
    }     
```

### **6. Programa para calcular el área de un triángulo:**

```java
package com.mycompany.areadetriangulo;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class AreadeTriangulo {

    public static void main(String[] args) {
        try(Scanner scnner =new Scanner(System.in)){
         System.out.print("Ingrese la base del triangulo: ");
         double base = scnner.nextDouble();
         
         System.out.print("Ingrese la altura del triangulo: ");
         double altura = scnner.nextDouble();
         
         double area = (base * altura) / 2;
         System.out.println("El area del triangulo es:" + area); 
        }    
    }
}
```

### **Programa para calcular la raíz cuadrada de un número:**

```java
package com.mycompany.raizcuadradan;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class RaizCuadradaN {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese un número: ");
            double numero = scanner.nextDouble();
            
            double raizCuadrada = Math.sqrt(numero);
            System.out.println("La raíz cuadrada del número es: " + raizCuadrada);
        }
    }
}
```

### **8. Programa para calcular el máximo común divisor (MCD) de dos números:**

```java
package com.mycompany.mcd;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class MCD {

    public static void main(String[] args) {
      try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese el primer número: ");
            int numero1 = scanner.nextInt();
            
            System.out.print("Ingrese el segundo número: ");
            int numero2 = scanner.nextInt(); 
            
            int res = mcd(numero1, numero2);
            
            System.out.println("MCD:" + res);
        }
    }

    private static int calcularMCD(int numero1, int numero2) {
        
        int a = Math.max(numero1, numero2);
        int b = Math.min(numero1, numero2);
        
        int resultado = 0;
        do (
            resultado = b;
        b = a % b;
        a = resultado;
       
        )while(b!=0);
        
       return resultado;
    }
}
```

### **9. Programa para imprimir una cadena de texto en orden inverso:**

```java
package com.mycompany.cadenatextoinversa;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class CadenaTextoInversa {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese una cadena de texto: ");
        String texto = scanner.nextLine();

        String textoInverso = "";
        for (int i = texto.length() - 1; i >= 0; i--) {
            textoInverso += texto.charAt(i);
        }

        System.out.println("La cadena en orden inverso es: " + textoInverso);

        scanner.close();
    }
}
```

### ** 10. Programa para calcular el área de un rectángulo:**

```java
package com.mycompany.arearectangulo;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class AreaRectangulo {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese la base del rectángulo: ");
            double base = scanner.nextDouble();
            
            System.out.print("Ingrese la altura del rectángulo: ");
            double altura = scanner.nextDouble();
            
            double area = base * altura;
            System.out.println("El área del rectángulo es: " + area);
        }
    }
}
```
