# Encontra Divisores

## Visão Geral

Este programa Java solicita ao usuário que digite um número inteiro. Em seguida, ele encontra e imprime todos os divisores desse número, começando de 1 até o próprio número.

## Como Usar

Para executar este programa, você precisará ter o Java Development Kit (JDK) instalado em seu computador.

**Passos para executar o programa:**

1.  **Salve o código:** Salve o código Java fornecido em um arquivo chamado `Main.java` dentro de uma pasta chamada `principal`. A estrutura de pastas deve ser:
    ```
    seu_projeto/
    └── principal/
        └── Main.java
    ```

2.  **Compile o código:** Abra o terminal ou prompt de comando, navegue até a pasta raiz do seu projeto e execute o seguinte comando para compilar o código Java:
    ```bash
    javac principal/Main.java
    ```
    Isso irá gerar um arquivo chamado `Main.class` dentro da pasta `principal`.

3.  **Execute o programa:** No mesmo terminal ou prompt de comando, execute o programa com o comando:
    ```bash
    java principal.Main
    ```
    O programa solicitará que você digite um número no console.

## Explicação do Código

O código Java realiza as seguintes ações:

* **Importa `java.util.Scanner`:** Importa a classe `Scanner`, que é usada para obter entrada do usuário através do console.
* **Declaração da classe `Main`:** Define a classe principal do programa.
* **Método `main`:** O ponto de entrada da execução do programa.
* **Cria um objeto `Scanner`:**
    * `Scanner sc = new Scanner(System.in);`: Cria uma instância da classe `Scanner` chamada `sc`, que lê a entrada do sistema (o teclado, neste caso).
* **Lê a entrada do usuário:**
    * `int n = sc.nextInt();`: Lê o número inteiro que o usuário digitou no console e o armazena na variável `n`.
* **Loop `for`:** Um loop `for` é executado, começando de 1 e indo até o valor de `n` (inclusive).
    * **Verifica se `i` é um divisor de `n`:**
        * `if (n % i == 0)`: Dentro do loop, para cada número `i`, esta condição verifica se o resto da divisão de `n` por `i` é igual a 0. Se for, significa que `i` é um divisor de `n`.
    * **Imprime o divisor:**
        * `System.out.println(i);`: Se `i` for um divisor de `n`, este valor é impresso no console.
* **Fecha o objeto `Scanner`:**
    * `sc.close();`: Fecha o objeto `Scanner` para liberar os recursos do sistema. É uma boa prática fechar objetos `Scanner` após seu uso.

## Entrada do Usuário

O programa utiliza a classe `Scanner` para receber a entrada do usuário diretamente no console (linha de comando). Ao executar o programa, você precisará digitar um número inteiro e pressionar Enter. O programa então processará esse número para encontrar seus divisores.

## Requisitos

* Java Development Kit (JDK) instalado no sistema.

## Como Executar

1.  Certifique-se de ter o JDK instalado.
2.  Salve o código em `seu_projeto/principal/Main.java`.
3.  Abra o terminal e navegue até a pasta `seu_projeto`.
4.  Compile o código com: `javac principal/Main.java`
5.  Execute o programa com: `java principal.Main`

## Exemplo de Uso

1.  Após executar o programa, o terminal exibirá um cursor esperando pela sua entrada.
2.  Se você digitar `12` e pressionar Enter, a saída no console será:
    ```
    1
    2
    3
    4
    6
    12
    ```
    Estes são todos os divisores do número 12.

## Autor

gustavodees

gustavoemartins@gmail.com
