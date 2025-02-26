# Java → Funções

**O que são funções?**
Em programação, funções são blocos de código que realizam uma tarefa específica. Elas permitem reutilizar o código em diferentes partes de um programa, tornando-o mais organizado, modular e fácil de manter.

**Por que usar funções?**
Reutilização de código: Evita escrever o mesmo código várias vezes.
Organização: Divide o programa em partes menores e mais fáceis de entender.
Manutenção: Alterar uma função reflete em todos os lugares onde ela é usada.
Legibilidade: O código fica mais limpo e fácil de ler.

**Como criar uma função em Java?**
A criação de funções segue alguns passos básicos:
Definir o tipo de retorno:
Pode retornar um valor (como int, String, etc.).
Ou não retornar nada (usando void).
Nome da função:
Escolha um nome que seja descritivo e claro.
Parâmetros (opcional):
Se necessário, a função pode receber dados como entrada.
Corpo da função:
Aqui vai o código com a lógica que você quer executar.

```java
public class aula {
    // Função que retorna a soma de dois números
    public static int somar(int a, int b) {
        return a + b; // Retorna o resultado
    }

    // Função que exibe uma mensagem (sem retorno)
    public static void mostrarMensagem() {
        System.out.println("Olá, mundo!");
    }

    public static void main(String[] args) {
        // Usa a função somar
        int resultado = somar(5, 3); 
        System.out.println("Soma: " + resultado);

        // Usa a função mostrarMensagem
        mostrarMensagem(); 
    }
}
```

[Exercício 1](Java%20%E2%86%92%20Func%CC%A7o%CC%83es%201a4b8871e1d9804290eecc95f08a05f9/Exerci%CC%81cio%201%201a4b8871e1d9801794a3d98dcc5c6083.md)