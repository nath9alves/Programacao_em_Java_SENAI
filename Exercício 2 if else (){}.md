# Exercício 2

```java

 // 2. Pergunte o salário de um funcionário qualquer e verifique se ele paga imposto 
 // de renda.
 
 
import java.util.Scanner;

public class geral {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        double salario;

        System.out.print("Informe seu salário para análise: ");
        salario = sc.nextDouble();

        if (salario <= 2259.20){
            System.out.print(" Não precisa declarar Imposto de Renda.");
        }
         if (salario >= 2259.21 && salario <= 2826.65){
            System.out.print("Precisa pagar Imposto de Renda! Sua aliquota é 7,5% e Parcela a deduzir do IR é R$ 169,44.");
        }
         if (salario >= 2826.66 && salario <= 3751.05){
            System.out.print("Precisa pagar Imposto de Renda! Sua aliquota é 15% e Parcela a deduzir do IR é R$ 381,44.");
        }
         if (salario >= 3751.06 && salario <= 4664.68){
             System.out.print("Precisa pagar Imposto de Renda! Sua aliquota é 22% e Parcela a deduzir do IR é R$ 662,77.");
         }
         if (salario >= 4664.69){
             System.out.print("Precisa pagar Imposto de Renda! Sua aliquota é 27,5% e Parcela a deduzir do IR é R$ 896,00.");
         }
         System.out.println("Fim do Programa.");
    }
}
       
```

[Exercício 3](Exerci%CC%81cio%202%20199b8871e1d980d2853ee0e82a298bd4/Exerci%CC%81cio%203%20199b8871e1d980f0a479da739ca28e49.md)