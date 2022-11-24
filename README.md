# TrabalhoFacul

package exercicio;

import java.text.SimpleDateFormat;
import java.util.Calendar;
import java.util.Random;
public class LeituraTemperatura {
    
    public static void main(String[] args) {
        SimpleDateFormat sfd = new SimpleDateFormat("HH:mm");
        Calendar hora = Calendar.getInstance();
        String horaFormatada = sfd.format(hora);
        Random gerador = new Random();
        for(int i=0; i < 100; i++){
            System.out.println(gerador.nextInt());
        }
         
        //int temperat [][] = new int [48][2];
       
    }
    
}
