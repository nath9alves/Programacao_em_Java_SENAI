# Exercício 4 for (){}

//**4.** Pergunte para uma pessoa qual o mês de nascimento dela e responda qual o signo correspondente, repita 3x.

```java
import java.util.Scanner;

public class Signo {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in); // Scanner para entrada do usuário

        for (int i = 0; i < 3; i++) { // Repete o processo 3 vezes
            System.out.print("Digite o número do seu mês de nascimento (1 a 12): ");
            int mes = scanner.nextInt(); // Lê o número do mês

            String signo;

            switch (mes) {
                case 1:  signo = "Aquário ou Capricórnio"; break;
                case 2:  signo = "Peixes ou Aquário"; break;
                case 3:  signo = "Áries ou Peixes"; break;
                case 4:  signo = "Touro ou Áries"; break;
                case 5:  signo = "Gêmeos ou Touro"; break;
                case 6:  signo = "Câncer ou Gêmeos"; break;
                case 7:  signo = "Leão ou Câncer"; break;
                case 8:  signo = "Virgem ou Leão"; break;
                case 9:  signo = "Libra ou Virgem"; break;
                case 10: signo = "Escorpião ou Libra"; break;
                case 11: signo = "Sagitário ou Escorpião"; break;
                case 12: signo = "Capricórnio ou Sagitário"; break;
                default: signo = "Mês inválido!"; // Caso o número seja inválido
            }

            System.out.println("Seu signo pode ser: " + signo);
        }

        scanner.close(); // Fecha o Scanner para evitar vazamento de memória
    }
}
