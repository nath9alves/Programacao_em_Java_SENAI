# Exercício 4

//4. Escreva um programa que pergunte a nota de um aluno. Dada as ranges de conceitos, dê as seguintes respostas:
// < 20: Reprovado ; < 40 Rec 1 ; < 50 Rec 2 ; ≥ 50 Aprovado.

import java.util.Scanner;

public class geral {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int nota;

        System.out.println("Informe a nota do aluno: ");
        nota = sc.nextInt();

        if (nota < 20) {
            System.out.println("Reprovado!");
        }
        else if (nota < 40) {
            System.out.println("Recuperação 1!");
        }
        else if (nota < 50) {
            System.out.println("Recuperção 2");
        }
        else {
            System.out.println("Aprovado!");
        }
    }
}

//---------------------------------------------------------------------------------------

**// OBS:**

// Resumo da Estrutura de Condição:

if: Verifica se a nota é menor que 20. Se for, o aluno é reprovado.

java
Copiar
if (nota < 20) {
    System.out.println("Reprovado!");
}
else if: Se a primeira condição não for verdadeira (ou seja, se a nota não for menor que 20), verifica se a nota é menor que 40. Se for, o aluno está em recuperação 1.

java
Copiar
else if (nota < 40) {
    System.out.println("Recuperação 1!");
}
else if: Se as duas condições anteriores não forem verdadeiras, verifica se a nota é menor que 50. Se for, o aluno está em recuperação 2.

java
Copiar
else if (nota < 50) {
    System.out.println("Recuperação 2");
}
else: Se nenhuma das condições anteriores for atendida (ou seja, se a nota for 50 ou mais), o aluno está aprovado.

java
Copiar
else {
    System.out.println("Aprovado!");
}
