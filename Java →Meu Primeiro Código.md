# Java →Meu Primeiro Código

```java

//OBS: print  escrever na mesma linha
//printf  formatar o texto
//println  quebra de linha

// Cabeçalho
   // Exibição da minha mensagem na tela

public class Primeiro_Codigo {
    public static void main(String[] args) {
        System.out.println("Olá Mundo");
     }
}

//------------------------------------------------------------------------------------------------------------------------
          //Atribuição da String nome

public class Primeiro_Codigo {
    public static void main(String[] args) {
        String nome;
        nome = "nathalia";
        System.out.println(nome);
    }
}

//------------------------------------------------------------------------------------------------------------------------

public class Primeiro_Codigo {
    public static void main(String[] args) {
        String nome;
        nome = "nathalia";
        int idade = 25;
        System.out.println(nome);
          System.out.println(idade);
       }
}

//------------------------------------------------------------------------------------------------------------------------

public class Primeiro_Codigo {
   public static void main(String[] args) {
       String nome;
       nome = "Nathalia";
       int idade = 25;
       System.out.printf("Meu nome é %s.%n", nome);
       System.out.println(idade);
      }
  }

//------------------------------------------------------------------------------------------------------------------------
// SCANNER: simplificar a leitura de diversas formas de entrada do usuário.

   // Para criar um objeto de scanner, precisamos primeiro importá-lo:
      // Após rodar o código, o cmd solicitará uma entrada do usuário. Aqui o sistema pergunta sua idade.

 import java.util.Scanner;

public class Primeiro_Codigo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String nome;
        nome = "Nathalia";
        int idade;
        idade = sc.nextInt();
        System.out.printf("meu nome é %s.%n", nome);
        System.out.println("E eu tenho "+idade+" anos");

    }
}

//------------------------------------------------------------------------------------------------------------------------

    // Após rodar o código, o cmd solicitará uma entrada do usuário. Aqui foi solicitado primeiro a idade e depois o nome, e caso o usuário não siga essa ordem, o sistema apresenta erro na execução.

import java.util.Scanner;

public class Primeiro_Codigo {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);
        String nome;
        nome = "Nathalia";
        int idade;
        idade = leitor.nextInt();
        nome = leitor.next();
        System.out.printf("meu nome é %s.%n", nome);
        System.out.println("E eu tenho "+idade+" anos");

    }
}

//------------------------------------------------------------------------------------------------------------------------

// -> Exercício 1: CRIE UM PROGRAMA QUE PERGUNTE O NOME DO USUÁRIO E SUA IDADE. IMPRIMA A MENSAGEM: " Bom dia <user>, parabéns pelos seus <idade> anos".

import java.util.Scanner;  //<-- Importando o scanner

public class Primeiro_Codigo {
    public static void main(String[] args) {
        Scanner leia = new Scanner(System.in);  //<-- Declarando o Scanner como "leia"

          String nome; int idade;                 //<-- declarando o nome e a "idade" como int

        System.out.println("Informe seu nome:");   //<-- Java pergunta p/ o usuário juntamente com a mensagem de solicitação.

           nome = leia.next();                    // <-- a string nome resulta no scanner leia

        System.out.println("Agora informe sua idade:"); // <-- Java pergunta p/ o usuário juntamente com a mensagem de solicitação.

           idade = leia.nextInt();                 //<-- a string idade resulta no scanner leia

        System.out.println("Bom dia "+nome+", parabéns pelos seus "+idade+" anos.");  //<-- Java apresenta a mensagem final ao usuário

    }
}

```

[Scanner simples em Java ](Java%20%E2%86%92Meu%20Primeiro%20Co%CC%81digo%20192b8871e1d980ac8ce8c0609d799c38/Scanner%20simples%20em%20Java%20192b8871e1d980c899b0fbba85d35daa.md)