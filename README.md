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
        //Int Random
        Random gerador = new Random();
        for (int i = 0; i < 100; i++) {
            System.out.println(gerador.nextInt());
            //Declaração  da Matriz       
            int temp[][] = new int[48][2];
            
            for (int tempe = 0; tempe < temp.length; tempe++) {
                String entrada = JOptionPane.showInputDialog(null, "Digite a temperatura: ");
                for (int tempo = 0; tempo < temp.length; tempo++) {
                    entrada = JOptionPane.showInputDialog(null, "Digite o tempo da leitura: ");
                    double ent = Double.parseDouble(entrada);
                    temp[tempe][tempo] = ent;

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
}
