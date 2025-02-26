# Java → for (){}- Estrutura de Repetição

**O comando for em Java é usado para criar laços (ou loops), ou seja, executar um bloco de código repetidamente por um número específico de vezes.**

```java
import java.util.Scanner;

public class geral {
    public static void main(String[] args){
       for(int i = 0;i<15;i = i + 1){   // Inicialização
           System.out.println("Olá mundo!");
       }
    }
}

//---------------------------------------------------------------------------------------

// --> **EXPLICAÇÃO:**

/* **Estrutura de repetição (for)
java**
        

**for(int i = 0; i < 15; i = i + 1) {}**

O que faz: Executa um bloco de código 15 vezes.

Explicação de cada parte:

**int i = 0;** → Declara a variável i e inicia com 0.
**i < 15;** → Define a condição: enquanto i for menor que 15, o loop continua.
**i = i + 1;** → Incrementa i em 1 a cada repetição.
💡 **Dica: i = i + 1 pode ser escrito de forma mais curta como i++*/

//---------------------------------------------------------------------------------------

// OUTRO EXEMPLO USANDO ++:

public class geral {
    public static void main(String[] args) {
        for (int i = 0; i < 15; i++) { // Usando i++ em vez de i = i + 1
            System.out.println("Olá mundo!");
        }
    }
}**

```

[Exercício 1 for(){}](Java%20%E2%86%92%20for%20()%7B%7D-%20Estrutura%20de%20Repetic%CC%A7a%CC%83o%20199b8871e1d9808db718c8b4a77337b9/Exerci%CC%81cio%201%20for()%7B%7D%20199b8871e1d98096b24ef846cd0a017d.md)

[Revisão for(){} e while (){}: Exercícios](Java%20%E2%86%92%20for%20()%7B%7D-%20Estrutura%20de%20Repetic%CC%A7a%CC%83o%20199b8871e1d9808db718c8b4a77337b9/Revisa%CC%83o%20for()%7B%7D%20e%20while%20()%7B%7D%20Exerci%CC%81cios%2019db8871e1d98064a709f074d157f69e.md)