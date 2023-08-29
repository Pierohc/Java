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
          
          Scanner scanner = new Scanner(System.in); //creas un scanner que lo puede usar en todo el codigo
          String datoIngresado = scanner.nextLine();

Scanner todo lo guarda como String.
Si queremos ingresar un numero y luego convertirlo a entero:

                    int numero = Integer.parseInt(numeroString);

Si queremos convertir un True o False:
                    int opcion = Boolean.parse

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

break para while si usamos switch:
  
    buclePrincipal:

        switch{
          case 1:
            break;
          case2:
            break;
    
          case 3:
            breack bucle Principal;


---------------------------------
While:

    while(i<10){
      i++; 
      }
For:

    for(int i=1; i <=10; i++){

    }
        






