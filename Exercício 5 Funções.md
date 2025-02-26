# Exercício 5

//**5- Crie uma função que, a partir de um nome fornecido como argumento, retorne a mensagem: “Feliz aniversário <nome>”.**

```java
public class aula {
    public static void main(String[] args) {
        String nome = mensagem("Nathalia");
        System.out.println(nome);
    }
    public static String mensagem(String nome){
        return "Feliz Aniversário, " + nome + "!";
    }
}
