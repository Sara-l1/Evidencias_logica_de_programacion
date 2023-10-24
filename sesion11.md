<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 11 


<!-- Su documentación aquí -->

# Actividad: Ejercicios de Lógica de Programación

1. Basándose en el algoritmo 1 de la sesión 11, aplicar la siguiente variante: Dado un conjunto de números enteros, se debe determinar si existe algún número que aparezca más de una vez. Si es así, se deben imprimir todos los números que aparezcan más de una vez.

2. Desarrollar un algoritmo que realice la conversión de binario a decimal.

# DESARROLLO

### 1. Basándose en el algoritmo 1 de la sesión 11, aplicar la siguiente variante: Dado un conjunto de números enteros, se debe determinar si existe algún número que aparezca más de una vez. Si es así, se deben imprimir todos los números que aparezcan más de una vez.

```java
 * @author SaraLopera
 */
public class NumerosRepetidos {


    public static void main(String[] args)throws InterruptedException {
        
    Integer [] numeros = new Integer [] {1, 2, 3, 9, 2, 7, 8, 8, 3, 3, 10, 11, 3, 1, 3, 3, 9, 10};
    String repetidos = "";
    boolean imprimeComa = false; 

    System.out.println("Elementos duplicados en numeros: "); 

    for (int i = 0; i < numeros.length; i++) {  
       for (int j = i + 1; j < numeros.length; j++) {
         
          if (
               numeros[i].equals(numeros[j]) 
               && 
               !repetidos.contains("" + numeros[i].toString() + "") 
          ) {

             if (!imprimeComa){
                imprimeComa = true;
             } else {
                repetidos += ", "; 
             }

             // Imprime los elementos duplicados
             repetidos += "" + numeros[j] + "";
          }
       }
    }

    System.out.print(repetidos.replace("*", ""));
    }
}
```

### 2. Desarrollar un algoritmo que realice la conversión de binario a decimal.

```java
 @author SaraLopera
 */
public class AlgoritmoBinarioDecimal {

   
      public static void main(String[] args) {
     long numero, aux, digito, decimal;
     int exponente;
     boolean esBinario;
     Scanner Datos = new Scanner(System.in);

     do {
          System.out.print("Introduce un numero binario: ");
          numero = Datos.nextLong();
          
          esBinario = true;
          aux = numero;
          while (aux != 0) {
                     digito = aux % 10; 
                     if (digito != 0 && digito != 1) { 
                          esBinario = false; 
                     }
                     aux = aux / 10;                        
           }
      } while (!esBinario); //

      //proceso para pasar de binario a decimal
      exponente = 0;
      decimal = 0; //será el equivalente en base decimal
      while (numero != 0) {
                //se toma la última cifra
                digito = numero % 10;
                //se multiplica por la potencia de 2 correspondiente y se suma al número                          
                decimal = decimal + digito * (int) Math.pow(2, exponente);
                //se aumenta el exponente
                exponente++;
                //se quita la última cifra para repetir el proceso
                numero = numero / 10;
      }
      System.out.println("Decimal: " + decimal);
    }
}
```