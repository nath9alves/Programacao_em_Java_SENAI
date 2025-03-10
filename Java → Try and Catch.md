```java

// Exemplo 1
 
import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner (System.in);
        //int a = sc.nextInt();
        try{
            int b = 10/0;
            System.out.println(b);
        } catch (Exception erro)
        {
            System.out.println("não consegui, o erro foi: " +erro);
        }

    }

}

//---------------------------------------------------------------------------------------------------

//Exemplo 2

import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite um número inteiro: ");
        int a = sc.nextInt(); 

        try {
            int b = 10 / a; 
            System.out.println("Resultado da divisão: " + b);
        } catch (ArithmeticException erro) { // Captura erro de divisão por zero
            System.out.println("Erro: Divisão por zero não permitida.");
        } catch (Exception erro) { // Captura qualquer outro erro inesperado
            System.out.println("Erro inesperado: " + erro.getMessage());
        }
        
    }
}

//---------------------------------------------------------------------------------------------------

import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = 0;

        while (true) {  // O laço vai continuar até que o usuário forneça uma entrada válida
            try {
                System.out.print("Digite um número inteiro: ");
                a = sc.nextInt();  // Lê a entrada do usuário

                // Tentando a divisão por "a" (código crítico)
                int b = 10 / a;
                System.out.println("Resultado da divisão: " + b);
                break;  // Se a divisão for bem-sucedida, sai do loop
            } catch (ArithmeticException erro) {
                System.out.println("Erro: Divisão por zero não permitida. Tente novamente.");
            } catch (Exception erro) {
                System.out.println("Erro inesperado: " + erro.getMessage());
                sc.next();  // Limpa o buffer do scanner em caso de erro na entrada
            }
        }

    }
}
