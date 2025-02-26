# Java → switch(){case } default e break;

**Este código exibe o dia da semana com base em um número digitado pelo usuário:**

• O usuário digita um número de 1 a 7.
• O **switch-case** verifica qual número foi digitado.
• Se o número for 1, imprime "Domingo", se for 2, imprime "Segunda-feira" e assim por diante.
• Se o número não estiver entre 1 e 7, o default exibe "Número inválido!".
• Cada case finaliza com break para evitar que o código continue executando os próximos casos.
•  O switch-case é ideal quando há múltiplas opções fixas, como menus, dias da semana e categorias.

```java
import java.util.Scanner;

public class DiasSemana {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite um número de 1 a 7: ");
        int dia = scanner.nextInt();

        switch (dia) {
            case 1:
                System.out.println("Domingo");
                break;
            case 2:
                System.out.println("Segunda-feira");
                break;
            case 3:
                System.out.println("Terça-feira");
                break;
            case 4:
                System.out.println("Quarta-feira");
                break;
            case 5:
                System.out.println("Quinta-feira");
                break;
            case 6:
                System.out.println("Sexta-feira");
                break;
            case 7:
                System.out.println("Sábado");
                break;
            default:
                System.out.println("Número inválido!");
        }

        scanner.close();
    }
}

```

**Explicação:**

• O **break** é usado dentro do switch-case para interromper a execução do bloco após encontrar um case correspondente.

• Sem o **break**, o programa continuaria executando os próximos case, mesmo que já tenha encontrado uma correspondência.

• O **default** é um caso padrão que será executado se nenhum case corresponder ao valor testado.