## Resumo da aula de hoje.

Hoje nós continuamos a ver exemplos de estrutura condicionais que podem direcionar o fluxo do nosso programa.

As estruturas condicionais permitem que um programa tome decisões e altere o fluxo de execução 
com base em condições específicas.
Elas nos permitem controlar quais trechos de código
são executados com base em diferentes situações.


### Estrutura IF

- O `if`é usado para avaliar uma expressão booleana.
Expressão boolena é um expressão que pode apenas resultar em verdadeiro ou falso (true or false)
- Se a condição dentro do `if` for verdadeira, o bloco de código associado a ele é executado.
- Caso contrário, o fluxo de execução passa para o próximo bloco de código (se houver).
```
  idade := 18
if idade >= 18 {
    fmt.Println("Você é maior de idade!")
} else {
    fmt.Println("Você é menor de idade!")
}
```

### Estrutura IF sem ELSE
- Você também pode usar apenas o `if` sem o `else`
```
  temperatura := 25
if temperatura > 30 {
    fmt.Println("Está quente lá fora!")
}
```

### Operadores relacionais
- Os operadores relacionais, como `>`, `<`, `>=`, `<=`, `==` e `!=`, são usados para comparar valores.
- Eles retornam um valor booleano (true ou false).
```
  a := 10
b := 5
if a > b {
    fmt.Println("a é maior que b")
}
```

Lembre-se de que as estruturas condicionais nos permitem controlar o fluxo do programa
com base em condições específicas.
Elas são essenciais para a tomada de decisões em qualquer linguagem de programação.

### Estruturas condicionais aninhadas
São quando você coloca uma instrução if dentro de outra instrução if.
Isso permite que você avalie várias condições sequencialmente.
```
  package main

import "fmt"

func main() {
    numero := 10

    if numero > 0 {
        fmt.Println("O número é positivo")
    } else if numero < 0 {
        fmt.Println("O número é negativo")
    } else {
        fmt.Println("O número é zero")
    }
}

```
