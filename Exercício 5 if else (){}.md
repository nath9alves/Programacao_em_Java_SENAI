# Exercício 5

- 5. O programa deve: responder se o aluno foi aprovado. Receber os dados de um aluno ou do senai vila alpina ou do
mooca. Se ele for do senai vila alpina, no curso de python ele deve ter pelo menos 60 de nota e 75% de frequência. Se
ele for do senai mooca, também do curso de python, ele deve ter a mesma quantidade de presença porém com uma nota de 50
ele já consegue ser aprovado.

```java

import java.util.Scanner;

public class classefor {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite a unidade (Vila Alpina ou Mooca): ");
        String unidade = sc.nextLine(); // Pula uma linha e segue p/ a próxima

        System.out.print("Digite o curso: ");
        String curso = sc.nextLine();

        System.out.print("Digite a nota do aluno: ");
        double nota = sc.nextDouble();

        System.out.print("Digite a frequência do aluno (%): ");
        double frequencia = sc.nextDouble();

        // Verifica se é do curso de Python e aplica as regras de aprovação
        if (curso.equals("Python") && (     // <-- Digite Python quando o programa solicitar o curso
                (unidade.equals("Vila Alpina") && nota >= 60 && frequencia >= 75) || // <-- Digite Vila Alpina quando o programa solicitar
                        (unidade.equals("Mooca") && nota >= 50 && frequencia >= 75)  // <-- Digite Mooca quando o programa solicitar
        )) {
            System.out.println("O aluno foi APROVADO!");}
        else {
            System.out.println("O aluno foi REPROVADO!");}

    }
}

```

**Explicação**:

A classe **String** é usada para armazenar textos (sequências de caracteres). Como a unidade e o curso são informações que consistem em palavras e não números, o tipo mais apropriado para armazená-las é String.

Por que não usamos int ou double?
Se usássemos **int**, teríamos problemas ao armazenar nomes como "Vila Alpina".
**double** é usado para números decimais, mas não faz sentido aqui.
💡 O **String** é a melhor escolha porque permite que o usuário **insira qualquer texto, como "Python" ou "Mooca".**
