# Exercício 2

**2- Crie uma função aniversario que, quando chamada, pergunte o nome do aniversariante e imprima “Feliz aniversário <nome>”**

```java
import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        // Chamando o método que executa o aniversário
        felizAniversario();
    }

    public static void felizAniversario() {
        Scanner sc = new Scanner(System.in); // Cria o Scanner para entrada de dados
        System.out.println("Informe o nome do aniversariante: ");
        String nome = sc.next(); // Lê o nome digitado pelo usuário
        System.out.println("Feliz aniversário, " + nome + "!");
        sc.close(); // Fecha o Scanner
    }
}

```

[Exercício 3](Exerci%CC%81cio%202%201a4b8871e1d980689ddddbd3aaf14f21/Exerci%CC%81cio%203%201a4b8871e1d98042832afc9987b7e7c9.md)