# Exercício 6

//**6- Crie uma função multiplicação que retorne o resultado da multiplicação de dois números double.**

```java
public class aula {
    public static void main(String[] args) {
        double n1, n2;
        n1 = 10.5;
        n2 = 20;
        double resultado = multiplicacao(n1, n2);
        System.out.println("Resultado é: "+resultado);
    }
    public static double multiplicacao(double n1, double n2){
        return n1*n2;
        
        // O código não pode ter instruções após o return. O System.out.println 
        // após o return nunca será executado e causará um erro de compilação.

    }
}
