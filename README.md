//Los atributos deben ser privados.

//En el main se crean los objetos.

//CLASE_TIPODATO   nombre_propio = new CONSTRUCTOR

//getter <- para poder imprimir, te da el dato  

//setter <- Para asignar un valor o string

-----

String:

                    public String getNombre()
                    
                    public void setNombre(String nombre)

--------
Int:

                    public int getNumero()
                    
                    public void setNumero(int edad)

-------

Boolean:

                    public boolean isOpcion1()
                    
                    public void setOpcion1(boolean opcion)

--------------
LEER DATOS:

System.in para ingresar datos con el teclado.

scanner.nextLine() posiciona el cursos hasta que el usuario ingrese un dato y presione un enter, ese dato se guarda en una variable.

Recordar quitar el "ln" al println para que el cursor no este en la siguiente linea.

          Libreria: import java.util.Scanner;
          
          Scanner lector1 = new Scanner(System.in);
          String datoIngresado = scanner.nextLine();

Scanner todo lo guarda como String.
Si queremos ingresar un numero y luego convertirlo a entero:

                    int numero = Integer.parseInt(numeroString);

-----------------
CONDICIONALES:

if(opcion.equals("texto")){... Si el dato es String

if(opcion == 1){... Si el dato es Int



