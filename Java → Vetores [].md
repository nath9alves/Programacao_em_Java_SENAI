# Java → Vetores []

O que são vetores em Java?
Um **vetor** (ou array) é uma estrutura que armazena vários valores do mesmo tipo em uma única variável.

• Imagine um armário com gavetas numeradas. Cada gaveta pode guardar um valor, e usamos um número (índice) para acessar cada posição.

```java
// Exemplo de um vetor em Java:

int[] numeros = {10, 20, 30, 40, 50};
```

Aqui temos um **vetor de inteiros** com **5 posições**.

| Índice | Valor |
| --- | --- |
| 0 | 10 |
| 1 | 20 |
| 2 | 30 |
| 3 | 40 |
| 4 | 50 |

### **Como acessar um valor do vetor?**

Podemos acessar os valores pelo **índice**, que começa do `0`:

```java
System.out.println(numeros[0]); // Mostra 10
System.out.println(numeros[3]); // Mostra 40
```

**Como criar um vetor vazio e preencher depois?**

```java
int[] valores = new int[3]; // Vetor com 3 posições
valores[0] = 5;
valores[1] = 10;
valores[2] = 15;
```

### **Percorrendo um vetor com `for`**

```java
for (int i = 0; i < numeros.length; i++) {
    System.out.println(numeros[i]); // Exibe todos os valores
}
```

[Exercício 3](Java%20%E2%86%92%20Vetores%20%5B%5D%20199b8871e1d980e7878ffa4dc4c89d0f/Exerci%CC%81cio%203%20199b8871e1d9802cb44be8f67bb6c36f.md)

[Exercício 1](Java%20%E2%86%92%20Vetores%20%5B%5D%20199b8871e1d980e7878ffa4dc4c89d0f/Exerci%CC%81cio%201%20199b8871e1d9804599feef45f9a2948f.md)