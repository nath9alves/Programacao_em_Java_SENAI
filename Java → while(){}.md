# Java → while(){}

1. **Crie uma variável chamada a.<a> começa com um valor de 0. Faça com que a chegue até o valor 100, com incrementos de 1, e depois faça com que o programa se encerre sozinho. Utilize while.**

```java

public class whileclass {
    public static void main(String[] args) {

       int a = 0;

       while(a<=101){    // <-- Continua enquanto 'a' for menor ou igual a 100.
           System.out.println("Valor atual de a: "+a);
           a++;    // incrementar o valor de indice e me retornar o valor já incrementado
       }

       System.out.println("Fim do programa. 'a' atingiu 100!");

    }
}
```

1. **Utilizando o while, escreva 'Bom dia' 15 vezes**

```java
public class whileclass {
    public static void main(String[] args) {

        int bom_dia = 0;

        while(bom_dia <= 15){
            System.out.println("Bom dia! : "+bom_dia);
            bom_dia++;    // Incrementa o valor de 'a' em 1

        }

        System.out.print("Fim do programa");

        try {
            // Loop para adicionar os três pontos com delay
            for (int i = 0; i < 3; i++) {
                Thread.sleep(1000); // Pausa de 1000 milissegundos (0.5 segundos)
                System.out.print(".");
            }
        } catch (InterruptedException e) {
            e.printStackTrace();
        }

        System.out.println(); // Para pular uma linha após a mensagem
    }
}
```

1. **Faça um programa utilizando while que some dois números 
para o usuário e entregue o resultado da soma logo em 
seguida, repetindo infinitamente.**

```java
import java.util.Scanner;

public class whileclass {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        while (true) {
            System.out.print("Informe o primeiro número: ");
            int num1 = sc.nextInt();

            System.out.print("Informe o segundo número: ");
            int num2 = sc.nextInt();

            int soma = num1 + num2;

            System.out.print(" Resultado da soma: " + soma + "\n");

            System.out.print("Deseja continuar? (S/N) ");
            String continuar = sc.next();
            if (continuar.equalsIgnoreCase("N")) {
                System.out.println("Programa finalizado!");
                break;
            }
        }

    }
}
```