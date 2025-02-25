# netxLine()

```java
// 3• (nextLine() consome o enter) nextLine() para Tudo Se você quiser evitar problemas
// com nextInt() e next(), pode usar nextLine() para capturar tudo como string e depois
// converter para números quando necessário:

import java.util.Scanner;

public class Aula {
  public static void main(String[] args){
      Scanner sc = new Scanner(System.in); // Criação do objeto Scanner

      // Solicita dos dados da primeira pessoa
      System.out.println("Informe os dados da primeira pessoa:");
      System.out.print("Nome: ");
      String nome1 = sc.nextLine(); // Captura o nome da primeira pessoa
      System.out.print("Idade: ");
      int idade1 = sc.nextInt(); // Captura a idade da primeira pessoa
      sc.nextLine(); // quebra de linha após o nextInt()

      // Solicita dos dados da segunda pessoa
      System.out.println("\nInforme os dados da segunda pessoa:");
      System.out.print("Nome: ");
      String nome2 = sc.nextLine(); // Captura o nome da segunda pessoa
      System.out.print("Idade: ");
      int idade2 = sc.nextInt(); // Captura a idade da segunda pessoa

      // Exibição da mensagem final
      System.out.println("\nMensagem Final:");
      System.out.println("O funcionário(a) " + nome1 + " tem " + idade1 + " anos.");
      System.out.println("O funcionário(a) " + nome2 + " tem " + idade2 + " anos.");

      sc.close(); // Fechamento do Scanner (opcional, mas recomendado)
  }
}
```

[next() e nextInt()](netxLine()%20196b8871e1d98090856be1bac3209be6/next()%20e%20nextInt()%20196b8871e1d980ec9358fb7a485d0025.md)