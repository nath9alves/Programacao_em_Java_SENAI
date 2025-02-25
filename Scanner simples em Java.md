# Scanner simples em Java

![ezgif-1fc3fc54cbf9d.gif](Scanner%20simples%20em%20Java%20192b8871e1d980c899b0fbba85d35daa/ezgif-1fc3fc54cbf9d.gif)

# Scanner simples em Java

- Código
    
    
    ```java
    import java.util.Scanner;  //<-- Importando o scanner
    
    public class Primeiro_Codigo {
        public static void main(String[] args) {
            Scanner leia = new Scanner(System.in);  //<-- Declarando o Scanner como "leia"
    
              String nome; int idade;                 //<-- declarando o nome e a "idade" como int
    
            System.out.println("Informe seu nome:");   //<-- Java pergunta p/ o usuário juntamente com a mensagem de solicitação.
    
               nome = leia.next();                    // <-- a string nome resulta no scanner leia
    
            System.out.println("Agora informe sua idade:"); // <-- Java pergunta p/ o usuário juntamente com a mensagem de solicitação.
    
               idade = leia.nextInt();                 //<-- a string idade resulta no scanner leia
    
            System.out.println("Bom dia "+nome+", parabéns pelos seus "+idade+" anos.");  //<-- Java apresenta a mensagem final ao usuário
    
        }
    }
    ```
    
    [https://www.notion.so](https://www.notion.so)