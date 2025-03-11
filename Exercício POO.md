```java

/*1- `Crie 10 alunos (nome, nota b1-b4;calcular a media).`
*Extra hard:*`saber a nota minima, maxima; caso a primeira nota seja inferior a última nota, deve sinalizar declínio`*/


public class Aluno {
    String nome;
    String idade;
    double[] nota = new double[4]; // Mudado de 10 para 4, pois são 4 notas (B1, B2, B3, B4)

    // Construtor

    public Aluno(String nome, String idade, double[] nota) {
        this.nome = nome;
        this.idade = idade;
        this.nota = nota;
    }

    // média
    
    public double calcularMedia() {
        double soma = 0;
        for (double n : nota) {
            soma += n;
        }
        return soma / nota.length;
    }

    // Método para encontrar a nota mínima
    
    public double notaMinima() {
        double min = nota[0];
        for (double n : nota) {
            if (n < min) {
                min = n;
            }
        }
        return min;
    }

    // Método para encontrar a nota máxima
    
    public double notaMaxima() {
        double max = nota[0];
        for (double n : nota) {
            if (n > max) {
                max = n;
            }
        }
        return max;
    }

    // Verificando se houve declínio
    
    public boolean Declinio() {
        return nota[0] < nota[3];  // comparando a primeira e a última nota
    }

    // Método para imprimir as informações do aluno

    public void Informacoes() {
        System.out.println("Aluno: " + nome);
        System.out.println("Idade: " + idade);
        System.out.println("Notas: B1: " + nota[0] + ", B2: " + nota[1] + ", B3: " + nota[2] + ", B4: " + nota[3]);
        System.out.println("Média: " + calcularMedia());
        System.out.println("Nota mínima: " + notaMinima());
        System.out.println("Nota máxima: " + notaMaxima());
        System.out.println(Declinio() ? "Houve Declínio!" : "Sem Declínio!");
        System.out.println("--------------------------------------------------");
    }

    public static void main(String[] args) {
                                                  // Criando alunos
        Aluno aluno1 = new Aluno("Nathan", "15", new double[]{7.5, 8.0, 6.5, 7.0});
        Aluno aluno2 = new Aluno("Clarinha", "16", new double[]{9.0, 8.5, 8.0, 7.5});
        Aluno aluno3 = new Aluno("Pedro", "14", new double[]{6.0, 7.0, 6.5, 6.8});
        Aluno aluno4 = new Aluno("Ana", "17", new double[]{8.0, 7.5, 8.5, 9.0});
        Aluno aluno5 = new Aluno("Carlos", "16", new double[]{7.2, 6.9, 7.0, 6.5});
        Aluno aluno6 = new Aluno("Julia", "15", new double[]{5.5, 6.0, 5.8, 6.3});
        Aluno aluno7 = new Aluno("Lucas", "14", new double[]{9.5, 9.0, 9.2, 8.7});
        Aluno aluno8 = new Aluno("Nathalia", "16", new double[]{6.8, 7.1, 7.0, 6.9});
        Aluno aluno9 = new Aluno("Felipe", "18", new double[]{7.0, 7.5, 8.0, 7.8});
        Aluno aluno10 = new Aluno("Sofia", "17", new double[]{6.2, 6.5, 6.8, 7.0});


        //informações dos alunos

        aluno1.Informacoes();
        aluno2.Informacoes();
        aluno3.Informacoes();
        aluno4.Informacoes();
        aluno5.Informacoes();
        aluno6.Informacoes();
        aluno7.Informacoes();
        aluno8.Informacoes();
        aluno9.Informacoes();
        aluno10.Informacoes();
    }
}

