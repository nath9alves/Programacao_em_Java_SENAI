```java
// Exemplo:

public class aula{
    public static int fatorial(int n){
        if (n == 0 || n == 1){
            return 1;
        }
        return n * fatorial (n-1);
    }
    public static void main (String[] args){
        int numero = 5;
        System.out.println("fatorial de " + numero + " é: " + fatorial(numero));
    }
}

