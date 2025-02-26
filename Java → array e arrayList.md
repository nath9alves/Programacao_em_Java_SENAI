# Java → array e arrayList

**Array: O que é?**

O que é: Um array é uma estrutura de dados em que podem ser armazenados vários elementos de mesmo tipo (inteiros, strings, objetos, etc.).
Tamanho fixo: Ao criar um array, você precisa definir seu tamanho, e ele não pode ser alterado depois.
Acesso por índice: Os elementos são acessados por índices numéricos, começando do 0.

```java
  int[] numeros = new int[5]; // Array de inteiros com 5 posições
  numeros[0] = 10;           // Insere o valor 10 na posição 0
  System.out.println(numeros[0]); // Imprime o valor 10
```

**ArrayList: O que é?**

O que é: Uma ArrayList é uma classe da biblioteca do Java que armazena elementos de forma dinâmica.
Tamanho dinâmico: Ao contrário de arrays, o tamanho de uma ArrayList pode crescer ou diminuir conforme novos elementos são adicionados ou removidos.
Mais funcional: Oferece métodos úteis, como adicionar, remover e buscar elementos facilmente.
Pertence ao pacote: Está na coleção java.util.

```java
  import java.util.ArrayList;

  ArrayList<String> nomes = new ArrayList<>();
  nomes.add("Maria");           // Adiciona "Maria" na lista
  nomes.add("João");            // Adiciona "João"
  System.out.println(nomes);    // Imprime: [Maria, João]
  nomes.remove("Maria");        // Remove "Maria"
  System.out.println(nomes);    // Imprime: [João]
```

```java
import java.util.Scanner;
import java.util.ArrayList;

public class aula {
    public static void main(String[] args){
    
    Scanner sc = new Scanner(System.in);
    
    ArrayList<String> nomes = new ArrayList<>();
   
    nomes.add("Nathalia");nomes.add("Serafim"); nomes.add("Maria");
    
    while(true){
        System.out.println("Informe um nome ou 'vazio' para parar");
        String nome = sc.next();
        
        if(!nomes.equals("")) {
            nomes.add(nome);
        }
        else if(nome.equals("vazio")){}
        break;
    }
        System.out.println(nomes.toString());
    }
}

```

[Exercício das frutas](Java%20%E2%86%92%20array%20e%20arrayList%201a5b8871e1d980a7b54cd1014b4ee48e/Exerci%CC%81cio%20das%20frutas%201a5b8871e1d98056a05cee41b3024d18.md)