# Controle de Fluxo em JavaScript

## Objetivos:
- **Aprender a controlar o fluxo de execução do código** utilizando estruturas condicionais e laços de repetição.
- **Compreender como as decisões e repetições funcionam em JavaScript** e como implementá-las no seu código.

## 1. Condicionais em JavaScript

As condicionais permitem que você execute diferentes partes do código com base em condições.

### 1.1 if/else

A estrutura `if/else` é usada para tomar decisões. O `if` executa um bloco de código se uma condição for verdadeira, e o `else` executa um bloco de código alternativo se a condição for falsa.

#### Sintaxe:
```javascript
if (condição) {
    // Bloco de código executado se a condição for verdadeira
} else {
    // Bloco de código executado se a condição for falsa
}
```

#### Exemplo:
```javascript
let idade = 20;

if (idade >= 18) {
    console.log("Você é maior de idade.");
} else {
    console.log("Você é menor de idade.");
}
```

### 1.2 else if

O `else if` é usado quando há múltiplas condições a serem verificadas. Isso permite testar várias condições diferentes, uma após a outra.

#### Sintaxe:
```javascript
if (condição1) {
    // Bloco de código executado se condição1 for verdadeira
} else if (condição2) {
    // Bloco de código executado se condição2 for verdadeira
} else {
    // Bloco de código executado se nenhuma das condições anteriores for verdadeira
}
```

#### Exemplo:
```javascript
let nota = 8;

if (nota === 10) {
    console.log("Nota excelente!");
} else if (nota >= 7) {
    console.log("Boa nota!");
} else {
    console.log("Precisa melhorar.");
}
```

### 1.3 switch

O `switch` é útil quando temos várias opções para testar uma variável ou expressão. Ele compara o valor da variável com os diferentes casos fornecidos e executa o bloco de código correspondente.

#### Sintaxe:
```javascript
switch (expressão) {
    case valor1:
        // Bloco de código executado se a expressão for igual a valor1
        break;
    case valor2:
        // Bloco de código executado se a expressão for igual a valor2
        break;
    default:
        // Bloco de código executado se nenhum dos casos for verdadeiro
}
```

#### Exemplo:
```javascript
let dia = "segunda-feira";

switch (dia) {
    case "segunda-feira":
        console.log("Hoje é segunda-feira.");
        break;
    case "terça-feira":
        console.log("Hoje é terça-feira.");
        break;
    case "quarta-feira":
        console.log("Hoje é quarta-feira.");
        break;
    default:
        console.log("Não sei que dia é hoje.");
}
```

## 2. Laços de Repetição em JavaScript

Os laços de repetição permitem que um bloco de código seja executado várias vezes. Eles são essenciais quando precisamos executar ações repetidamente, como iterar sobre listas ou executar uma tarefa até que uma condição seja atendida.

### 2.1 for

O laço `for` é ideal quando sabemos o número exato de iterações. Ele é composto por três partes: inicialização, condição e incremento.

#### Sintaxe:
```javascript
for (inicialização; condição; incremento) {
    // Bloco de código executado enquanto a condição for verdadeira
}
```

#### Exemplo:
```javascript
for (let i = 1; i <= 5; i++) {
    console.log("Contagem: " + i);
}
```

### 2.2 while

O laço `while` é usado quando não sabemos o número de iterações com antecedência. Ele executa um bloco de código enquanto uma condição for verdadeira.

#### Sintaxe:
```javascript
while (condição) {
    // Bloco de código executado enquanto a condição for verdadeira
}
```

#### Exemplo:
```javascript
let contador = 1;
while (contador <= 5) {
    console.log("Contagem: " + contador);
    contador++;
}
```

### 2.3 do...while

O laço `do...while` é similar ao `while`, mas a diferença é que ele garante que o bloco de código seja executado **pelo menos uma vez**, mesmo que a condição seja falsa.

#### Sintaxe:
```javascript
do {
    // Bloco de código executado pelo menos uma vez
} while (condição);
```

#### Exemplo:
```javascript
let contador2 = 1;
do {
    console.log("Contagem: " + contador2);
    contador2++;
} while (contador2 <= 5);
```

## Conclusão

O **controle de fluxo** é uma das bases para escrever programas lógicos e dinâmicos. Com as **estruturas condicionais** e os **laços de repetição**, você pode controlar o comportamento do seu código com base em condições e repetição de tarefas.

- **Condicionais** como `if`, `else`, e `switch` permitem que o programa tome decisões.
- **Laços de repetição** como `for`, `while`, e `do...while` permitem que você execute ações repetidamente.

Dominar essas estruturas é fundamental para criar programas mais complexos e eficientes.