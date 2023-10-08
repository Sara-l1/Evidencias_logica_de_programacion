<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->

# Actividad 3: Ejercicios de operaciones básicas en Java.
- Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

- Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

- Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

- Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

- Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

- Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

- Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

- Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.

# DESAROLLO
- **Suma y multiplicación:**

```java
package com.mycompany.sumaymultiplicacion;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class SumayMultiplicacion {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner (System.in);
        
        System.out.println("Ingrese el primer numero: ");
        int num1 = entradaDatos.nextInt();
        
        System.out.println("Ingrese el segundo numero: ");
        int num2 = entradaDatos.nextInt();
        
        int suma = (num1 + num2);
        int multiplicacion = (num1 * num2);
        
        System.out.println(" La suma es: " + suma);
        System.out.println(" La multiplicacion es : " + multiplicacion);
        
    }
}

```
- **Resta y división:**

```java
package com.mycompany.restaydivision;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class RestayDivision {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);
       
        System.out.println("Ingresa su primer numero: ");
        int num1 = entradaDatos.nextInt();
        
        System.out.println("Ingresa su segundo numero: ");
        int num2 = entradaDatos.nextInt();
        
        int resta = (num1 - num2);
        int division = (num1 / num2);
        
        
        System.out.println("La resta es: " + resta);
        
        System.out.println("La division es: " + division);
     
        
    }
}
```

- **Operaciones combinadas**

```java 
package com.mycompany.operacionescombinadas;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class OperacionesCombinadas {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);

        System.out.println("Ingrese el primer numero: ");
        int num1 = entradaDatos.nextInt();

        System.out.println("Ingrese el segundo numero: ");
        int num2 = entradaDatos.nextInt();

        System.out.println("Ingrese el tercer numero: ");
        int num3 = entradaDatos.nextInt();
        
        int suma = (num1 + num2 + num3);
        int combinada = (num1 * num2 / num3);
        
        System.out.println("La suma es: " + suma);
        System.out.println("El resultado de la multiplicacion y division es: " + combinada);
        
        System.out.println("El resultado de la suma es " + " " + suma + " " + "Resultado operacion combinada es " + combinada);
       
    }
}
```

- **Operaciones con decimales**

```java
package com.mycompany.operacionesdecimales;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class OperacionesDecimales {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);
        double num1;
        double num2;
     
        System.out.println("Ingresa tu primer numero decimal: ");
        num1 = entradaDatos.nextDouble(); 
        System.out.println("Ingresa tu segundo numero decimal: ");
        num2 = entradaDatos.nextDouble();
        
        
        System.out.println("La suma de estos numeros es: " + (num1 + num2));
        System.out.println("La resta de estos numeros es: " + (num1 - num2));
        System.out.println("La multiplicacion de estos numeros es: " + (num1 * num2));
        System.out.println("La division de estos numeros es: " + ((double)num1 / (double)num2));
        
        
    }
}
```
- **Incremento y decremento:**

```java
package com.mycompany.incrementodescremento;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class IncrementoDescremento {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);

        System.out.println("Ingrese el numero: ");
        int num1 = entradaDatos.nextInt();

        System.out.println("El incremento del numero es: " + ++num1);

        System.out.println("El decremento del numero es: " + num1--);

    }
}
```
- **Operador ternario:**

```java
package com.mycompany.operadorternanrio;

import java.util.Scanner;

/**
 *
 * @author SaraLopera
 */
public class OperadorTernanrio {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner (System.in);
        
        System.out.println("Ingresa un numero: ");
        int numero = entradaDatos.nextInt();
        System.out.println((numero >= 0) ? "El numero es positivo" + numero: numero + "El numero es negativo");
    }
}
```
