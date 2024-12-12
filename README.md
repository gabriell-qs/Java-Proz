# Java-Proz
Exercícios realizados durante a disciplina 'Desenvolvimento de Aplicações', ministrada no curso de _Desenvolvimento de Sistemas_ da Escola Proz

<hr>

### **Variáveis + Inputs e Outputs + Operadores + Métodos em Strings**

**Q1.** Crie um programa cujo objetivo é inserir seus dados pessoais (nome, idade, gênero e cidade) e armazenar em cada variável determinada e depois exibidos na tela.
```

```
**Q2.** Dado o cálculo 12 x 3 + 4 - 8 / 2 % 3, qual o resultado segundo a precedência de operadores?
```

```
**Q3.** Crie um programa que utilize os métodos de Strings, onde o usuário envia uma frase e o programa exibe as informações dessa frase (tamanho, letra maiúscula, letra minúscula, substring e index).
```

```
**Q1.** Explique como criar um diretório para projetos Java e quais são as Convenções para sua criação. Envie os prints do passo a passo.
```

```
**Q2.** Explique o que é e dê um exemplo de uma Classe em Java e quais são as Convenções para sua declaração.
```

```
**Q3.** Explique o que é e dê um exemplo de um Método em Java e quais são as Convenções para sua declaração.
```

```
**Q4.** Quais são as Convenções para a declaração de uma variável em Java?
```

```
**Q5.** Envie um programa com a classe "Variáveis" que imprima 4 variáveis:
* Uma variável do tipo Texto
* Uma variável do tipo Número Inteiro
* Uma variável do tipo Número Decimal (ou ponto flutuante)
* Uma variável do tipo Lógica
```

```
**Q6.** Para cada Operação abaixo, crie um programa que leia dois valores enviados pelo usuário, faça a operação indicada e retorne o valor final.
* Soma
* Subtração
* Multiplicação
* Divisão
* Módulo
* Concatenação
```

```
**Q7.** Crie um programa que utilize os métodos de Strings, onde o usuário envia uma frase e o programa exiba as informações dessa frase (tamanho, letra maiúscula, letra minúscula, substring e index).
```

```
**Q8.** Crie um programa que utilize os métodos de Matemática, onde o usuário envia uma número decimal x e o programa exiba o valor absoluto de x e o quadrado  de x.
```

```
**Q9.** Crie um programa que retorne um número aleatório.
```

```
**Q10.** Crie um programa com operadores lógicos e relacionais.
```

```

### **Controle de Fluxo - Condicionais + Laços de Repetição**

**Q1.** Desenvolva um programa utilizando uma condicional simples.
```

```
**Q2.** Desenvolva um programa qualquer utilizando a condicional composta.
```

```
**Q3.** Desenvolva um programa qualquer utilizando a condicional ternária.
```

```
**Q4.** Desenvolva um programa que pede para o usuário digitar o dia da semana. Se for sábado ou domingo, deve aparecer a mensagem "descanso", senão, deve aparecer a mensagem "estudar".
```

```
**Q5.** Desenvolva um programa onde o usuário informa um número de 1 a 12 e retorna o mês correspondente.
```

```
**Q6.** Desenvolva um programa que pede as notas 1, 2 e 3 com pesos 2, 3 e 5, respectivamente, do aluno e faça o cálculo da média. Dependendo da nota, o programa retorna a seguinte mensagem:
* se a media for entre 0.0 e 4.9: reprovado
* se a media for entre 5.0 e 7.9: em recuperação
* se a media for entre 8.0 e 10.0: aprovado
```

```
**Q7.** Crie um laço de repetição com que exiba os com os números de 1 até 10 em ordem crescente e depois em ordem decrescente.
```

```
**Q8.** Crie um laço de repetição que exiba os com os números pares de 10 até 50 em ordem crescente e depois em ordem decrescente.
```

```
**Q9.** Utilizando um laço de repetição, desenvolva um programa que exiba a tabuada de 1 a 10. Para isso, peça para o usuário escolher um número de 1 a 10. Se o usuário digitar um valor fora desse intervalo, deve aparecer a seguinte mensagem de erro: “Digite um valor entre 1 e 10.” A tela esperada deve conter os valores da tabuada para o número digitado pelo usuário.
```

```

### **Vetores e Matrizes**

**Q1.** Crie um programa que leia um vetor de números inteiros e exiba a soma de todos os elementos.
```

```
**Q2.** Faça um programa que leia um vetor de números inteiros e exiba o maior elemento presente no vetor.
```

```
**Q3.** Faça um programa que leia um vetor de números inteiros e exiba a média dos elementos.
```

```
**Q4.** Crie um programa que leia um vetor de números inteiros e verifique se todos os elementos são pares.
```

```
**Q5.** Faça um programa que leia duas matrizes 2x2 e exiba a soma das duas matrizes.
```

```

### **Projetos POO - Programação Orientada a Objetos**

:brain: _Calculadora:_ Crie uma calculadora simples que realiza operações aritméticas básicas (adição, subtração, multiplicação e divisão).
```
import java.util.Scanner;

public class CXalculadoraBase {

    public static void main(String[] args) {
        
    

    Scanner vdd = new Scanner(System.in);

    System.out.println("digite o  primeiro numero");
    double num1 = vdd.nextDouble();

    System.out.println("didgite o segundo numero");
    double num2 = vdd.nextDouble();

    double resultado = 0;
    boolean operacaoValida = true;


    System.out.println("escolha uma operaçao");
    int  operacoes = vdd.nextInt();
   

    switch(operacoes){
    case 1 :
    resultado = num1+num2;
    break;
    case 2 :
    resultado = num1-num2;
    break;
    case 3 :
    resultado = num1*num2;
    break;
    case 4 :
    if(num2 !=0 ){
    resultado = num1/num2;}
    else{System.out.println("erro divisao por zero");
operacaoValida= false;}
    break;
default:System.out.println("operaçao invalida");


}
if (operacaoValida)
System.out.println("oresulatado da opercao "+ operacoes+ " e "+ resultado );
vdd.close();
    }}
```
:brain: _Conversor de unidades:_ Desenvolva um programa que converta unidades de medida como temperatura (Celsius para Fahrenheit e vice-versa) e distância (metros para quilômetros e vice-versa).
```
import java.util.Scanner;

public class Conversor {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int escolha;

        do {
            System.out.println("Escolha uma conversão:");
            System.out.println("1. Celsius para Fahrenheit");
            System.out.println("2. Fahrenheit para Celsius");
            System.out.println("3. Metros para Quilômetros");
            System.out.println("4. Quilômetros para Metros");
            System.out.println("0. Sair");
            escolha = scanner.nextInt();

            switch (escolha) {
                case 1:
                    System.out.print("Digite a temperatura em Celsius: ");
                    double celsius = scanner.nextDouble();
                    double fahrenheit = celsiusParaFahrenheit(celsius);
                    System.out.println(celsius + "°C é igual a " + fahrenheit + "°F");
                    break;
                case 2:
                    System.out.print("Digite a temperatura em Fahrenheit: ");
                    fahrenheit = scanner.nextDouble();
                    celsius = fahrenheitParaCelsius(fahrenheit);
                    System.out.println(fahrenheit + "°F é igual a " + celsius + "°C");
                    break;
                case 3:
                    System.out.print("Digite a distância em Metros: ");
                    double metros = scanner.nextDouble();
                    double quilometros = metrosParaQuilometros(metros);
                    System.out.println(metros + " metros é igual a " + quilometros + " quilômetros");
                    break;
                case 4:
                    System.out.print("Digite a distância em Quilômetros: ");
                    quilometros = scanner.nextDouble();
                    metros = quilometrosParaMetros(quilometros);
                    System.out.println(quilometros + " quilômetros é igual a " + metros + " metros");
                    break;
                case 0:
                    System.out.println("Saindo...");
                    break;
                default:
                    System.out.println("Opção inválida! Tente novamente.");
            }
        } while (escolha != 0);

        scanner.close();
    }

    public static double celsiusParaFahrenheit(double celsius) {
        return (celsius * 9/5) + 32;
    }

    public static double fahrenheitParaCelsius(double fahrenheit) {
        return (fahrenheit - 32) * 5/9;
    }

    public static double metrosParaQuilometros(double metros) {
        return metros / 1000;
    }

    public static double quilometrosParaMetros(double quilometros) {
        return quilometros * 1000;
    }
}

```
:brain: _Jogo de adivinhação:_ Crie um jogo onde o computador escolhe um número aleatório entre 1 e 100 e o usuário tenta adivinhá-lo. O programa deve fornecer dicas como "é maior" ou "é menor".
```
import java.util.Random;
import java.util.Scanner;

public class Jogo {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Random random = new Random();
        
        int numeroAleatorio = random.nextInt(100) + 1; // Número entre 1 e 100
        int tentativas = 0;
        int palpite = 0;

        System.out.println("Bem-vindo ao Jogo de Adivinhação!");
        System.out.println("Tente adivinhar o número entre 1 e 100.");

        while (palpite != numeroAleatorio) {
            System.out.print("Digite seu palpite: ");
            palpite = scanner.nextInt();
            tentativas++;

            if (palpite < numeroAleatorio) {
                System.out.println("É maior! Tente novamente.");
            } else if (palpite > numeroAleatorio) {
                System.out.println("É menor! Tente novamente.");
            } else {
                System.out.println("Parabéns! Você adivinhou o número em " + tentativas + " tentativas.");
            }
        }

        scanner.close();
    }
}

```
:brain: _Gerador de senhas:_ Crie um programa onde o usuário informa a quantidade de caracteres e o programa gere uma senha aleatória que possua letras maiúsculas, letras minúsculas, números e caracteres especiais.
```
import java.util.Random;
import java.util.Scanner;

public class Senha{
    public static void main(String[] args) {

        Scanner vds = new Scanner(System.in);
        System.out.println("digite o  tamanho da senha ");
        int tamanho = vds.nextInt();

        String caracteres ="ABCDEFGHIJKLMLOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyzéáç0123456789!?.,@#$%&*-_+=<>/^~`";

        StringBuilder senha = new StringBuilder();
        Random random = new Random();

        for (int i =0;i < tamanho;i++){int indice = random.nextInt(caracteres.length());
        
        senha.append(caracteres.charAt(indice));}

        System.out.println("senha gerada:" + senha.toString());

        vds.close();


        
    }


}
    

```
:brain: _SmartTv:_ Crie um sistema de uma SmartTv, onde o usuário pode realizar as seguintes tarefas:
* Ligar e Desligar a Tv
* Aumentar volume
* Diminuir volume
* Aumentar canal
* Diminuir canal
* Mudar Canal
```

```

