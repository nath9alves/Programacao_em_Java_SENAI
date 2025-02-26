// 2 - Crie um vetor com 4 nomes fornecidos pelo usuário. Ao final, imprima a mensagem: “Bem vindo <nome>” para cada um deles.

```java

import java.util.Arrays;
import java.util.ArrayList;
import java.util.Scanner;

public class aula {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        ArrayList<String> nomes = new ArrayList<>();

        System.out.println("Informe quatro nomes:");
        String nome = sc.nextLine();

        for (int i = 1;i <4; i++ ){
            System.out.println("Informe o "+(i + 1)+ " nome: ");
            String nome_novo = sc.nextLine();
            nomes.add(nome_novo);
        }
        for (String a: nomes){
            System.out.println("Bem vindo "+a);
        }

    }
}
