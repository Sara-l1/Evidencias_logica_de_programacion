<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 


<!-- Su documentación aquí -->

# Actividad: Ejecicios de métodos en Java
Implementar los siguientes métodos:

1. Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.
2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.
3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.
4. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.
5. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las palabras en orden alfabético.

# DESARROLLO

## 1. Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.

```java 
@author SaraLopera
 */
public class MayorDeDosNumeros {

    public static void main(String[] args) {
      int num1 = 35;
        int num2 = 45;
        int mayor = mayorNumero(num1, num2);
        System.out.println("El número mayor es: " + mayor);
    }

    public static int mayorNumero(int num1, int num2) {
        if (num1 > num2) {
            return num1;
        } else {
            return num2;
        }
    }
}

```

## 2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.

```java
 @author SaraLopera
 */
public class Vocales {

    public static void main(String[] args) {
      String texto = "Hola, Buenas tardes, espero estes muy bien";
        int cantidadVocales = contarVocales(texto);
        System.out.println("El total de vocales es: " + cantidadVocales);
    }

    public static int contarVocales(String texto) {
        int contadorVocales = 0;

        texto = texto.toLowerCase();

        for (int i = 0; i < texto.length(); i++) {
            char caracter = texto.charAt(i);
            if (caracter == 'a' || caracter == 'e' || caracter == 'i' || caracter == 'o' || caracter == 'u') {
                contadorVocales++;
            }
        }

        return contadorVocales;
    }
}
```

## 3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.

```java
 * @author SaraLopera
 */
public class MayusculasYMinusculas {

    public static void main(String[] args) {
        String texto = "BUENAS TARDES,MI NOMBRE ES sara";
        String resultado = cambiarMayusculasMinisculas(texto);
        System.out.println("Texto modificado: " + resultado);
    }

    public static String cambiarMayusculasMinisculas(String texto) {
        char[] caracteres = texto.toCharArray();

        for (int i = 0; i < caracteres.length; i++) {
            char caracter = caracteres[i];
            if (Character.isUpperCase(caracter)) {
                caracteres[i] = Character.toLowerCase(caracter);
            } else if (Character.isLowerCase(caracter)) {
                caracteres[i] = Character.toUpperCase(caracter);
            }
        }
```

## 4. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.

```java
 * @author SaraLopera
 */
public class Plabras {

    public static void main(String[] args) {
        String texto = "Buenos dias, como estan todos?";

        int cantidadPalabras = contarPalabras(texto);
        System.out.println("La cantidad de palabras en el texto es: " + cantidadPalabras);
    }

    public static int contarPalabras(String texto) {
        String[] palabras = texto.split("\\s+"); 
        return palabras.length;
    }
}
```

## 5. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las palabras en orden alfabético.

```java
 * @author SaraLopera
 */
public class OrdenDePalabras {

    public static void main(String[] args) {
               String texto = "Funcionando esta cadena de texto en varias palabras.";
        String resultado = ordenarPalabras(texto);
        System.out.println("Palabras ordenadas: " + resultado);
    }

    public static String ordenarPalabras(String texto) {
        
        String[] palabras = texto.split("\\s+");

       
        Arrays.sort(palabras);

        String resultado = String.join(" ", palabras);

        return resultado;
    }
}
```