### Método `flat()`
O método `flat()` **achata** arrays aninhados, ou seja, transforma um array de arrays em um único array.

#### Exemplo de `flat()`:
```javascript
let arr = [1, [2, 3], [4, [5, 6]]];
let arrAchado = arr.flat(2);  // Aprofunda até o nível 2
console.log(arrAchado);  // Exibe: [1, 2, 3, 4, 5, 6]
```

Aqui, `flat(2)` achata o array até o segundo nível, unindo todos os valores em um único array.

### Método `sort()`
O método `sort()` permite ordenar os elementos de um array. Ele ordena **de forma lexicográfica** por padrão (como se fosse uma string), mas é possível passar uma função de comparação para ordenação numérica.

#### Exemplo de `sort()` com números:
```javascript
let numeros = [4, 1, 7, 3, 9];
numeros.sort((a, b) => a - b);  // Ordenação numérica crescente
console.log(numeros);  // Exibe: [1, 3, 4, 7, 9]
```

A função de comparação `(a, b) => a - b` garante que os números sejam ordenados corretamente.

---

## 3. Manipulação de Arrays com Funções de Alta Ordem

Agora que já discutimos as funções de alta ordem, podemos aplicar isso para manipular arrays de maneira avançada.

#### Exemplo de uso de `map()`, `filter()` e `reduce()` em conjunto:
```javascript
let numeros = [1, 2, 3, 4, 5];

// Usando map() para multiplicar os números por 2
let dobrados = numeros.map(num => num * 2);

// Usando filter() para pegar apenas os números maiores que 5
let maioresQueCinco = dobrados.filter(num => num > 5);

// Usando reduce() para somar os números restantes
let soma = maioresQueCinco.reduce((acc, num) => acc + num, 0);

console.log(soma);  // Exibe: 18 (6 + 8 + 10)
```

Aqui, usamos `map()` para multiplicar os números por 2, `filter()` para filtrar os números maiores que 5, e `reduce()` para somar os números restantes.

---

## Conclusão do Dia 5:
No **Dia 5**, você aprendeu conceitos **avançados de funções e arrays**, como funções de alta ordem, recursivas, closures, e a manipulação de arrays com métodos modernos como `find()`, `some()`, `every()`, `flat()`, e ordenação com `sort()`. Esses conceitos são essenciais para escrever códigos mais poderosos e eficientes.

Essas técnicas irão te ajudar a escrever códigos mais limpos, reutilizáveis e com melhor desempenho. 