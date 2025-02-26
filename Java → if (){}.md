# Java → if (){}

Nesse exercício estou perguntando as horas com valor inteiro e, dependendo do horário, o sistema retorna “bom dia”, “boa tarde” ou “boa noite.

```java
// Exercício: Perguntar que hora são usando apenas o if. Caso seja das 06 as 11 
//será bom dia e assim por diante.

import java.util.Scanner;

public class NomeDaClasse {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        int hora;

        System.out.println("Que horas são agora? ");
        hora = sc.nextInt();

        if (hora >= 5 && hora <11) {
            System.out.println("Bom dia");
        }
        if (hora >= 12 && hora <17){
            System.out.println("Boa tarde");
        }
        if (hora >= 18){
            System.out.println("Boa noite");
        }
        if (hora <= 4){
            System.out.println("Boa noite");
        }

        System.out.println("Obrigada!");
    }
}
```

[Java → Exercícios 12_02 if else](Java%20%E2%86%92%20if%20()%7B%7D%20197b8871e1d980a097fec69131039e04/Java%20%E2%86%92%20Exerci%CC%81cios%2012_02%20if%20else%20198b8871e1d980ad9503db62117f1eb8.md)

[Java → if(){} Código simples](Java%20%E2%86%92%20if%20()%7B%7D%20197b8871e1d980a097fec69131039e04/Java%20%E2%86%92%20if()%7B%7D%20Co%CC%81digo%20simples%20196b8871e1d9802fb196e1270efb3aee.md)