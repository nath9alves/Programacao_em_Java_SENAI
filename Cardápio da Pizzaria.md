// Você é dono de uma pizzaria e gostaria de registrar 5 pizzas em um vetor que já contém 5 sabores, totalizando 10 sabores.
//Cada sabor deve ter um preço atrelado a ele (double).  Crie uma sequência aonde os 5 próximos sabores e valores devem
//ser cadastrados utilizando um for.  Ao final, printe todo os 10 sabores e preços das pizzas e o valor total a ser pago,
//informe o valor das parcelas caso parcele em 3x e o valor de pagamento no pix (5% de desconto).


```java

import java.util.Arrays;
import java.util.Scanner;
import java.util.ArrayList;

public class aula {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Sabores e preços já existentes
        String[] sabores_existentes = {"Calabresa", "Queijo", "Atum", "Costela", "Brócolis"};
        double[] precos_existentes = {35.0, 30.0, 40.0, 45.0, 38.0};

        // Lista para armazenar sabores e preços
        ArrayList<String> sabores = new ArrayList<>();
        ArrayList<Double> precos = new ArrayList<>();

        // Adicionando sabores e preços existentes
        sabores.addAll(Arrays.asList(sabores_existentes));
        for (double preco : precos_existentes) {
            precos.add(preco);
        }

        System.out.println("Os sabores do cardápio são: " + Arrays.toString(sabores_existentes));
        System.out.println("Informe cinco novos sabores e seus preços para completar o cardápio:\n");

        // Adicionando os novos sabores e preços
        for (int i = 0; i < 5; i++) {
            System.out.print("Informe o " + (i + 1) + "º novo sabor: ");
            String sabor_novo = sc.nextLine();
            sabores.add(sabor_novo);

            System.out.print("Informe o preço da pizza " + sabor_novo + ": R$ ");
            double preco_novo = sc.nextDouble();
            precos.add(preco_novo);
            sc.nextLine(); // Consumir a quebra de linha
        }

        // Exibindo todos os sabores e preços
        System.out.println("\nCardápio completo:");
        for (int i = 0; i < sabores.size(); i++) {
            System.out.printf("%d. %s - R$ %.2f\n", (i + 1), sabores.get(i), precos.get(i)); // .get(i) <- significa "pegar o elemento na posição i da lista sabores"
        }

        // Cálculo do valor total
        double valor_total = 0;
        for (double preco : precos) {
            valor_total += preco;
        }

        System.out.printf("\nValor total a ser pago: R$ %.2f\n", valor_total);

        // Parcelamento em 3x
        double valor_parcela = valor_total / 3;
        System.out.printf("Valor das parcelas em 3x: R$ %.2f\n", valor_parcela);

        // Pagamento no PIX com desconto de 5%
        double desconto = valor_total * 0.05;
        double valor_com_desconto = valor_total - desconto;
        System.out.printf("Valor de pagamento no Débito, Pix ou Dinheiro (5%% de desconto): R$ %.2f\n", valor_com_desconto);
        
    }
}
