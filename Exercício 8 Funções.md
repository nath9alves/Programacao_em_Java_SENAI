# Exercício 8

//**8- Crie um programa que pergunte ao usuário quantos números ele quer somar e, em seguida, receba estes números. A partir destes números fornecidos, faça com que o programa retorne a soma destes números para o programa, realizando então um print do resultado.**

```java
import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("--- Soma de Números ---");

        // Pergunta ao usuário a quantidade de números
        System.out.print("Quantos números você deseja somar? ");
        int quantidade = sc.nextInt();

        // Verifica se a quantidade é válida
        if (quantidade <= 0) {
            System.out.println("Erro: Digite novamente!.");
        } else {
            // Recebe os números e calcula a soma
            double resultado = calcularSoma(sc, quantidade);

            // Exibe o resultado
            System.out.printf("A soma dos números é: %.2f\n", resultado);
        }
    }

    /**
     * Função para calcular a soma dos números fornecidos pelo usuário.
     *
     * @param sc        Scanner para leitura de entradas.
     * @param quantidade Quantidade de números a somar.
     * @return Soma dos números.
     */
     
    public static double calcularSoma(Scanner sc, int quantidade) {
        double soma = 0;

        // Loop para receber os números e somá-los
        for (int i = 1; i <= quantidade; i++) {
            System.out.print("Informe o número " + i + ": ");
            double numero = sc.nextDouble();
            soma += numero;
        }

        return soma;
    }
}
