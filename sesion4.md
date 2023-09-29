<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->


# Actividad 4: Ejercicios de control de flujo con expresiones compuestas
``````java
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
``````
### Con la información anterior, implementa los siguientes ejercicios:

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
  ____
  ____
  # Solución
  
/
package com.mycompany.act4;

/**
 *
 * @author Julio Cesar Torres
  
 ```java

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
