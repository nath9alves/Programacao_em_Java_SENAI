# Exercício 3

**3- Crie uma função soma que pergunte dois valores e printe o resultado da soma destes valores em uma mensagem “O resultado da soma é: <resultado>”**

```java
import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        // Chamando a função que realiza a soma e imprime o resultado
        soma();
    }

    public static void soma() {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite os dois número: \n");
        double num1 = sc.nextDouble();
        double num2 = sc.nextDouble();

        // Calcula e exibe o resultado
        double resultado = num1 + num2;
        System.out.println("O resultado da soma é: " + resultado);

    }
}
```

[Exercício 4](Exerci%CC%81cio%203%201a4b8871e1d98042832afc9987b7e7c9/Exerci%CC%81cio%204%201a4b8871e1d980a9be87d7a0bebd074b.md)