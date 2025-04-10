# Java-Proz
Exercícios realizados durante a disciplina 'Desenvolvimento de Aplicações', ministrada no curso de _Desenvolvimento de Sistemas_ da Escola Proz

<hr>

### **Variáveis + Inputs e Outputs + Operadores + Métodos em Strings**

**Q1.** Crie um programa cujo objetivo é inserir seus dados pessoais (nome, idade, gênero e cidade) e armazenar em cada variável determinada e depois exibidos na tela.
```var nome = ""
var idade = ""
var genero = ""
var cidade = ""


nome = prompt("digite seu nome: ")

document.write("<br>ola " + nome + " seja bem vindo! ")

idade = prompt("digite sua idade: ")

document.write("<br>voce tem " + idade + " anos! ")

genero = prompt("digite seu genero: ")

document.write("<br>voce é " + genero )

cidade = prompt("digite sua cidade: ")

document.write("<br>voce é de " + cidade  )


```
**Q2.** Dado o cálculo 12 x 3 + 4 - 8 / 2 % 3, qual o resultado segundo a precedência de operadores?
```var numero = (12 * 3) + 4 - (8 / 2) % 3

document.write("<br> o  resuitado de 12 * 3 + 4 - 8 / 2 % 3 é : " + numero )

```
**Q3.** Crie um programa que utilize os métodos de Strings, onde o usuário envia uma frase e o programa exibe as informações dessa frase (tamanho, letra maiúscula, letra minúscula, substring e index).
```var texto = ""
var letra = ""
var achar = texto.indexOf(letra)

texto = prompt("qual a frase?")
document.write("<br>a frase é :" + texto )
document.write("<br>o  tamanho é :" + texto.length )
document.write("<br>a frase cortado :" + texto.substring(0,9) )
document.write("<br>em forma maiuscula :" + texto.toUpperCase() )
document.write("<br>em forma mininuscula :" + texto.toLowerCase() )

letra = prompt("qual a letra que voce quer achar?")

if(achar){ 
    document.write("<br> a frase tem a " + letra + " na " + texto)

}else {
    document.write("<br> a "+ texto + " nao tem a letra " + letra)
}

```
**Q1.** Explique como criar um diretório para projetos Java e quais são as Convenções para sua criação. Envie os prints do passo a passo.
```
Escolha um local: Decida onde você quer criar seu diretório (por exemplo, na área de trabalho ou em uma pasta específica).

Crie o diretório:
No Windows: Clique com o botão direito, selecione "Novo" > "Pasta" e nomeie-a (ex.: MeuProjetoJava).
No macOS: Clique com o botão direito na área de trabalho ou na pasta desejada e selecione "Nova Pasta".
Estrutura recomendada: Siga as convenções de nomenclatura, como usar letras minúsculas e separar palavras com sublinhado ou hífen. A estrutura geralmente inclui:
src/ (para código fonte)
bin/ (para arquivos compilados)
lib/ (para bibliotecas externas)

```
**Q2.** Explique o que é e dê um exemplo de uma Classe em Java e quais são as Convenções para sua declaração.
```
Uma classe em Java é um modelo que define as propriedades (atributos) e comportamentos (métodos) de um objeto. Por exemplo, uma classe Carro pode ter atributos como cor e modelo, e métodos como acelerar() e frear().
public class Carro {
    // Atributos
    private String cor;
    private String modelo;

    // Construtor
    public Carro(String cor, String modelo) {
        this.cor = cor;
        this.modelo = modelo;
    }

    // Métodos
    public void acelerar() {
        System.out.println("O carro está acelerando.");
}
}
Convenções para Declaração:
Nome da Classe: Use a convenção CamelCase (ex.: NomeDaClasse).
Visibilidade: Normalmente, usa-se public para classes que precisam ser acessíveis de fora.
Atributos: Devem ser privados (private) para encapsulamento.
Métodos: Nomeie-os em camelCase, começando com letra minúscula

```
**Q3.** Explique o que é e dê um exemplo de um Método em Java e quais são as Convenções para sua declaração.
```
Um método em Java é um bloco de código que realiza uma tarefa específica. Ele pode aceitar parâmetros e retornar um valor. Métodos são usados para organizar o código, permitindo a reutilização e a modularização.
public class Calculadora {
    // Método que soma dois números e retorna o resultado
    public int somar(int a, int b) {
        return a + b;
 }
}
Convenções para Declaração de Métodos:
Nome do Método: Use a convenção camelCase, começando com letra minúscula (ex.: calcularSoma).
Tipo de Retorno: Declare o tipo de retorno antes do nome do método. Use void se o método não retornar nada.
Parâmetros: Declare o tipo e o nome dos parâmetros entre parênteses. Por exemplo, (int a, int b).
Visibilidade: Normalmente, usa-se public para métodos que precisam ser acessíveis de fora da classe.

```
**Q4.** Quais são as Convenções para a declaração de uma variável em Java?
```
Nome da Variável: Use camelCase, começando com letra minúscula (ex.: minhaVariavel).
Tipo: Declare o tipo da variável antes do nome (ex.: int idade;).
Inicialização: É uma boa prática inicializar variáveis no momento da declaração (ex.: String nome = "João";).
Visibilidade: Use modificadores de acesso (como private, public) conforme necessário, especialmente em atributos de classes.
Constantes: Para constantes, use letras maiúsculas e sublinhados (ex.: final int MAX_TAM = 100;).

```
**Q5.** Envie um programa com a classe "Variáveis" que imprima 4 variáveis:
* Uma variável do tipo Texto
* Uma variável do tipo Número Inteiro
* Uma variável do tipo Número Decimal (ou ponto flutuante)
* Uma variável do tipo Lógica
```
public class App {

    public static void main(String[] args) throws Exception {
        System.out.println("Hello, World!");

        String name = "gabriel";
        int num = 50;
        double numDois = 11.23;
        char sexo = 'M';
        boolean logica = true;

        System.out.println(name);
        System.out.println(num);
        System.out.println(numDois);
        System.out.println(sexo);
        System.out.println(logica);
   
    } 



    }
```
**Q6.** Para cada Operação abaixo, crie um programa que leia dois valores enviados pelo usuário, faça a operação indicada e retorne o valor final.
* Soma
* Subtração
* Multiplicação
* Divisão
* Módulo
* Concatenação
```
import java.util.Scanner;

public class ExeSeisvezes {
    
public static void main(String[] args) {
        
    Scanner entrada = new Scanner(System.in);
    
    int num5;
    int num6;
    int vezes;
    
    System.out.println("Digite o primeiro numero: ");
    num5 = entrada.nextInt();

    System.out.println("Digite o segundo numero: " );
    num6 = entrada.nextInt();

    vezes = num5 * num6;

    System.out.println("igual a " + vezes);
    
    }

}
import java.util.Scanner;


public class ExeSeisSoma {

   
    public static void main(String[] args) {
        
    Scanner entrada = new Scanner(System.in);
        
    int num1;
    int num2;
    int soma;
    
    System.out.println("Digite o primeiro numero: ");
    num1 = entrada.nextInt();

    System.out.println("Digite o segundo numero: " );
    num2 = entrada.nextInt();

    soma = num1 + num2;

    System.out.println("soma igual a " + soma);
    

    }

}
import java.util.Scanner;

public class ExeSeisMenos {
    public static void main(String[] args) {
        
        Scanner entrada = new Scanner(System.in);
        
        int num3;
        int num4;
        int menos;
        
        System.out.println("Digite o primeiro numero: ");
        num3 = entrada.nextInt();
    
        System.out.println("Digite o segundo numero: " );
        num4 = entrada.nextInt();
    
        menos = num3 - num4;
    
        System.out.println("igual a " + menos);
        
        }
    
}
import java.util.Scanner;

public class ExeSeisDividir {
    
public static void main(String[] args) {
        
    Scanner entrada = new Scanner(System.in);
    
    int num7;
    int num8;
    int dividir;
    
    System.out.println("Digite o primeiro numero: ");
    num7 = entrada.nextInt();

    System.out.println("Digite o segundo numero: " );
    num8 = entrada.nextInt();

    dividir = num7 / num8;

    System.out.println("igual a " + dividir);
    
    }

}
```
**Q7.** Crie um programa que utilize os métodos de Strings, onde o usuário envia uma frase e o programa exiba as informações dessa frase (tamanho, letra maiúscula, letra minúscula, substring e index).
```
import java.util.Scanner;

public class ExeSete {
    public static void main(String[] args) {

    Scanner scanner = new Scanner(System.in);

    System.out.println("Digite uma frase ");
    String frase = scanner.nextLine();

    System.out.println("Tamanho da frase " + frase.length());

    System.out.println("Frase em maiuscculas " + frase.toUpperCase());

    System.out.println("Frase em letra minusculas " + frase.toLowerCase());

    System.out.println("Digite uma palavra ou sequencia para encontra ");
    String subString = scanner.nextLine();

    int index = frase.indexOf(subString);
    if (index != -1) {System.out.println("A substring\"" + subString + "\" foi encontrada no indice:" + index);
    }else{
       System.out.println("A subtring\"" + subString + "\" nao foi encontrada" );
    }
    

    scanner.close();
    }
    
}
```
**Q8.** Crie um programa que utilize os métodos de Matemática, onde o usuário envia uma número decimal x e o programa exiba o valor absoluto de x e o quadrado  de x.
```
import java.util.Scanner;

public class ExeOito {
    public static void main(String[] args) {

    Scanner scanner = new Scanner(System.in);

    System.out.println("Digite um numero decimal: ");
    double x = scanner.nextDouble();

    double absoluto = Math.abs(x);
    System.out.println("O valor absoluto de " + x + " e " + absoluto);

    double quadrado = Math.pow(x,2);
    System.out.println("O quadrado de " + x + " e " + quadrado);

    scanner.close();
     

    }
    
}
```
**Q9.** Crie um programa que retorne um número aleatório.
```
import java.util.Random;

public class ExeNove {
     public static void main(String[] args) {
        
        Random random = new Random();

        int numeroAle = random.nextInt(101);

        System.out.println("Numero aleatorio gerado " +  numeroAle);
     }
    
}
```
**Q10.** Crie um programa com operadores lógicos e relacionais.
```
import java.util.Scanner;

public class ExeDez {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Digite o  primeiro numero: ");
        int num1 = scanner.nextInt();

        System.out.println("Digite o segundo numero: ");

        int num2 = scanner.nextInt();

        System.out.println("Operadores Realacionais: " );
        System.out.println(num1 +" e maior que "+ num2 + ":" + (num1>num2) );
        System.out.println(num1 +" e menor que "+ num2 + ":"  + (num1<num2) );
        System.out.println(num1 +" e igual que "+ num2 + ":" + (num1==num2) );
        System.out.println(num1 +" e diferente que "+ num2 + ":" + (num1!=num2) );
        
        System.out.println("\nOperadores Logicos");

        System.out.println("Ambos os numeros sao positivos:" + (num1> 0&&num2 > 0));
        System.out.println("Ambos dos numeros e positivos:" + (num1> 0||num2 > 0));
        System.out.println("Ambos dos numeros e positivos:" + !(num1> 0||num2 > 0));

        scanner.close();
    }

    
}
```

### **Controle de Fluxo - Condicionais + Laços de Repetição**

**Q1.** Desenvolva um programa utilizando uma condicional simples.
```
public class App {
    public static void main(String[] args) throws Exception {
        System.out.println("Hello, World!");

        int idade = 22;
        String cidade = "Sao Paulo";

        if (idade >= 18 && cidade.equals("Sao Paulo")) {
            System.out.println("Bem vindo a festa");
        }
        
    }
}
```
**Q2.** Desenvolva um programa qualquer utilizando a condicional composta.
```
public class Exe2 {

    public static void main(String[] args) {
        System.out.println("Hello, World!");

        int idade = 17;
        String cidade = "Sao Paulo";

        if (idade >= 18 && cidade.equals("Sao Paulo")) {
            System.out.println("Bem vindo a festa");
        }
        
        else 
            System.out.println("Voce n tem idade");

        
    }
    
}
```
**Q3.** Desenvolva um programa qualquer utilizando a condicional ternária.
```
public class Exe3 {
    public static void main(String[] args) {

        double salario = 1000;
        double bonus = 0.0;

        if (salario > 1000) {bonus = salario * 0.10;}
        else {bonus = salario * 0.15;}

        System.out.println(bonus);
        
    }
}
```
**Q4.** Desenvolva um programa que pede para o usuário digitar o dia da semana. Se for sábado ou domingo, deve aparecer a mensagem "descanso", senão, deve aparecer a mensagem "estudar".
```
import java.util.Scanner;

public class Exe4 {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);
        
        System.out.println("Digite o dia");
        String day = scanner.next();
     

            switch (day) {
                case "domingo" :
                System.out.println("descansar");
                break;
                case "sabado":
                System.out.println("descansar");
                break;
                case "segunda":
                System.out.println("estudar");
                break;
                case "terça":
                System.out.println("estudar");
                break;
                case "quarta":
                System.out.println("estudar");
                break;
                case "quinta":
                System.out.println("estudar");
                break;
                case "sexta":
                System.out.println("estudar");

                default:
                System.out.println("Vc deve escrever o dia da semana");
                    break;
            }
        scanner.close();
    }
         
```
**Q5.** Desenvolva um programa onde o usuário informa um número de 1 a 12 e retorna o mês correspondente.
```
import java.util.Scanner;


public class Exe5 {

    public static void main(String[] args) {


        Scanner scanner = new Scanner(System.in);
        
        System.out.println("Digite o mes");
        String day = scanner.next();
     

            switch (day) {
                case "1" :
                System.out.println("jan");
                break;
                case "2":
                System.out.println("fev");
                break;
                case "3":
                System.out.println("mar");
                break;
                case "4":
                System.out.println("abr");
                break;
                case "5":
                System.out.println("mai");
                break;
                case "6":
                System.out.println("jun");
                break;
                case "7":
                System.out.println("jul");
                case "8":
                System.out.println("ago");
                case "9":
                System.out.println("set");
                case "10":
                System.out.println("out");
                case "11":
                System.out.println("nov");
                case "12":
                System.out.println("dez");

                default:
                System.out.println("Vc deve digitar o mes");
                    break;
            }
        scanner.close();
    }
         
        
        

    }
```
**Q6.** Desenvolva um programa que pede as notas 1, 2 e 3 com pesos 2, 3 e 5, respectivamente, do aluno e faça o cálculo da média. Dependendo da nota, o programa retorna a seguinte mensagem:
* se a media for entre 0.0 e 4.9: reprovado
* se a media for entre 5.0 e 7.9: em recuperação
* se a media for entre 8.0 e 10.0: aprovado
```
import java.util.Scanner;

public class Exe6 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("Digite a nota");
        double nota = scanner.nextDouble();

        System.out.println("digdite a nota ( peso 2 :)");
        double nota1 = scanner.nextDouble();

        System.out.println("digdite a nota ( peso 3 :)");
        double nota2 = scanner.nextDouble();

        System.out.println("digdite a nota ( peso 5 :)");
        double nota3 = scanner.nextDouble();

        double media = (nota1*2 + nota2*3 + nota3*5)/ (2+3+5);

        System.out.println(nota);



        if (nota >= 8.0 && nota <= 10.0) 
            {System.out.println("vc foi aprovado");
            
        }
        else if (nota >= 5.0 && nota <= 7.9) 
            { System.out.println("vc esta de recuperaçao");
            
        }
        else if (nota >= 0.0 && nota <= 4.9)
        {System.err.println("vc reprovou");}
        
        else{System.out.println("media invalida");}
        
        scanner.close();
    }
    
}
```
**Q7.** Crie um laço de repetição com que exiba os com os números de 1 até 10 em ordem crescente e depois em ordem decrescente.
```
public class ExeSete {

    public static void main(String[] args) {



       for (int i =  1; i <= 10; i++){
        System.out.println("a contagem ta em " + i);
        }

       for (int i =  10; i >= 1; i--){System.out.println("a contagem ta em " + i);}

        
    }
    
}
```
**Q8.** Crie um laço de repetição que exiba os com os números pares de 10 até 50 em ordem crescente e depois em ordem decrescente.
```
public class Exe8 {

    public static void main(String[] args) {
        for (int i =  10; i <= 50; i += 2){System.out.println(i);}

        for (int i =  50; i >= 10; i -= 2){System.out.println(i);}

        
    }
    
}
```
**Q9.** Utilizando um laço de repetição, desenvolva um programa que exiba a tabuada de 1 a 10. Para isso, peça para o usuário escolher um número de 1 a 10. Se o usuário digitar um valor fora desse intervalo, deve aparecer a seguinte mensagem de erro: “Digite um valor entre 1 e 10.” A tela esperada deve conter os valores da tabuada para o número digitado pelo usuário.
```
import java.util.Scanner;
public class Exe9 {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);
        
        System.out.println("Digite o numero");
        int numero;

        numero=scanner.nextInt();
        System.out.println("digite um numero de 1 a 10 ");
        if (numero < 1 && numero > 10 )
        {System.out.println("erro digitw entre 1 a 10 ");}
        else System.out.println("tabuada do " + numero + ":" );



        for (int i =  1; i <= 10; i++){System.out.println(numero + "x" + i + "=" +(numero*i));}

        
        scanner.close();
    }
    
}
```

### **Vetores e Matrizes**

**Q1.** Crie um programa que leia um vetor de números inteiros e exiba a soma de todos os elementos.
```
import java.util.Scanner;

public class ExeU {
    public static void main(String[] args) {
        Scanner goiaba = new Scanner(System.in);

        System.out.println("didgite um numero pro vetor ");
        int tamanho = goiaba.nextInt();
        int[] numeros = new int[tamanho];

         for (int i = 0; i <tamanho ;i++){System.out.println("elemento"+ (i+1)+":");

        numeros[i] = goiaba.nextInt();}

        int soma =0;
        for ( int num : numeros){soma += num;}

        System.out.println(" a soma total e " + soma);

        goiaba.close();
        
    }
    
}
```
**Q2.** Faça um programa que leia um vetor de números inteiros e exiba o maior elemento presente no vetor.
```
import java.util.Scanner;

public class ExeD {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("digite a quantidade de numero ");

        int n = scanner.nextInt();

        int[] vetor =  new int[n];
        System.out.println("digite ");

        for (int i = 0;i<n;i++){
            vetor[i]=scanner.nextInt();
        }

        int maior = vetor[0];

        for (int i = 1; i<n;i++){
            if (vetor[i]>maior){maior= vetor[i];}

        }

        System.out.println("o maior numero e " + maior);

        scanner.close();

        
    }
    
}
```
**Q3.** Faça um programa que leia um vetor de números inteiros e exiba a média dos elementos.
```
import java.util.Scanner;

public class ExeT {

    public static void main(String[] args) {
         Scanner pdp = new Scanner(System.in);

         System.out.println("digite o tamanho do numero");

         int tamanho = pdp.nextInt();

         int[] numeros = new int[tamanho];
         int soma = 0;

    for (int i = 0;i<tamanho;i++){System.out.println("didgite o mumero " + (1+i) + ":");
    numeros[i]=pdp.nextInt();

    soma+=numeros[i];}

    double media = (double)soma/tamanho;

    System.out.println("a media e " + media);

        pdp.close();
        
    }
    
}
```
**Q4.** Crie um programa que leia um vetor de números inteiros e verifique se todos os elementos são pares.
```
import java.util.Scanner;

public class ExeQu {

    public static void main(String[] args) {
        Scanner sla = new Scanner(System.in);

        System.out.println("digite o tamanho");
        int tamanho = sla.nextInt();

        int[] numeros = new int[tamanho];

        System.out.println("didgite o numero intero");

        for (int i= 0;i< tamanho; i++){
            numeros[i] = sla.nextInt();
        }

        boolean todosPares = true;
        for (int num : numeros){ 
            if (num % 2 !=0){todosPares = false;break;}
        }
        if (todosPares){System.out.println("todos os numeros sao pares ");}
        else{System.out.println("nem todos numeros sao pares");}

        sla.close();
    }
    
}
```
**Q5.** Faça um programa que leia duas matrizes 2x2 e exiba a soma das duas matrizes.
```
import java.util.Scanner;

public class ExeC {

    public static void main(String[] args) {

        Scanner pato = new Scanner(System.in);

        int[][] mat1 = new int[2][2];
        int[][] mat2 = new int[2][2];
        int[][] soma = new int[2][2];

        System.out.println("digite o primeiro numero da matriz 2x2 ");
        for(int i= 0;i<2; i++){for(int j = 0;j<2;j++){
            System.out.println("elemento ["+i+"]["+j+"]:");
             mat1[i][j]=pato.nextInt();}}

             System.out.println("digite o segundo numero da matriz 2x2 ");
        for(int i = 0; i < 2;i++){for(int j = 0;j<2;j++){
            System.out.println("elemento["+i+"]["+j+"]:");
             mat2[i][j]=pato.nextInt();}}

             for(int i = 0; i < 2;i++){for(int j = 0;j<2;j++){
             soma[i][j]=mat1[i][j]+mat2[i][j];}}

                System.out.println("a soma das duas matrizes e:");
             for(int i = 0; i < 2;i++){for(int j = 0;j<2;j++)
                {System.out.println(soma[i][j]+" ");System.out.println();}
             }
        
        pato.close();
    }
    
}
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

