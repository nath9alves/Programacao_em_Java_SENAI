# Java → equals() - Comparação de Strings

**O que é o método equals?**
O método equals() é uma função herdada da classe base Object, presente em qualquer objeto no Java. Ele é usado para comparar dois objetos e verificar se eles são "iguais".
Comportamento Padrão
Por padrão, o método equals() na classe Object verifica se dois objetos apontam para a mesma referência de memória (ou seja, se são o mesmo objeto).

```java

// 1º Exemplo:

import java.util.Scanner;

public class comparacao {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String nome = sc.next();
        System.out.println(nome.equals("Nathalia"));
    }
}

//----------------------------------------------------------------------------------------

// 2º Exemplo:

public class ComparacaoStrings {
    public static void main(String[] args) {
        String str1 = "Java";
        String str2 = "Java";
        String str3 = new String("Java");

        // Comparando as referências de objetos (não recomendado para conteúdo)
        System.out.println(str1 == str2); // true, porque as duas variáveis referenciam o mesmo objeto
        System.out.println(str1 == str3); // false, porque str3 é um novo objeto na memória

        // Comparando o conteúdo das strings
        System.out.println(str1.equals(str2)); // true, porque o conteúdo é o mesmo
        System.out.println(str1.equals(str3)); // true, porque o conteúdo é o mesmo

        // Comparando sem considerar maiúsculas e minúsculas
        String str4 = "java";
        System.out.println(str1.equalsIgnoreCase(str4)); // true, porque é ignorada a diferença de maiúsculas e minúsculas
    }
}
```