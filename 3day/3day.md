# Fundamentos de JavaScript (Dia 1-3)

## Objetivos dos Dias 1-3:
- **Compreender os conceitos fundamentais do JavaScript**.
- **Aprender a trabalhar com variáveis, tipos de dados e operadores**.
- **Entender como usar o controle de fluxo** para criar decisões e repetição no código.

## 1. Variáveis e Tipos de Dados

### 1.1 Variáveis
Em JavaScript, as variáveis são usadas para armazenar valores. Existem três maneiras de declarar variáveis:
- **`let`**: Para variáveis cujo valor pode ser alterado.
- **`const`**: Para variáveis cujo valor não pode ser alterado após a atribuição.
- **`var`**: Forma mais antiga de declarar variáveis, mas não é recomendada para uso moderno.

#### Exemplo:
```javascript
let nome = "Bruna";  // String
const idade = 25;   // Number
let ativo = true;   // Boolean
```

### 1.2 Tipos de Dados
JavaScript tem vários tipos de dados:
- **Primitivos**:
  - **String**: Sequência de caracteres, ex: `"Bruna"`.
  - **Number**: Números, ex: `25`, `8.5`.
  - **Boolean**: Valor lógico, `true` ou `false`.
  - **Null**: Representa um valor nulo, ex: `null`.
  - **Undefined**: Quando uma variável não tem valor atribuído.
  - **Symbol** (ES6): Tipo único usado para identificadores.

#### Exemplo:
```javascript
let nome = "Bruna";  // String
let idade = 25;     // Number
let ativo = true;   // Boolean
```

---

## 2. Operadores

Os operadores em JavaScript são usados para realizar operações em variáveis e valores.

### 2.1 Operadores Aritméticos
- **`+`**: Soma
- **`-`**: Subtração
- **`*`**: Multiplicação
- **`/`**: Divisão
- **`%`**: Módulo (resto da divisão)

#### Exemplo:
```javascript
let soma = 10 + 5;   // 15
let multiplicacao = 4 * 3;   // 12
let resto = 10 % 3;   // 1
```

### 2.2 Operadores de Comparação
São usados para comparar valores.
- **`==`**: Igualdade (sem tipo)
- **`===`**: Igualdade (com tipo)
- **`!=`**: Diferença
- **`>`**: Maior que
- **`<`**: Menor que
- **`>=`**: Maior ou igual
- **`<=`**: Menor ou igual

#### Exemplo:
```javascript
let resultado = (5 == 5);  // true
let diferente = (10 != 5);  // true
```

### 2.3 Operadores Lógicos
São usados para combinar expressões booleanas:
- **`&&`**: E (AND)
- **`||`**: Ou (OR)
- **`!`**: Não (NOT)

#### Exemplo:
```javascript
let idade = 18;
let temCarta = true;

if (idade >= 18 && temCarta) {
  console.log("Você pode dirigir!");
}
```

---

## 3. Controle de Fluxo

O controle de fluxo permite que o código tome decisões baseadas em condições e execute repetições.

### 3.1 Condicionais (`if`, `else`, `else if`)

O **`if`** executa um bloco de código se a condição for verdadeira. O **`else`** executa um bloco alternativo se a condição for falsa. O **`else if`** permite verificar múltiplas condições.

#### Sintaxe:
```javascript
if (condição) {
    // Código se a condição for verdadeira
} else if (outra condição) {
    // Código se a outra condição for verdadeira
} else {
    // Código se nenhuma das condições anteriores for verdadeira
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

### 3.2 switch

O **`switch`** é utilizado para comparar uma variável com múltiplos casos. Ele é mais útil quando há muitas condições baseadas em um único valor.

#### Sintaxe:
```javascript
switch (expressão) {
  case valor1:
    // Código para o caso 1
    break;
  case valor2:
    // Código para o caso 2
    break;
  default:
    // Código para o caso padrão
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
  default:
    console.log("Não sei que dia é hoje.");
}
```

### 3.3 Laços de Repetição (`for`, `while`, `do...while`)

Os laços de repetição permitem executar um bloco de código várias vezes.

#### 3.3.1 `for`
Usado quando sabemos o número de iterações que queremos executar.

#### Sintaxe:
```javascript
for (inicialização; condição; incremento) {
  // Bloco de código
}
```

#### Exemplo:
```javascript
for (let i = 1; i <= 5; i++) {
  console.log("Contagem: " + i);
}
```

#### 3.3.2 `while`
Usado quando não sabemos quantas iterações serão necessárias, mas temos uma condição para checar.

#### Sintaxe:
```javascript
while (condição) {
  // Bloco de código
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

#### 3.3.3 `do...while`
Executa o bloco de código pelo menos uma vez e depois verifica a condição.

#### Sintaxe:
```javascript
do {
  // Bloco de código
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

---

## Conclusão

Nos primeiros três dias, cobrimos os conceitos básicos de JavaScript:
- **Variáveis** e **tipos de dados**.
- **Operadores** aritméticos, de comparação e lógicos.
- **Controle de fluxo** utilizando **condicionais** e **laços de repetição**.

Esses conceitos são fundamentais para a construção de qualquer programa ou aplicação em JavaScript e serão a base para aprender e trabalhar com recursos mais avançados no futuro. 

### Próximos Passos:
- Continuar praticando esses conceitos criando pequenos projetos.
- Explorar mais sobre funções, manipulação do DOM e eventos em JavaScript.