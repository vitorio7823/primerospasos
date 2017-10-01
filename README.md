package pkg09.hombremujer;

import java.util.Scanner;
import javax.swing.JOptionPane;
////////////////////////////////////////////
///////////////////////////////////////////
////CAMBIOS///////////////////////////////////
////////////////////////////
/**
 *
 * @author victor
 */
public class HombreMujer {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner scan = new Scanner(System.in);

        char respuesta;
        int edad;
        System.out.println("Dime tu edad");
        edad = scan.nextInt();
        System.out.println("Dime si eres Hombre \"H\" o Mujer \"M\" ");
        respuesta = scan.next().charAt(0);

        if (edad >= 18 && (respuesta == 'H' || respuesta =='h')) {
            System.out.println("Eres hombre mayor de edad");

        }
        if (edad < 18 && (respuesta == 'H' || respuesta =='h')) {
            System.out.println("Eres hombre menor de edad");
        }
        if (edad >= 18 && (respuesta == 'M' || respuesta =='m')) {
            System.out.println("Eres mujer mayor de edad");

        }
        if (edad < 18 && (respuesta == 'M' || respuesta =='m')) {
            System.out.println("Eres mujer menor de edad");
        }

    }

}
