# Target Quests

Este repositório contém soluções para uma série de desafios de lógica e programação. Cada desafio aborda um problema específico e fornece uma solução na linguagem JavaScript.

## Desafios

### 1. Soma de Números

Dado o trecho de código em um pseudocódigo:

```plaintext
int INDICE = 13, SOMA = 0, K = 0;

enquanto K < INDICE faça
{
    K = K + 1;
    SOMA = SOMA + K;
}

imprimir(SOMA);
```

Ao final do processamento, qual será o valor da variável SOMA?

**Resposta:** A variável SOMA conterá o valor 91.

### 2. Sequência de Fibonacci

Escreva um programa em JavaScript onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não à sequência.

**Resposta:** 
```javascript
function verificaFibonacci(numero) {
    let a = 0;
    let b = 1;
    let temp;

    while (b <= numero) {
        if (b === numero) {
            return true;
        }
        temp = b;
        b = a + b;
        a = temp;
    }

    return false;
}

const numeroVerificar = 21;
if (verificaFibonacci(numeroVerificar)) {
    console.log(numeroVerificar + " pertence à sequência de Fibonacci.");
} else {
    console.log(numeroVerificar + " não pertence à sequência de Fibonacci.");
}
```

### 3. Completar Sequências

Descubra a lógica e complete o próximo elemento das seguintes sequências:

a) 1, 3, 5, 7, ___

b) 2, 4, 8, 16, 32, 64, ____

c) 0, 1, 4, 9, 16, 25, 36, ____

d) 4, 16, 36, 64, ____

e) 1, 1, 2, 3, 5, 8, ____

f) 2,10, 12, 16, 17, 18, 19, ____

**Respostas:**

a) 1, 3, 5, 7, **9**

b) 2, 4, 8, 16, 32, 64, **128**

c) 0, 1, 4, 9, 16, 25, 36, **49**

d) 4, 16, 36, 64, **100**

e) 1, 1, 2, 3, 5, 8, **13**

f) 2,10, 12, 16, 17, 18, 19, **20**


### 4. Descobrindo Interruptores e Lâmpadas

Você está em uma sala com três interruptores, cada um conectado a uma lâmpada em uma sala diferente. Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas, qual interruptor controla cada lâmpada?

**Resposta:**
    Ligue o primeiro interruptor e aguarde alguns minutos.
    Desligue o primeiro interruptor e ligue o segundo interruptor.
    Entre na sala.
    Se a lâmpada estiver acesa, o primeiro interruptor controla essa lâmpada. Se estiver desligada e a lâmpada estiver quente, o segundo interruptor controla essa lâmpada. Se estiver desligada e a lâmpada estiver fria, o terceiro interruptor controla essa lâmpada.

### 5. Inverter uma String

Escreva um programa em JavaScript que inverta os caracteres de uma string.

**Resposta:**
```javascript
function inverteString(string) {
    let novaString = '';
    for (let i = string.length - 1; i >= 0; i--) {
        novaString += string[i];
    }
    return novaString;
}

const minhaString = "Olá, mundo!";
console.log("String original: " + minhaString);
console.log("String invertida: " + inverteString(minhaString));
```

## Licença

Este projeto está licenciado sob a Licença MIT - consulte o arquivo [LICENSE](LICENSE) para obter detalhes.

```
