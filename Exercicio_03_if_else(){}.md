//3. Crie um programa que decida se um vendedor irá receber um bônus. Para que o vendedor receba o bônus, é necessário
// que tanto ele como a sua empresa tenham batido suas respectivas metas e, caso ele consiga dobrar a meta, ele recebe
// 20% de bônus ao invés dos 10% padrão.
// --> A meta de vendas da empresa é de R$ 200.000,00, e a meta de vendas do funcionário.
// é de R$ 15.000,00.


// 1º Forma:


import java.util.Scanner;

public class geral{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        double metaEmpresa = 200000.00;
        
        System.out.println("Informe a meta de vendas do vendedor: ");
        double metaVendedor = sc.nextDouble();

        System.out.println("Informe o total de vendas do vendedor: ");
        double vendasVendedor = sc.nextDouble();

        System.out.println("Informe o total de vendas da empresa: ");
        double vendasEmpresa = sc.nextDouble();

        boolean bateuMetaVendedor = vendasVendedor >= metaVendedor;
        boolean bateuMetaEmpresa = vendasEmpresa >= metaEmpresa;

        // Verifica se o vendedor dobrou sua meta
        boolean dobrouMetaVendedor = vendasVendedor >= 2 * metaVendedor;

        // Determina o bônus
        double bonus = 0;
        
        if (bateuMetaVendedor && bateuMetaEmpresa) {
            // Se o vendedor e a empresa bateram as metas, verifica o bônus
            if (dobrouMetaVendedor) {
                bonus = vendasVendedor * 0.20; // 20% se dobrou a meta
                System.out.println("Vendedor dobrou a meta! Bônus de 20%: R$ " + bonus);
            } else {
                bonus = vendasVendedor * 0.10; // 10% se não dobrou a meta
                System.out.println("Vendedor bateu a meta! Bônus de 10%: R$ " + bonus);
            }
        } else {
            System.out.println("Vendedor ou empresa não bateram as metas. Sem bônus.");
        }

        System.out.println("Fim do programa.");
    }
}


//---------------------------------------------------------------------------------


// 2º Forma: 



import java.util.Scanner;

public class geral {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        double meta, venda1, venda2;

        // Solicita as vendas
        System.out.println("Vendedor, informe o valor total de vendas desse mês: ");
        venda1 = sc.nextDouble();

        System.out.println("Informe o valor total de vendas da empresa: ");
        venda2 = sc.nextDouble();

        // Soma as vendas do vendedor com as da empresa
        meta = venda1 + venda2;

        // Exibe o total das vendas
        System.out.println("O total das vendas do vendedor + a empresa é: " + meta);

        // Verifica se o vendedor bateu a meta
        if (venda1 < 15000.00) {
            // Caso o vendedor não tenha batido a meta
            System.out.println("Vendedor não bateu a meta! O bônus à receber será de 10% do valor.");
        } else {
            // Caso o vendedor tenha batido a meta
            System.out.println("Vendedor bateu a meta! O bônus à receber será de 20%.");
        }

        // Finaliza o programa
        System.out.println("Fim do programa.");
    }
}
