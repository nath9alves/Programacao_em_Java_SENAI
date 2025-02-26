# Java → Primeira Calculadora

```jsx
import java.util.Scanner;

public class aula {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int opcao;
        double num1, num2, resultado;

        do {  // Inicia um loop que executa o bloco de código pelo menos uma vez e 
              //repete enquanto a condição for verdadeira. Para que serve?: Permite que o usuário 
              //faça várias operações sem precisar reiniciar o programa.
              
            // Exibe o menu
            
            System.out.println("\n--- Calculadora ---\n");
            System.out.println("1. +");
            System.out.println("2. -");
            System.out.println("3. *");
            System.out.println("4. /");
            System.out.println("0. Sair\n");
            System.out.print("Escolha uma opção: ");
            opcao = scanner.nextInt();

            if (opcao != 0) {    // <-- "se" verdadeiro
                // Solicita os números ao usuário
                System.out.print("Digite o 1º número: ");
                num1 = scanner.nextDouble();
                System.out.print("Digite o 2º número: ");
                num2 = scanner.nextDouble();

                // Realiza a operação escolhida
                switch (opcao) {  // <-- Verifica o valor da variável opcao e executa o 
                                  //bloco de código correspondente.
                                  
                    case 1:   // Se a opção for 1, realiza a soma de num1 e num2 e exibe o resultado.
                        resultado = num1 + num2;
                        System.out.println("Resultado da soma: " + resultado);
                        break;
                    case 2:   // Se a opção for 2, realiza a subtração de num1 por num2 
                              // e exibe o resultado.
                        resultado = num1 - num2;
                        System.out.println("Resultado da subtração: " + resultado);
                        break;
                    case 3:   // Se a opção for 3, realiza a multiplicação de num1 por 
                              // num2 e exibe o resultado.
                        resultado = num1 * num2;
                        System.out.println("Resultado da multiplicação: " + resultado);
                        break;
                    case 4:   // Se a opção for 4, realiza a divisão de num1 por num2, 
                              // mas verifica se num2 é diferente de zero para evitar 
                              // erros.
                        if (num2 != 0) {
                            resultado = num1 / num2;
                            System.out.println("Resultado da divisão: " + resultado);
                        } else {
                            System.out.println("Erro: Divisão por zero!");
                        }
                        break;
                    default:   // Se o usuário digitar uma opção que não existe, exibe 
                               // uma mensagem de erro.
                        System.out.println("Opção inválida! Tente novamente.");
                }
            }
        } while (opcao != 0); // Repete até o usuário escolher sair

        
  // Mensagem de encerramento com delay e três pontinhos
        System.out.print("Calculadora encerrada!");
        try {
            for (int i = 0; i < 3; i++) {
                Thread.sleep(1000); // Delay de 1000
                System.out.print(".");
            }
            System.out.println(); // Pula uma linha após os pontinhos
        } catch (InterruptedException e) {
            System.out.println("Erro ao criar o delay.");
        }

        scanner.close();
    }
}
```