# Interpretador de Linguagem Python
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>

Este projeto implementa um **interpretador de linguagem simplificada**, construído em Python, com suporte a análise léxica, interpretação de código e execução de estruturas básicas como variáveis, expressões e condicionais.

---

## Visão geral

O sistema funciona como uma mini-linguagem própria, contendo:

- Análise léxica (Lexer com Regex)
- Interpretador manual (Parser + Executor)
- Variáveis dinâmicas
- Operações matemáticas
- Operadores lógicos
- Estruturas condicionais (`if / else`)
- Bloco principal (`main { }`)

---

## Como o projeto funciona

### 🔤 Lexer
O código é convertido em tokens usando expressões regulares, identificando:
```
- Números
- Identificadores
- Palavras-chave (`var`, `if`, `else`, `main`)
- Operadores (`+ - * / == != >= <=`)
- Símbolos (`{ } ( ) ; :`)
```

---

### 🧩 Interpretador
Após a tokenização, o interpretador:
```
- Executa comandos sequencialmente
- Gerencia variáveis em memória (`self.vars`)
- Avalia expressões matemáticas e lógicas
- Controla fluxo de execução (`if/else`, blocos)
```
---

## Ilustração 
<img width="1282" height="951" alt="1000327435" src="https://github.com/user-attachments/assets/6aa5eb8b-e30b-42b7-aa31-db2599218bd1" />

## Execução
<img width="1503" height="1047" alt="1000327405" src="https://github.com/user-attachments/assets/7845c744-dedf-44c8-a9a7-45ef8112bde8" />

---

## Exemplo de código suportado

```txt
var x:int = 10;
var y:int = 5;
var z:int = 0;

main {
    x = x + 3;
    y = y * 2;

    if x > 10 {
        z = 1;
    } else {
        z = 2;
    }

    if y < 5 or z == 1 {
        x = x + 1;
    }
}


