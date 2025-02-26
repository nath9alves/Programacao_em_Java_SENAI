# Exercício 1

```java
// 1. Crie um programa que, pergunte a nota de um aluno e verifique se ele passou 
// na nota de corte (acima de 50)

import java.util.Scanner;

public class geral {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        int nota;

        System.out.println("Informe sua nota: ");
        nota = sc.nextInt();

        if (nota >= 50){
            System.out.print("Aprovado!");
        }

        if (nota < 50){
            System.out.print("Reprovado!");
        }
    }
}

```

[Exercício 2](Exerci%CC%81cio%201%20199b8871e1d980fca779f0c0688b32e8/Exerci%CC%81cio%202%20199b8871e1d980d2853ee0e82a298bd4.md)