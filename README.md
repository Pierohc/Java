//Los atributos deben ser privados.

//En el main se crean los objetos.

//CLASE_TIPODATO   nombre_propio = new CONSTRUCTOR

//getter <- para poder imprimir, te da el dato  

//setter <- Para asignar un valor o string


--------------
# LEER DATOS:

System.in para ingresar datos con el teclado.

scanner.nextLine() posiciona el cursos hasta que el usuario ingrese un dato y presione un enter, ese dato se guarda en una variable.

Recordar quitar el "ln" al println para que el cursor no este en la siguiente linea.

          Libreria: import java.util.Scanner;
          
          Scanner scanner = new Scanner(System.in); //creas un scanner que lo puede usar en todo el codigo
          String datoIngresado = scanner.nextLine();

Scanner todo lo guarda como String.
Si queremos ingresar un numero y luego convertirlo a entero:

                    int numero = Integer.parseInt(numeroString);

Si queremos convertir un True o False:
                    int opcion = Boolean.parse

# Problema con nextInt():
            System.out.printf("Seleccione una opción: ");
            int opcion = scanner.nextInt();
            
en este caso sabemos que lo que se va a ingresar será un número y al hacer uso del next.Int(), escribiremos el numero y daremos enter para ingresar el dato; sin embargo, cuando intentas leer una cadena con scanner.nextLine() después del nextInt(), el nextLine() consume la línea en blanco (Enter) dejada por la entrada anterior en lugar de esperar una entrada real de texto.

Para solucionar este problema, puedes agregar un scanner.nextLine() adicional justo después de leer el número para consumir el carácter de nueva línea antes de leer la cadena. . Para ello si lo siguiente que queremos hacer es ingresar de nuevo un dato, deberemos colocar un scanner.nextLine():

            System.out.println("Ingrese el nombre del producto que dese actualizar: " );
            scanner.nextLine();
            String productoActualizar = scanner.nextLine();


--------------------

# Una clase dentro de otra clase:
          

se creo un estudiante dentro de una clase de jerarquia mayor y estudiante que es una clase Estudiante, tiene como atributo computadora y la computadora es de clase Computadora, que es una clase adicional de jerarquia menor que Estudiante, la cual tiene una funcion llamada registro():


          Computadora computadora = new Computadora();
          
          public void registrarEstudiante(Estudiante estudiante){
           
          computadora.registro(); //llamo al registro de la computadora
          estudiante.setComputadora(computadora); //guardo la informacion de esa computadora en el estudiante
          System.out.println("El precio es: " + estudiante.getComputadora().getPrecio());



-----------------
CONDICIONALES:
y = &&
o = ||

Si el dato es String:

    if(opcion.equals("texto")){
    }
Si el dato es Int, para numeros:

    if(opcion == 1){
    }

Si una clase esta vacia:

    if(albergue.getGato1() == null){
    albergue.setGato1(gato);
    }


----------------------

Math.PI

-----------------

public final int num = 5 <- atributo que no se puede cambiar, valor fijo.

----------------

Si un metodo a su vez es una clase:

Agregar un valor:

    firulais.getGalleta().setIngredientePrincipan("carne");

Retornar un valor:

    firulais.getGalleta().getMarca()


----------------------------
Ternario para asignaciones:

    int total = 20
    total = num > 6 ? 40 : 10;

Reemplaza a:

    if(num>6){
     total = 40;
    }else{
      total = 10;
    }

------------------------------

# break para while si usamos switch:
  
    buclePrincipal:

    while (true){

        switch{
        
          case 1:
            break;
            
          case2:
            break;
            
          case 3:
            breack buclePrincipal; //Finaliza todo el bucle while
            
         }
     }

---------------------------------
# While:

    while(i<10){
      i++; 
      }
# For:

    for(int i=1; i <=10; i++){

    }


------------------------
# Arreglos:
Crear arreglos:

    int[] arreglo = new int[10]
    int arreglo[] = new int[10]

    int[] notas;
    notas = new int[15];

    int[] notas = {10,17,18,20,15}

Dar valores:

      notas[0] = 10;
      notas[1] = 20;...

    
Conocer tamaño del arreglo:

sout(arreglo.length);

Imprimir todos los valores:

    for(int i=0; i < arreglo.length; i++){
        sout(arreglo[i]);
     }

-------------------------------------------

# Arreglo Multidimensional (Matrices):

Longitud multidimensional constante:

![image](https://github.com/Pierohc/Java/assets/133154904/bb528412-4075-4425-bed5-f6e50dacc44b)

Longitud multidimensional variable:

![image](https://github.com/Pierohc/Java/assets/133154904/812486d7-9087-41a8-a486-0fbefebb4e72)

Imprimir matriz: Se necesita un doble for

    for(int i=0; i<3;i++){
    
        for(int j=0; j<5; j++){
        
        }
     }
--------------------------------------

# ArrayList:

Libreria para usar Array(herramiento para manejar arreglos):

    java.util.ArrayList;
    
![sd](https://github.com/Pierohc/Java/assets/133154904/cb37a48a-5ee7-4d2d-97ad-0bd7fb9591b5)

![Sin título](https://github.com/Pierohc/Java/assets/133154904/2fc7b0cd-4b77-46bb-8c56-1217f252db60)

![aaa](https://github.com/Pierohc/Java/assets/133154904/bf309d40-896b-4e9f-a08e-96793a0973c2)

------------------------------------
# Funcion Split:

        String correo = "a20200814@pucp.edu.pe";
        String partes[] = correo.split("@");

        System.out.println(partes[0]); //Imprimir solo un elemento del arreglo

        for (String eachPart : partes){ //Imprimir todo el arreglo
            System.out.println(eachPart);
        }

------------------------------------
# Verificar si una clase está vacía:

          if (nuevoEstudiante.getComputadora() == null){
              System.out.println("compu vacia");
          }


