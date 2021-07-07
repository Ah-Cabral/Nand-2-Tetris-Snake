# Programação em alto nível

## Aula 01 - Visão Geral Da Linguagem Jack

### Linguagem Jack: 

- Linguagem simples.
- Muito similar à linguagem Java (Java-like).
- Propósito Geral (Pode ser utilizada em diversas aplicações).
- Permite desenvolver aplicações com interação com o usuário.

### Como será abordado?

<b> -Programação em alto Nível: </b>
- Hello World
- Programação Procedural
- Programação Orientada à objetos
- Processando Listas

#### Hello World

```java

/* Hello World */

class Main{ //Classe main é a classe principal do programa

    function void main(){ //Onde dentro dela existe uma função main interna

        /*Fazer print de algum texto utilizando uma lib padrão*/

    //  do --> utilizado para execução de comando
        do Output.printString("Hello World!"); //A função printString imprime a frase Hello World na tela.

        do Output.println(); //Quebra de linha

        return; //Obrigatório em jack, indica final da função
    }
}

```

#### Como Temos Um Programação Procedural Dentro Do Jack?

```java

/* Insira alguns números e retorne a média entre eles */

class Main{ 

    function void main(){ //Respondendo a pergunta acima, inserindo variáveis dentro da function main

        //Declarando Variáveis
        var Array a;
        //length --> Comprimento do Array
        var int comprimento;
        var int i, soma;

        let comprimento = Keyboard.readInt("Quantos Números?") //Definindo tamanho do array

        let a Array.new(comprimento);

        while(i < length){ //Enquanto o i for um valor menor do que o comprimento do array

            let a[i] = Keyboard.readInt("Insira um número: "); //Um número é inserido

            let soma = soma + a[i]; //E colocado na variável

            let i = i + 1; //Incrementação no índice
        }

        do Output.printString("O Valor da média é "); //Printando String
        do Output.printInt( soma / comprimento ); //Printando cálculo da média (Note que aqui não foi colocado o do Output.println();)
        //Logo, tudo será impresso na mesma linha
        return;
    }
}

```

#### Estrutura da linguagem Jack:

<ul>
    <li> <p> Um programa jack é uma coleção de classes onde uma delas precisa ser a main </p> </li>
    <li>
        <ul>
            <li>Tipos Primitivos em Jack (3 Tipos):</li>
            <li>Int (Inteiro) </li>
            <li>Char (Caractere) </li>
            <li>Boolean (True / False) </li>
        </ul>
        <ul>
            <li>Tipos Baseados Em Classes:</li>
            <li>Array (Implementado Como Parte Da Lib Padrão Do Jack) / Não São Tipados (Podem haver diversos tipos de variáveis)</li>
            <li>String</li>
        </ul>
         <ul>
            <li>Controles De Fluxo:</li>
            <li>if / if... else</li>
            <li>While</li>
            <li>do</li>
        </ul>
        <ul>
            <li>Serviços de Sistema Operacional:</li>
            <li>Keyboard.readInt()</li>
            <li>Output.printString()</li>
            <li>Output.printInt()</li>
        </ul>
    </li>
</ul>