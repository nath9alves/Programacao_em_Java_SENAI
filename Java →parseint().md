# Java →parseint()

**O método `parseInt()` em Java é usado para converter uma `String` em um número inteiro (`int`). Ele faz parte da classe `Integer` e pode ser utilizado da seguinte forma:**

```java
int numero = Integer.parseInt("123");
```

Exemplo completo:

```java
public class ExemploParseInt {
    public static void main(String[] args) {
        String numeroTexto = "50";
        int numero = Integer.parseInt(numeroTexto);
        System.out.println("O número é: " + numero);
    }
}

Exemplos:

```java
int numero = Integer.parseInt("abc"); // Isso causará um erro!
```


```java
int numeroBinario = Integer.parseInt("1010", 2); // Converte "1010" de binário para decimal (resultado: 10)
```

```java
import java.util.Scanner;

public class aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double i = 1111.48;
        int j = (int) i;
        System.out.println(j);

    }
}
