<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


<!-- Su documentación aquí -->

# Actividad 5: Ejercicios de bucles

 Resolver los siguientes ejercicios:

# Ejercicios - while

1. Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.
   
2. Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.
   
# Ejercicios - do while

1. Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.
   
2. Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.
   
# Ejercicios - for

1. Imprimir los números impares del 1 al 50.
   
2. Imprimir los números primos del 1 al 100.
   
# Solución
_______________

```java

package com.mycompany.act5;

import java.util.Scanner;

/**
 *
 * @author Julio Cesar Torres
 */
public class ACT5 {

    public static void main(String[] args) {

        Scanner entradaDatos = new Scanner(System.in);
        // Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.

        System.out.println("ingrese un numero");
        int numero = entradaDatos.nextInt();
        int i = 0;

        while (i <= 10) {
            int resultado = i * numero;
            System.out.println(i + " * " + numero + " : " + resultado);
            i++;
        }
        System.out.println("-----------------------------------------------------------------");
        // Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

        Scanner sc = new Scanner(System.in);
        System.out.print("Ingrese una cadena de caracteres: ");
        String cadena = sc.nextLine();

        i = 0;
        int contadorNumeros = 0;
        while (i < cadena.length()) {
            char caracter = cadena.charAt(i);
            if (caracter == '0' || caracter == '1' || caracter == '2' || caracter == '3' || caracter == '4'
                    || caracter == '5' || caracter == '6' || caracter == '7' || caracter == '8' || caracter == '9') {
                contadorNumeros++;
            }
            i++;
        }

        System.out.println("La cadena ingresada contiene " + contadorNumeros + "Numeros.");

        System.out.println("-----------------------------------------------------------------");
        //Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.

        Scanner entrada1 = new Scanner(System.in);
        System.out.println("si quiere detener el programa dijite un numero negativo");
        numero = entrada1.nextInt();

        i = 1;
        if (numero >= 0) {
            do {
                System.out.println(i);
                i++;

            } while (i <= 100);
        }
        System.out.println("-----------------------------------------------------------------");
        // Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

        Scanner entrada2 = new Scanner(System.in);
        System.out.println("digite un numero entero para imprimir la tabla de multiplicar o 0 para detener");
        numero = entrada2.nextInt();

        i = 0;
        if (numero > 0) {
            do {
                int resultado = i * numero;
                System.out.println(i + " * " + numero + " : " + resultado);
                i++;

            } while (i <= 10);
        }
        System.out.println("-----------------------------------------------------------------");
        // Imprimir los números impares del 1 al 50.

        for (i = 1; i < 50; i += 2) {
            System.out.println(i);
        }
        System.out.println("-----------------------------------------------------------------");
        //Imprimir los números primos del 1 al 100.

        for (int x = 1; x <= 100; x++) {
            int divisores = 0;
            for (int j = 1; j <= x / 2; j++) {
                if (x % j == 0) {
                    divisores += 2;
                }
            }
            if (divisores == 2) {
                System.out.println(x + " es un numero primo");
            }
        }
    }
}

```