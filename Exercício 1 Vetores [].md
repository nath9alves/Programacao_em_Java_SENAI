# Exercício 1

**1-Crie um vetor manualmente com os doze meses do ano**

```java
import java.util.Scanner;

public class classefor {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String[] meses = {
                "Janeiro", "Fevereiro", "Março", "Abril", "Maio", "Junho",
                "Julho", "Agosto", "Setembro", "Outubro", "Novembro", "Dezembro"
        };
        
        for (int i = 0; i <meses.length; i++){
        }
        
        System.out.println("Digite um número de 1 a 12 para exibir o mês correspondente: ");
        int escolha = scanner.nextInt();

        if (escolha >= 1 && escolha <= 12){
            System.out.println("O mês é: "+meses[escolha - 1]);
        }
        else {
            System.out.println("Inválido! Digite novamente.");
        }

    }
}

```