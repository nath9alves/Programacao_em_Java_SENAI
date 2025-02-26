# Java → contains()

**O que é contains() em Java?**
O método **contains()** é usado para verificar se uma String contém uma determinada sequência de caracteres.

Ele retorna:
✅ true → Se a String contém o valor procurado.
❌ false → Se o valor não está presente na String.

6. Faça um programa que retorne o servidor do email do usuário, vocês precisam avisar caso não tenha @ no endereço do email que o usuário deve digitar um e-mail válido.

**Exemplo simples:**

```java
String texto = "Olá, mundo!";

if (texto.contains("mundo")) {
    System.out.println("A palavra 'mundo' está presente!");
} else {
    System.out.println("A palavra 'mundo' não foi encontrada.");
}

```

Observação:

Essa linha extrai o servidor do e-mail, ou seja, tudo que vem depois do "@". Vamos entender parte por parte:

```java
String servidor = email.substring(email.indexOf("@") + 1);
```

Quebra da lógica
1️⃣ email.indexOf("@")

Procura a posição do caractere "@" dentro da string.
Exemplo: Se email = "[usuario@gmail.com](mailto:usuario@gmail.com)", o "@" está na posição 7.
2️⃣ email.indexOf("@") + 1

Adicionamos 1 para pegar o próximo caractere (evitando incluir o @).
Se "@" está na posição 7, pegamos a partir da posição 8, que seria "[gmail.com](http://gmail.com/)".
3️⃣ email.substring(email.indexOf("@") + 1)

O método substring(posição) retorna tudo a partir da posição informada.
Como pegamos a posição depois do "@", o resultado é o servidor do e-mail.