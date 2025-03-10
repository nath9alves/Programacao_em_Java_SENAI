```java

// Primeiro código java POO
// Exemplo: Parentesco de quatro pessoas
// Sem utilizar o for

public class Parentes {
    String parentesco;
    String idade;
    String nome;

    // Construtor correto da classe Parentes
    public Parentes(String parentesco, String idade, String nome) {
        this.parentesco = parentesco;
        this.idade = idade;
        this.nome = nome;
    }
}

// Classe principal separada

class Main {
    public static void main(String[] args) {

        Parentes parentes1 = new Parentes("Mãe ", "47 anos ", "Maria");
        Parentes parentes2 = new Parentes("Irmã ", "6 anos ", "Isabel");
        Parentes parentes3 = new Parentes("Tia ", "55 anos ", "Cícera");
        Parentes parentes4 = new Parentes("Prima ", "28 anos ", "Izamara");

        System.out.println("Parentes: " + parentes1.parentesco + ", Idade: " + parentes1.idade + ", Nome: " + parentes1.nome);
        System.out.println("Parentes: " + parentes2.parentesco + ", Idade: " + parentes2.idade + ", Nome: " + parentes2.nome);
        System.out.println("Parentes: " + parentes3.parentesco + ", Idade: " + parentes3.idade + ", Nome: " + parentes3.nome);
        System.out.println("Parentes: " + parentes4.parentesco + ", Idade: " + parentes4.idade + ", Nome: " + parentes4.nome);

    }
}
