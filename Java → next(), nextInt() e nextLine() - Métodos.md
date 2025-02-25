# Java → next(), nextInt() e nextLine() - Métodos da classe Scanner

**1• método next() da classe Scanner é usado para capturar uma string (texto) digitada pelo usuário.
2• O método nextInt() é usado para capturar um número inteiro digitado pelo usuário.
3• (nextLine() consome o enter) nextLine() para Tudo Se você quiser evitar problemas com nextInt() e next(), pode usar nextLine() para capturar tudo como string e depois converter para números quando necessário:**

```java
//public class Aula {
//    public static void main(String[] args){
//        System.out.println("Bom dia!\n Boa noite");
//    }
//}

 
//----------------------------------------------------------------------------------

//import java.util.Scanner; // Importação da classe Scanner
//
//public class Aula {
//    public static void main(String[] args) {
//        Scanner sc = new Scanner(System.in); // Criação do Scanner
//        int a, b; // Declarando das variáveis
//
//        System.out.println("Informe dois números: ");
//
//        // Captura do primeiro número
//        System.out.print("Número 1: ");
//        a = sc.nextInt();
//
//        // Captura do segundo número
//        System.out.print("Número 2: ");
//        b = sc.nextInt();
//
//        // Exibição dos números informados
//        System.out.println("Você informou os números: " + a + " e " + b);
//
//        // Exemplo de operação: soma dos números
//        int soma = a + b;
//        System.out.println("A soma dos números é: " + soma);
//
//        sc.close(); // Fechamento do Scanner (opcional, mas recomendado)
//    }
//}

//---------------------------------------------------------------------------------------------------------------------

// 1 - Pergunte o nome e idade de duas pessoas respectivamente, e imprima a seguinte mensagem final: "O funcionário(a) <nome> tem <idade> anos.

//import java.util.Scanner;
//
//public class Aula {
//  public static void main(String[] args){
//      Scanner sc = new Scanner(System.in); // Criação do objeto Scanner
//
//      // Solicita dos dados da primeira pessoa
//      System.out.println("Informe os dados da primeira pessoa:");
//      System.out.print("Nome: ");
//      String nome1 = sc.nextLine(); // Captura o nome da primeira pessoa
//      System.out.print("Idade: ");
//      int idade1 = sc.nextInt(); // Captura a idade da primeira pessoa
//      sc.nextLine(); // quebra de linha após o nextInt()
//
//      // Solicita dos dados da segunda pessoa
//      System.out.println("\nInforme os dados da segunda pessoa:");
//      System.out.print("Nome: ");
//      String nome2 = sc.nextLine(); // Captura o nome da segunda pessoa
//      System.out.print("Idade: ");
//      int idade2 = sc.nextInt(); // Captura a idade da segunda pessoa
//
//      // Exibição da mensagem final
//      System.out.println("\nMensagem Final:");
//      System.out.println("O funcionário(a) " + nome1 + " tem " + idade1 + " anos.");
//      System.out.println("O funcionário(a) " + nome2 + " tem " + idade2 + " anos.");
//
//      sc.close(); // Fechamento do Scanner (opcional, mas recomendado)
//  }
//}

//---------------------------------------------------------------------------------------------------------------------

// --> Agora com três pessoas:

import java.util.Scanner;

public class Aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Declaração das variáveis
        String nome1, nome2, nome3; // Nomes devem ser do tipo String
        int idade1, idade2, idade3;

        // Captura dos dados da primeira pessoa
        System.out.println("Informe o nome da 1ª pessoa: ");
        nome1 = sc.next();                                      // método next() da classe Scanner é usado para capturar uma string (texto) digitada pelo usuário.
        System.out.println("Informe a idade da 1ª pessoa: ");
        idade1 = sc.nextInt();                                 // O método nextInt() é usado para capturar um número inteiro digitado pelo usuário.

        // Captura dos dados da segunda pessoa
        System.out.println("Informe o nome da 2ª pessoa: ");
        nome2 = sc.next();
        System.out.println("Informe a idade da 2ª pessoa: ");
        idade2 = sc.nextInt();

        // Captura dos dados da terceira pessoa
        System.out.println("Informe o nome da 3ª pessoa: ");
        nome3 = sc.next();
        System.out.println("Informe a idade da 3ª pessoa: ");
         idade3 = sc.nextInt();

        // Exibição dos dados coletados
        System.out.println("\nDados das pessoas:");
        System.out.println("1. " + nome1 + " tem " + idade1 + " anos.");
        System.out.println("2. " + nome2 + " tem " + idade2 + " anos.");
       System.out.println("3. " + nome3 + " tem " + idade3 + " anos.");

    }
}

```

[netxLine()](Java%20%E2%86%92%20next(),%20nextInt()%20e%20nextLine()%20-%20Me%CC%81todos%20d%20196b8871e1d9805881bae8bce4f66b0b/netxLine()%20196b8871e1d98090856be1bac3209be6.md)