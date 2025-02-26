# Revisão for(){} e while (){}: Exercícios

**1. --> Repita 10 vezes a frase "Olá SENAI!”**

```java
 public class aula {
    public static void main(String[] args) {
    System.out.println("Iniciando...");

                for(int i = 0;i<10;i++){
                    System.out.print("\nOlá SENAI!");
                }
    }
}
```

1. **-> EXERCÍCIO: SEM O USO DO for CRIE UM RETORNO COM 5 NOMES. CRIE TAMBÉM UM VATOR DE 5 IDADES. IMPRIMA A MENSAGEM:
A pessoa 'nome', possui idade 'anos'. Após terminar, refaça a impressão utilizando o for para iterar entre os vetores."**

```java
public class aula {
    public static void main(String[] args) {
    System.out.println("Repetição de nomes e idade: ");

        String[] nome = {"Nathalia", "Marcelo", "Adriana", "Daniel", "Márcia"};
        int[] anos = {25, 30, 42, 55, 60};

        System.out.println("A pessoa " + nome[0] + " possui idade " + anos[0] + " anos.");
        System.out.println("A pessoa " + nome[1] + " possui idade " + anos[1] + " anos ");
        System.out.println("A pessoa " + nome[2] + " possui idade " + anos[2] + " anos ");
        System.out.println("A pessoa " + nome[3] + " possui idade " + anos[3] + " anos ");
        System.out.println("A pessoa " + nome[4] + " possui idade " + anos[4] + " anos ");

    System.out.print("Finalizando...");

    }
}
```

**• Com for:**

```java
public class aula {
    public static void main(String[] args) {
        System.out.println("Repetição de nomes e idade: ");

        String[] nome = {"Nathalia", "Marcelo", "Adriana", "Daniel", "Márcia"};
        int[] anos = {25, 30, 42, 55, 60};

        for (int i = 0; i < nome.length; i++) {
            System.out.print("\nA pessoa " + nome[i] + " possui idade " + anos[i] + " anos \n");
        }

    System.out.print("\nFinalizando...\n");
    }
}
```

**EXERCÍCIO: 1. --> Crie um vetor de Strings com 10 nomes. Percorra estes 10 nomes informando uma mensagem de “Bem vindo <nome>”**

```java
public class aula {
    public static void main(String[] args) {
        System.out.println("Iniciando....");

        String[] nome = {"Maria", "Jailson", "Isabel", "Jonathan", "Arthur", "José", "Nathalia", "Everson", "Cícero", "Ana",};

        for (int i = 0; i < nome.length; i++) {
            System.out.print("\nBem vindo, " + nome[i]);
        }
    }
}
```

**EXERCÍCIO: 2. --> Crie um vetor com 4 nomes fornecidos pelo usuário. Ao final, imprima a mensagem: “Bem vindo <nome>”**

```java
 import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        System.out.println("Iniciando....");
        Scanner sc = new Scanner(System.in);

        String[] nome = new String[4];

        for(int i = 0;i<4;i++){
            System.out.print("Digite o seu nome: ");
            nome[i] = sc.nextLine();
        }

        for (int i = 0;i < 4; i++){
            System.out.println("Bem-vindo, " + nome[i] + "!");
        }

    }
} 
```

• Imprima todos os nomes da lista, exceto o terceiro utilizando o for:

```java
import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        System.out.println("Iniciando....");
        Scanner sc = new Scanner(System.in);

        String[] nome = new String[4];

        for(int i = 0;i<4;i++){
            System.out.print("Digite o seu nome: ");
            nome[i] = sc.nextLine();
        }

        for (int i = 0;i < 4; i++) {
            if (i != 2 ) {    // --> **diferente** de 2, pois 2 é o dígito que representa o terceiro.
                System.out.println("Bem-vindo, " + nome[i] + "!");
            }

        }

    }
}
```

**EXERCÍCIO: 3 -->Crie uma lista de mercado com 5 produtos e 5 preços informados pelo usuário. Ao final, imprima uma mensagem para cada produto, informando quanto eles custam.**

```java
import java.util.Scanner;

public class aula {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);

        String[] produto = new String[5];
        String[] preco = new String[5];

        for (int i = 0;i < 5; i++){
            System.out.print("Informe um produto " +(i +1)+ ":");
            produto[i] = sc.nextLine();
        }

        for (int i = 0;i < 5; i++){
            System.out.print("Informe o preço do produto " +(i +1)+":");
            preco[i] = sc.nextLine();
        }

        for (int i = 0; i < 5; i++) {
            System.out.println("O produto " + produto[i] + " está custando: " + preco[i]);
        }

    }
}
```

**EXERCÍCIO: 4 --> Você é dono de uma pizzaria e gostaria de registrar 5 pizzas em um vetor que já contém 5 sabores, totalizando 10 sabores. Cada sabor deve ter um preço atrelado a ele (double).  Crie uma sequência aonde os 5 próximos sabores e valores devem ser cadastrados utilizando um for.  Ao final, printe todo os 10 sabores e preços das pizzas**

```java
import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String[] sabores = {" Calabresa", "Frango", "Queijo", "Costela", "Brócolis", "", "", "", "", ""};
        double[] precos = {35.0, 40.0, 28.0, 55.0, 35.0, 0.0, 0.0, 0.0, 0.0, 0.0};

        for (int i = 5; i < 10; i++) {
            System.out.print("Informe o novo sabor da pizza: ");
            sabores[i] = sc.nextLine();
        }
        for (int i = 5;i < 10;i++){
            System.out.println("Informe o preço da pizza: "+sabores[i]);
            precos[i] = sc.nextDouble();
        }
        for (int i = 5;i < 10;i++){
            System.out.print("\nO novo sabor de "+sabores[i]+"custa o valor de "+precos[i]);
        }
        
        System.out.print("Finalizando...");
    }
}

// Outra forma:

import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String[] sabores = {"Calabresa", "Frango", "Queijo", "Costela", "Brócolis", "", "", "", "", ""};
        double[] precos = {35.0, 40.0, 28.0, 55.0, 35.0, 0.0, 0.0, 0.0, 0.0, 0.0};

        for (int i = 5; i < 10; i++) {
            System.out.print("Informe o novo sabor da pizza: ");
            sabores[i] = sc.nextLine();

            System.out.print("Informe o preço da pizza " + sabores[i] + ": ");
            precos[i] = sc.nextDouble();
            sc.nextLine(); 
        }

        System.out.println("\nSabores e preços das pizzas:");
        double total = 0.0; // Variável para armazenar a soma dos preços

        for (int i = 0; i < 10; i++) { // 
            System.out.println("Sabor: " + sabores[i] + " | Preço: R$ " + precos[i]);
            total += precos[i]; // Soma os preços
        }

        // Exibindo o valor total
        System.out.println("\nO total dos preços das pizzas é: R$ " + total);

        System.out.println("Finalizando...");

    }
}

```

**EXERCÍCIO: 5 —> Crie um sistema de login aonde você terá 5 códigos de usuários pré cadastrados. O usuário terá que digitar um (de números inteiros) e, se ele existir, digitar a senha correspondente (também de números inteiros).
Caso ele consiga acertar, informe login efetuado com sucesso. Ele deve ter 3 tentativas e depois exibir uma mensagem de “acesso negado”, terminando o programa, caso ele erre.**

```java
import java.util.Scanner;

public class aula {
    public static void main(String[] args) {

        int[] codigo = new int[100];    // <-- Arrays p/ armazenar os dados dos usuários (até 100 dígitos em senha e código).
        int[] senha = new int[100];

        for (int i = 0; i < 100; i++) {
            codigo[i] = 1000 + i;    // <-- aceita códigos e senhas de 1000 até 1099 dígitos.
            senha[i] = 2000 + i;    // <-- senha de 2000 até 2099.
        }

        Scanner sc = new Scanner(System.in);
        int tentativas = 3;    // <-- o usuário terá direito a 3 tentativas de login.

        while (tentativas > 0) {    // <-- while serve p/ repetir um bloco de código enquanto uma condição específica for verdadeira.
            System.out.print("Informe seu código de acesso: ");
            int codigousuario = sc.nextInt();

            boolean codigoencontrado = false;
            int indiceuser = -1;

            for (int i = 0; i < codigo.length; i++) {
                if (codigo[i] == codigousuario) {
                    codigoencontrado = true;
                    indiceuser = i;  // Corrigido: indiceuser deve ser o índice onde o código foi encontrado
                    break;    // <-- Vai "parar" o processo
                }
            }

            if (codigoencontrado) {
                System.out.print("Informe sua senha: ");
                int senhaacesso = sc.nextInt();

                if (senha[indiceuser] == senhaacesso) {
                    System.out.print("Login realizado!");
                    return;    // <-- Encerra o processo após o usuário ter feito o login
                } else {
                    System.out.print("Falha no login! Tente novamente\n");
                }
            } else {
                System.out.print("Código de acesso não encontrado! Tente novamente\n");
            }

            tentativas--;
            if (tentativas > 0) {
                System.out.print("Restam mais " + tentativas + " tentativas.\n");
            } else {
                System.out.print("Acesso negado!\n");
            }
        }
    }
}
```

1.