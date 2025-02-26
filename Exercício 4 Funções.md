# Exercício 4

//**4- Refaça os exercícios dois e três porém agora fornecendo os dados como argumentos ao invés de fazer os scan na função**

```java
// ex 2

public class aula {
    public static void main(String[] args) {
        // Chamando a função e passando o nome como argumento
        felizAniversario("Maria");
    }

    public static void felizAniversario(String nome) {
        System.out.println("Feliz aniversário, " + nome + "!");
    }
}

//-------------------------------------------------------------------------------

// ex 3

public class SomaArgumentos {
    public static void main(String[] args) {
        // Chamando a função soma e passando os valores como argumentos
        soma(7, 5);
    }

    public static void soma(double num1, double num2) {
        // Soma os dois números e imprime o resultado
        double resultado = num1 + num2;
        System.out.println("O resultado da soma é: " + resultado);
    }
}
