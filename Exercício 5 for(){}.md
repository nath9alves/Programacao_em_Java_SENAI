# Exercício 5 for(){}

**5.** Seu cliente precisa saber o salário dos funcionários de acordo com seu código de cadastro.

Os funcionários foram cadastrados em ordem cronológica e tem códigos de cadastros que começam em 700, e se alteram se 7 em 7, de forma decrescente, fazendo com que um número seja par, e o seguinte, ímpar. 

Sabendo que a empresa tem 60 funcionários, e os funcionários de número par recebem 4 vezes seu código em R$ de bônus, informe quanto cada funcionário deve receber de bônus, com a frase no seguinte formato:

“Funcionário <Código> Receberá R$<ValorDoBonus>,00 de Bônus.” 

```java
public class BonusFuncionarios {
    public static void main(String[] args) {
        int codigo = 700; // Código inicial
        int totalFuncionarios = 60;

        for (int i = 0; i < totalFuncionarios; i++) {
            int bonus = (codigo % 2 == 0) ? codigo * 4 : 0; // Calcula bônus apenas 
            //para códigos pares
            System.out.println("Funcionário " + codigo + " Receberá R$" + bonus + ",00 de Bônus.");
            codigo -= 7; // Decrementa o código em 7
        }
    }
}

```

**Explicação:**

Verifica se o código é par (codigo % 2 == 0):
Se for par, o bônus é codigo * 4.
Se for ímpar, o bônus é 0.
Imprime a frase no formato correto.
Decrementa o código em 7 para seguir a sequência decrescente.

# **Corrigido em aula:**

```jsx
import java.util.Scanner;

public class calculadora {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        int contador = 0;
        for (double cod = 700;contador<60;cod -= 7){
            contador +=1;
            System.out.println(cod);
            if (cod%2==0) {
                System.out.printf("Bônus: R$%.2f\n",(cod+4));
            }
            else System.out.printf("Bônus: R$%.2f\n",(cod+4));
        }

    }
}
