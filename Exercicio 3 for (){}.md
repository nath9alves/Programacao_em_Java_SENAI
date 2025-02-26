# Exercício 3 for (){}

//Faça um programa que pergunte o nome de uma pessoa e responda *“Bom dia <nome>!”*, repetindo o processo 5 vezes.

```java
import java.util.Scanner;

public class classefor {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        for (int i = 0; i < 5; i++) { // Repete o processo 5 vezes
            System.out.print("Digite seu nome: ");
            String nome = scanner.nextLine();
            System.out.println("Bom dia " + nome + "!");
        }

        scanner.close(); // Fecha o Scanner para evitar vazamento de memória
    }
}

