package operaciones;
import java.util.*;
public class Operaciones {

    
    public static void main(String[] args) {
        // TODO code application logic here
            Scanner leer = new Scanner(System.in);
            int a, b,opc;
            
            System.out.println("Escribe un numero");
            a = leer.nextInt();
            
            System.out.println("Escribe otro numero");
            b = leer.nextInt();
            /*con un (do{ }while) pódemos hacer que se vuelva a 
            regresar lo k uno quiera*/
            do{
            System.out.println("Selecciona la opcion a realizar");
            System.out.println("1)suma\n2)resta\n3)division\nmultiplicacion");    
            opc = leer.nextInt();
           
            switch(opc){
                case 1:
                    System.out.println("SUMAR");
                    System.out.println(a+b);
                    break;
                case 2:
                    System.out.println("RESTAR");
                    System.out.println(a-b);
                    break;
                case 3:
                    System.out.println("DIVICION");
                    System.out.println(a/b);
                    break;
                case 4:
                    System.out.println("MULTIPLICACION");
                    System.out.println(a*b);
                case 5:
                    System.out.println("modulo");
                    System.out.println(a%b);
                    break;
                default:
                    System.out.println("LA OPCION NO ES CORRECTA");
            }
            /*aqui ponemos la condicion y se regresara*/
            }while(opc < 10);
            
    }
}
