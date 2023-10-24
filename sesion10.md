<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


<!-- Su documentación aquí -->

# Actividad: Prueba, ejecución y explicación de ejercicios de lógica de programación.
- Selecciona dos ejercicios de la sesión 10, impleméntalos, ejecútalos y proporciona una explicación detallada de cada uno

### 1. Cálculo del índice de masa corporal (IMC) 

```java
* @author SaraLopera
 */
public class Ejercicio10IMC {

   public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
      double weight, height, imc;
      
      // Solicita el peso y la altura
      System.out.print("Ingrese su peso en kilogramos: ");
      weight = input.nextDouble();
      System.out.print("Ingrese su altura en metros: ");
      height = input.nextDouble();

      // Calcula el IMC
      imc = weight / (height * height);

      // Muestra el resultado en la consola
      System.out.printf("Su IMC es %.2f", imc);
      
   }
}
```
## Explicación: 
El IMC utilizando la fórmula IMC = weight / (height * height). Recibe el weight y la height como argumentos y devuelve el IMC calculado.
Mostramos un mensaje inicial y solicitamos al usuario que ingrese su peso en kilogramos, y despues que ingrese su altura en metros,llamamos a la función 'calcularIMC' para calcular el IMC y guardamos el resultado en la variable 'imc', finalmente, se muestra el resultado en la consola con dos decimales utilizando el método printf de la clase System.out.




### 2. Calcular el movimiento rectilíneo uniforme

```java
 * @author SaraLopera
 */
public class Ejercicio10Rectilineo {

    public static void main(String[] args) {
     Scanner input = new Scanner(System.in);
      double velocidad, tiempo, distancia;
      
      // Solicita la velocidad y el tiempo
      System.out.print("Ingrese la velocidad en metros por segundo: ");
      velocidad = input.nextDouble();
      System.out.print("Ingrese el tiempo en segundos: ");
      tiempo = input.nextDouble();

      // Calcula la distancia recorrida
      distancia = velocidad * tiempo;

      // Muestra el resultado en la consola
      System.out.printf("La distancia recorrida es de %.2f metros.", distancia);
   }
}
```

## Explicación: 
El movimiento rectilíneo uniforme se calcula con la formmula de *distancia = velocidad x tiempo.* Entonces empezamos con un scanner input y unas variables tipo double que se llamaran: Velocidad, tiempo y distancia. Luego se le pedira al usuario que ingrese la velocidad en metros por segundo y se almacenara en velocidad, al momento que ingrese el tiempo en segundos se almacenara en tiempo. Esto realizara la operacion en donde la variable distancia, almacenara el resultado: Velocidad * tiempo, y luego un System.out.printf, regresara el resultado con una cadena de texto que es “La distancia recorrida es de %.2f metros.”, distancia”.