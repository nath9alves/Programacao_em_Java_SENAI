# Exercício 2

**-Crie um vetor de Strings com 3 nomes informados pelo usuário:**

```java
import java.util.Scanner;

public class classefor {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String[] nomes = {"Nath","Washington","Maria"};
        System.out.println("Meu nome é: "+nomes[0]);
        System.out.println("Meu pai é: "+nomes[1]);
        System.out.println("Minha mãe é: "+nomes[2]);

        int[] numeros = new int[10];

        numeros[3] = 355;

        System.out.println(numeros[3]);
    }
}

```
