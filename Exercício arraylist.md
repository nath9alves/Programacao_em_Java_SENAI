# Exercício das frutas

**Exercício:
Crie um programa em Java que:**

**Crie uma ArrayList para armazenar nomes de frutas.
Adicione pelo menos 5 frutas à lista.
Exiba todas as frutas da lista.
Permita que o usuário remova uma fruta pelo nome.
Exiba a lista atualizada após a remoção.**

```java
import java.util.ArrayList; 
import java.util.Scanner;

public class Aula { 
    public static void main(String[] args) { 
        Scanner sc = new Scanner(System.in); 

        ArrayList<String> listaFrutas = new ArrayList<>(); 

        System.out.println("Informe quantas frutas deseja adicionar: "); 
        int quantidade = sc.nextInt();
        sc.nextLine(); 

        for (int i = 0; i < quantidade; i++) { 
            System.out.println("Informe o nome da fruta para a lista da feira: "); 
            String fruta = sc.nextLine(); 
            listaFrutas.add(fruta); 
        }

        System.out.println("\nLista de frutas:"); // "\n" pula uma linha antes da mensagem
        for (String fruta : listaFrutas) { 
            System.out.println("- " + fruta); 
        }

        while (true) { 
            System.out.println("\nDeseja remover alguma fruta? (sim ou não)"); 
            String resposta = sc.nextLine(); // 

            if (resposta.equalsIgnoreCase("sim")) { 
                System.out.println("Digite o nome da fruta para removê-la: ");
                String removerFruta = sc.nextLine(); 

                if (listaFrutas.contains(removerFruta)) { 
                    listaFrutas.remove(removerFruta); 
                    System.out.println("Fruta removida."); 
                } else { // Se a fruta não estiver na lista
                    System.out.println("A fruta não está na lista :("); 
                }

                System.out.println("\nLista atualizada de frutas:"); // "\n" pula uma linha antes da mensagem
                for (String fruta : listaFrutas) { // Percorre a lista atualizada
                    System.out.println("- " + fruta); // Exibe cada fruta restante na lista
                }
            } 
            else if (resposta.equalsIgnoreCase("não")) { // Se o usuário responder "não", encerra o loop
                break; // Sai do loop "while" e continua a execução do código após ele
            } 
            else { 
                System.out.println("Resposta inválida! Digite 'sim' ou 'não'."); 
            }
        }

        System.out.println("\nLista final das frutas: " + listaFrutas); 

        sc.close(); // Fecha o Scanner para liberar recursos
    }
}



