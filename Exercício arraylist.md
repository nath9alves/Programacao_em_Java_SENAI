# Exercício das frutas

**Exercício:
Crie um programa em Java que:**

**Crie uma ArrayList para armazenar nomes de frutas.
Adicione pelo menos 5 frutas à lista.
Exiba todas as frutas da lista.
Permita que o usuário remova uma fruta pelo nome.
Exiba a lista atualizada após a remoção.**

```java
import java.util.ArrayList; // Importa a classe ArrayList para usar listas dinâmicas
import java.util.Scanner; // Importa a classe Scanner para ler a entrada do usuário

public class Aula { // Declaração da classe principal chamada "Aula"
    public static void main(String[] args) { // Método principal que inicia a execução do programa
        Scanner sc = new Scanner(System.in); // Criação do objeto Scanner para capturar a entrada do usuário

        // Criando uma lista dinâmica do tipo String chamada listaFrutas
        ArrayList<String> listaFrutas = new ArrayList<>(); 

        System.out.println("Informe quantas frutas deseja adicionar: "); // Exibe uma mensagem no console
        int quantidade = sc.nextInt(); // Lê um número inteiro do usuário (quantidade de frutas a serem adicionadas)
        sc.nextLine(); // Consome a quebra de linha pendente após o nextInt()

        // Loop para adicionar frutas à lista, de acordo com a quantidade informada pelo usuário
        for (int i = 0; i < quantidade; i++) { 
            System.out.println("Informe o nome da fruta para a lista da feira: "); // Mensagem para o usuário
            String fruta = sc.nextLine(); // Lê o nome da fruta digitada pelo usuário
            listaFrutas.add(fruta); // Adiciona a fruta à lista de frutas
        }

        // Exibir a lista inicial de frutas
        System.out.println("\nLista de frutas:"); // "\n" pula uma linha antes da mensagem
        for (String fruta : listaFrutas) { // Loop "for-each" que percorre cada fruta na lista
            System.out.println("- " + fruta); // Exibe a fruta com um marcador "-"
        }

        // Loop para remover frutas, se o usuário desejar
        while (true) { // Loop infinito que só será interrompido se o usuário responder "não"
            System.out.println("\nDeseja remover alguma fruta? (sim ou não)"); // Pergunta ao usuário se deseja remover frutas
            String resposta = sc.nextLine(); // Lê a resposta do usuário

            if (resposta.equalsIgnoreCase("sim")) { // Verifica se a resposta do usuário é "sim" (ignora maiúsculas/minúsculas)
                System.out.println("Digite o nome da fruta para removê-la: "); // Solicita o nome da fruta a ser removida
                String removerFruta = sc.nextLine(); // Lê o nome da fruta digitada pelo usuário

                if (listaFrutas.contains(removerFruta)) { // Verifica se a fruta está na lista
                    listaFrutas.remove(removerFruta); // Remove a fruta da lista
                    System.out.println("Fruta removida."); // Mensagem confirmando a remoção
                } else { // Se a fruta não estiver na lista
                    System.out.println("A fruta não está na lista :("); // Mensagem de erro
                }

                // Exibir lista atualizada
                System.out.println("\nLista atualizada de frutas:"); // "\n" pula uma linha antes da mensagem
                for (String fruta : listaFrutas) { // Percorre a lista atualizada
                    System.out.println("- " + fruta); // Exibe cada fruta restante na lista
                }
            } 
            else if (resposta.equalsIgnoreCase("não")) { // Se o usuário responder "não", encerra o loop
                break; // Sai do loop "while" e continua a execução do código após ele
            } 
            else { // Se o usuário digitar algo diferente de "sim" ou "não"
                System.out.println("Resposta inválida! Digite 'sim' ou 'não'."); // Mensagem de erro
            }
        }

        // Exibir a lista final após remoções
        System.out.println("\nLista final das frutas: " + listaFrutas); // Exibe a lista completa no formato [fruta1, fruta2, ...]

        sc.close(); // Fecha o Scanner para liberar recursos
    }
}

```

### **Explicação dos principais elementos do código:**

📌

**`import java.util.ArrayList;`**

→ Importa a classe

```
ArrayList
```

para criar listas dinâmicas.

📌

**`import java.util.Scanner;`**

→ Importa a classe

```
Scanner
```

para receber entrada do usuário.

📌

**`public class Aula {}`**

→ Declara a classe principal chamada

```
Aula
```

.

📌

**`public static void main(String[] args) {}`**

→ Método principal que executa o programa.

📌

**`Scanner sc = new Scanner(System.in);`**

→ Cria um Scanner para ler dados do teclado.

📌

**`ArrayList<String> listaFrutas = new ArrayList<>();`**

→ Cria uma lista dinâmica para armazenar frutas.

📌

**`for (int i = 0; i < quantidade; i++) {}`**

→ Laço

```
for
```

para adicionar frutas à lista.

📌

**`while (true) {}`**

→ Loop infinito que só para quando o usuário digita "não".

📌

**`listaFrutas.add(fruta);`**

→ Adiciona uma fruta à lista.

📌

**`listaFrutas.remove(removerFruta);`**

→ Remove uma fruta da lista.

📌

**`listaFrutas.contains(removerFruta);`**

→ Verifica se a fruta existe na lista antes de remover.

📌

**`break;`**

→ Sai do loop

```
while
```

.

📌

**`sc.close();`**

→ Fecha o Scanner para evitar consumo desnecessário de memória.