//1. **Crie um vetor para nomes e um para idades, cada um com 5 informações.** 
  //  1. **Informe a mensagem: “A pessoa <nome> tem <idade> anos sem utilizar o for.**
   // 2. **Após, repita o print, agora utilizando o for.** 
  //  3. **Imprima as informações de todos os usuários da lista, exceto o terceiro, utilizando o for**.



  ```java

import java.util.Arrays;
import java.util.ArrayList;
import java.util.Scanner;

public class aula {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        ArrayList<String> nomes = new ArrayList<>();
        ArrayList<String> idades = new ArrayList<>();

        System.out.println("\nInforme cinco nomes para completar a lista.");
        for (int i = 0; i < 5 ; i++){
            System.out.println("Informe o "+(i+1)+ " nome: ");
            String nome_novo = sc.nextLine();
            nomes.add(nome_novo);
        }

        System.out.println("Informe as idades correspondentes.");
        for (int i = 0; i <5; i++){
            System.out.println("Informe a "+(i+1)+ " idade: ");
            String idade_novo = sc.nextLine();
            idades.add(idade_novo);
        }

        System.out.println("A pessoa "+nomes.get(0)+ " possui "+idades.get(0)+" anos.\n");
        System.out.println("A pessoa "+nomes.get(1)+ " possui "+idades.get(1)+" anos.\n");
        System.out.println("A pessoa "+nomes.get(2)+ " possui "+idades.get(2)+" anos.\n");
        System.out.println("A pessoa "+nomes.get(3)+ " possui "+idades.get(3)+" anos.\n");
        System.out.println("A pessoa "+nomes.get(4)+ " possui "+idades.get(4)+" anos.\n");

    }
    
}

// -------------------------------------------------------------------------------------------------------------------------


import java.util.Arrays;
import java.util.ArrayList;
import java.util.Scanner;

public class aula {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        ArrayList<String> nomes = new ArrayList<>();
        ArrayList<String> idades = new ArrayList<>();

        System.out.println("\nInforme cinco nomes para completar a lista.");
        for (int i = 0; i < 5 ; i++){
            System.out.println("Informe o "+(i+1)+ " nome: ");
            String nome_novo = sc.nextLine();
            nomes.add(nome_novo);
        }

        System.out.println("Informe as idades correspondentes.");
        for (int i = 0; i <5; i++){
            System.out.println("Informe a "+(i+1)+ " idade: ");
            String idade_novo = sc.nextLine();
            idades.add(idade_novo);
        }
        for (int i = 0; i < 5; i++) {
            System.out.println("A pessoa " + nomes.get(i) + " possui " + idades.get(i) + " anos.\n");
        }


    }

}

// -------------------------------------------------------------------------------------------------------------------------


import java.util.Arrays;
import java.util.ArrayList;
import java.util.Scanner;

public class aula {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        ArrayList<String> nomes = new ArrayList<>();
        ArrayList<String> idades = new ArrayList<>();

        System.out.println("\nInforme cinco nomes para completar a lista.");
        for (int i = 0; i < 5 ; i++){
            System.out.println("Informe o "+(i+1)+ " nome: ");
            String nome_novo = sc.nextLine();
            nomes.add(nome_novo);
        }

        System.out.println("Informe as idades correspondentes.");
        for (int i = 0; i <5; i++){
            System.out.println("Informe a "+(i+1)+ " idade: ");
            String idade_novo = sc.nextLine();
            idades.add(idade_novo);
        }
        for (int i = 0; i < 5; i++) {
            if (i != 2) {
                System.out.println("Nome: " + nomes.get(i) + " Idade: " + idades.get(i));
            }
        }


    }

}
