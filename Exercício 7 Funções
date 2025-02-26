# Exercício 7

//**7- Crie um programa de calculadora que permita ao usuário fornecer dois números e escolher uma das 4 operações básicas e retorne o resultado da operação para o programa, printando-o em seguida.**

```java
import java.util.Scanner;

public class aula {
    public static void main(String[] args) {

        System.out.println("--- Calculadora ---");

        double resultado = calculadora();
        System.out.println("O resultado da operação é: " + resultado);
    }

    public static double calculadora() {
        Scanner sc = new Scanner(System.in);
        System.out.println("Informe dois números: \n");
        double num1 = sc.nextDouble();
        double num2 = sc.nextDouble();
        System.out.println("Escolha a operação: ");
        System.out.println("1 --> +");
        System.out.println("2 --> -");
        System.out.println("3 --> *");
        System.out.println("4 --> /");
        int operacao = sc.nextInt();

        double resultado = 0;

        switch (operacao) {
            case 1:
                resultado = num1 + num2;
                break;

            case 2:
                resultado = num1 - num2;
                break;

            case 3:
                resultado = num1 * num2;
                break;

            case 4:
                if (num2 != 0) {
                    resultado = num1 / num2;
                }
                else{
                    System.out.println("Erro! tente novamente");
                }
                break;
            default:
                System.out.println("Opção Inválida! Tente novamente");

        }
        return resultado;
    }
}

```

**Outra forma com opção de encerrar e tentar novamente!**

```java
import java.util.Scanner;

public class Aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        boolean continuar = true;

        System.out.println("--- Calculadora ---");

        // Loop para continuar ou encerrar a calculadora
        while (continuar) {
            // Chama a função calculadora que executa a lógica principal
            double resultado = calculadora(sc);

            // Exibe o resultado
            System.out.printf("O resultado da operação é: %.2f\n", resultado);

            // Pergunta ao usuário se deseja continuar ou sair
            System.out.print("Deseja realizar outra operação? (S para Sim / N para Não): ");
            char resposta = sc.next().toUpperCase().charAt(0);

            // Se o usuário digitar 'N' ou 'n', encerra o programa
            if (resposta == 'N') {
                continuar = false;
                System.out.println("Calculadora encerrada. Até mais!");
            }
        }
    }

    public static double calculadora(Scanner sc) {
        // Solicita os dois números ao usuário
        System.out.print("Informe os dois números: ");
        double num1 = sc.nextDouble();
        double num2 = sc.nextDouble();

        // Exibe as opções de operações
        System.out.println("Escolha a operação: ");
        System.out.println("1 --> Soma (+)");
        System.out.println("2 --> Subtração (-)");
        System.out.println("3 --> Multiplicação (*)");
        System.out.println("4 --> Divisão (/)");
        int operacao = sc.nextInt();

        // Variável para armazenar o resultado
        double resultado = 0;

        // Lida com a escolha do usuário
        switch (operacao) {
            case 1:
                resultado = num1 + num2; // Soma
                break;
            case 2:
                resultado = num1 - num2; // Subtração
                break;
            case 3:
                resultado = num1 * num2; // Multiplicação
                break;
            case 4:
                if (num2 != 0) { // Proteção contra divisão por zero
                    resultado = num1 / num2; // Divisão
                } else {
                    System.out.println("Erro: Não é possível dividir por zero!");
                    return 0; // Retorna 0 como resultado em caso de erro
                }
                break;
            default:
                System.out.println("Opção inválida! Escolha uma operação entre 1 e 4.");
                return 0; // Retorna 0 como resultado em caso de erro
        }

        // Retorna o resultado da operação
        return resultado;
    }
}
