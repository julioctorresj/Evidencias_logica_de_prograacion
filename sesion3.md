<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->



# Actividad 3: Ejercicios de operaciones básicas en Java. 

1. Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

2. Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

3. Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

4. Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

5. Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

6. Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

7. Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

8. Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.
   ________________
   ________________

   # Solución
# 1.

``````java

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Project/Maven2/JavaApp/src/main/java/${packagePath}/${mainClassName}.java to edit this template
 */

package com.mycompany.act1;
import java.util.Scanner;
/**
 *
 * @author Julio Cesar Torres
 */
public class Act1 {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);
        
        System.out.println("Ingrese el primer numero");
        int numero1 = entradaDatos.nextInt();
        
          System.out.println("Ingrese el segundo numero");
        int numero2 = entradaDatos.nextInt();
        
        int suma = numero1 + numero2;
        int multi = numero1 * numero2;
        
           System.out.println("El resultado de la suma es: "+ suma);
           System.out.println("El resultado de la multiplicacion es: "+ multi);
    }
}
``````
## Act 2


<!-- Su documentación aquí -->

```java
package com.mycompany.act2;

import java.util.Scanner;

/**
 *
 * @author Julio Cesar Torres
 */
public class Act2 {

    public static void main(String[] args) {
         Scanner entradaDatos = new Scanner(System.in);
        
        System.out.println("Ingrese el primer numero");
        int numero1 = entradaDatos.nextInt();
        
          System.out.println("Ingrese el segundo numero");
        int numero2 = entradaDatos.nextInt();
        
        int resta = numero1 - numero2;
        int divis = numero1 / numero2;
         
           System.out.println("El resultado de la resta es: " + resta);
           System.out.println("El resultado de la division es: "+ divis);
    }
}

```
## Act 3

```java
package com.mycompany.act3;

import java.util.Scanner;

/**
 *
 * @author Julio Cesar TORRES
 */
public class Act3 {

    public static void main(String[] args) {
             Scanner entradaDatos = new Scanner(System.in);
        
        System.out.println("Ingrese el primer numero");
        int numero1 = entradaDatos.nextInt();
        
          System.out.println("Ingrese el segundo numero");
        int numero2 = entradaDatos.nextInt();
        
          System.out.println("Ingrese el tercer numero");
        int numero3 = entradaDatos.nextInt();
        
        int suma = numero1 + numero2 + numero3;
        int resultado = (numero1 * numero2)/ numero3;
        
           System.out.println("El resultado de la suma de los 3 numeros es: " + suma);
           System.out.println("El resultado de la operacion es: "+ resultado);
    }
}
```
## Act 4

```java
package com.mycompany.act4;

/**
 *
 * @author ALEJANDRA ARIAS
 */
public class Act4 {

    public static void main(String[] args) {
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

        //Determinar si el estudiante es mayor de edad y tiene un estado activo.
        System.out.println("Determinar si el estudiante es mayor de edad y tiene un estado activo. ");
        if (edad >= 18 && esActivo) {
            System.out.println("el estudiante es mayor de edad y esta activo");
        } else {
            System.out.println("el estudiante es menor de edad o no esta activo");
        }
        System.out.println("-------------------------------------------------------");
        System.out.println("Determinar si el estudiante tiene una beca o una carrera relacionada con el desarrollo de software");

        if (becado == true || carrera.equals("Desarrollo de Software")) {
            System.out.println("el estudiante tiene una beca o estudia dsarrollo de software");
        } else {
            System.out.println("el estudiante no es becado y no estudia desarrollo de software");
        }
        System.out.println("-------------------------------------------------------");
        System.out.println("determinar si e estudiante esta en el ultimo semestre de su carrera y tiene un esado activo");

        if (semestre == 3 && esActivo) {
            System.out.println("el estudiante esta en el ultimo semestre y esta activo");
        } else {
            System.out.println("el estudiante no esta en ultimo semestre o no esta activo");
        }
        System.out.println("-------------------------------------------------------");
        System.out.println("determinar si e estudiante tiene una carrera relacionada con el desarrollo de software y un promedio superior a 4");

        if (carrera.equals("Desarrollo de Software") && promedio > 4.0) {
            System.out.println("esta en desarrollo de software y un promedio mayor a 4");
        } else {
            System.out.println("el estudiante no esta en desarrollo de software o no tiene promedio mayor a 4");
        }
        System.out.println("-------------------------------------------------------");
        System.out.println("Mostrar toda la información del estudiante si está matriculado en el Cesde.");
        
        if(universidad.equals("Cesde")){
            System.out.println("Nombre: "+ nombre);
            System.out.println("Apellido: "+ apellido);
            System.out.println("Identificacion: "+ identificación);
            System.out.println("Edad: "+ edad);
            System.out.println("Genero: "+ género);
            System.out.println("Coreo: "+ correo);
            System.out.println("Carrera: "+ carrera);
            System.out.println("Universidad: "+ universidad);
            System.out.println("Activo: "+ esActivo);
            System.out.println("Becado: "+ becado);
            System.out.println("Promedio: "+ promedio);
            System.out.println("Semestre: "+ semestre); 
        }
        else{
            System.out.println("el estudiante no esta matriculado en cesde");
        }
        System.out.println("-------------------------------------------------------");
        System.out.println("Asignar una beca del 50% si el estudiante está matriculado en el Cesde, tiene un promedio superior a 4.0 y está activo.");
        
        if(universidad.equals("Cesde")&& promedio > 4.0 && esActivo){
            System.out.println("asignar beca");
        }
        else{
            System.out.println("no asignar beca");
        }
        System.out.println("-------------------------------------------------------");
        System.out.println("Determinar la cantidad de beca que recibe el estudiante según su promedio.");
        
        if(promedio >= 0.0 && promedio <= 3.4){
            System.out.println("El estudiante no recibe beca");
        }
        else if (promedio >=3.5 && promedio <=3.9){
            System.out.println("el estudiante recibe 25% de beca");
        }
            else if(promedio >=4.0 && promedio <=4.4){
                    System.out.println("el estudiante recibe 50% de beca");
                    }
            else if (promedio >=4.5 && promedio <=5.0 ){
                System.out.println("el estudiante recibe 100% de beca");
        }
            else{
                System.out.println("Nota no valida");
            }
    }
}
```
## Act 5

```java
package com.mycompany.act5;

import java.util.Scanner;

/**
 *
 * @author ALEJANDRA ARIAS
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
## Act 6
```java
package com.mycompany.acti6;

/**
 *
 * @author Julio Cesar Torres
 */
public class Acti6 {

    public static void main(String[] args) {
    int numero1 = 10;
    
    numero1 += 5;
        System.out.println("El valor es " + numero1);
        
    }
}

```
## Act 7
```java
public class Acti7 {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);
        //boolean resultado;
        
        System.out.println("ingrese num 1: true o false ");
        boolean num1 = entradaDatos.nextBoolean();
        
          System.out.println("ingrese num 2: true o false ");
        boolean num2 = entradaDatos.nextBoolean();
        
        boolean resultado = num1 && num2;
        
         System.out.println("El resultado de la and es: " + resultado);
         
         resultado = num1 || num2;
           System.out.println("El resultado de la or es: " + resultado);
           
            resultado = !num1 ;
             System.out.println("El resultado de not num 1 es: " + resultado);
             
             resultado = !num2 ;
             System.out.println("El resultado de not num 2 es: " + resultado);
    }
  
}

```
## Act 8
```java
public class Act8 {

    public static void main(String[] args) {
       Scanner entradaDatos = new Scanner(System.in);
       
        System.out.println("Ingrese un numero");
        int num1 = entradaDatos.nextInt();
        System.out.println((num1 >= 0) ? "El numero es positivo " + num1 : "El numero es negativo " + num1);
    }
}

```