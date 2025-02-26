# Java → Strings

**1- A partir de um nome informado pelo usuário, mostre aquele nome em letras maiúsculas.**

```java

import java.util.Scanner;

public class aula {

    public static void main(String[] args) {
    
        Scanner scanner = new Scanner(System.in);
        
        String nome;
        
        System.out.println("Digite seu nome: ");
        
        nome = scanner.nextLine();

        String nomemaisculo = nome.toUpperCase().replace("", "");

        System.out.printf(nomemaisculo);

    }
}
```

**2- Salve seu nome completo em uma variável do tipo String. Imprima todos os elementos do seu nome completo, um em cada print, utilizando métodos de string**

```java
import java.util.Scanner;

public class aula {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

      String nome;

      System.out.println("Digite seu nome completo: ");
      nome = sc.nextLine();

      String[] nomes = nome.split(" ");

        System.out.println("\nSeu nome completo por partes é: \n");
        for (String parte : nomes){
            System.out.println(parte);
        }

    }
}
```

**3- A partir de um CPF informado, verifique se, após retirar os espaços iniciais, finais, pontos e traços, ele tem onze dígitos. Caso sim, informe CPF válido e encerre o programa. Caso contrário, informe a mensagem “Favor digitar somente números e onze dígitos.” e deixe que o usuário tente novamente, até conseguir.**

```java
import java.util.Scanner;

public class aula {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        while (true) {
            System.out.println("Digite um CPF");
            String cpf = sc.nextLine();
            if (cpf.length() == 11)
                System.out.println("CPF Válido!");

            else if (cpf.length() != 11) {
                System.out.println("CPF Inválido! Digitar 11 dígitos para continuar.");
                continue;
            }

            break;

        }
    }
}
```