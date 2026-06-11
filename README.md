# Interpretador de uma Linguagem Própria Simplificada, Implementado em Python
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

**🔤 Lexer**
O código é convertido em tokens usando expressões regulares, identificando:
```
- Números
- Identificadores
- Palavras-chave (`var`, `if`, `else`, `main`)
- Operadores (`+ - * / == != >= <=`)
- Símbolos (`{ } ( ) ; :`)
```

---
**🧩 Interpretador**
Após a tokenização, o interpretador:
```
- Executa comandos sequencialmente
- Gerencia variáveis em memória (`self.vars`)
- Avalia expressões matemáticas e lógicas
- Controla fluxo de execução (`if/else`, blocos)
```
---

## Ilustração 
<img width="1520" height="937" alt="1000327436" src="https://github.com/user-attachments/assets/39d2c662-fe9e-4fa0-8c13-8142a1fbac12" />

---
