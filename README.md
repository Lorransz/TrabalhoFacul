package exercicio;

import java.text.SimpleDateFormat;
import java.util.Calendar;
import java.util.Random;
import javax.swing.JOptionPane;

public class temperatura {

    public static void main(String[] args) {
        //DATA
        SimpleDateFormat sfd = new SimpleDateFormat("HH:mm");
        Calendar hora = Calendar.getInstance();
        String horaFormatada = sfd.format(hora);
            //Declaração  da Matriz       
            int temp[][] = new int[48][2];
            //Número Random
            Random numeroRandom = new Random ();
                for (int i=0; i<temperatu.length; i++) {
                for (int j= 0; j<tempo.length; j++) {
                numeroRandom[i] = temp.nextInt(100);

                }

            }
            //Entrada   
            for (int tempe = 0; tempe < 48; tempe++) {
                int tempo = 0;
                JOptionPane.showMessageDialog(null, "Temperatura atual: " + temp[tempe][tempo]);
                for (tempo = 0; tempo < temp.length; tempo++) {
                    JOptionPane.showMessageDialog(null, "Tempo atual: " + temp[tempe][tempo]);

               }
           }
       }

 }

