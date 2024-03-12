## Resumo da aula de hoje

Abaixo está o código que foi usado como exemplo durante as aulas

```
// Hello World program in Go
package main

import "fmt"

// Na linguagem de programação Go, a função main() é o ponto
// de entrada da sua aplicação.
/*
Isso é um comentário de bloco
*/

func main() {
	/*var nome string
	//var sobrenome string

	fmt.Println("Qual é o seu nome?")
	// Lê a entrada do usuário
	// Scaln é uma função que lê a entrada do usuário
	// e armazena na variável nome
	fmt.Scanln(&nome) // por hora, não vamos usar espaços.
	fmt.Println("Olá", nome)
	*/

	var v1 float64
	var v2 float64
	var resultado float64

	fmt.Println("########################################")
	fmt.Println("Programa de somar")
	fmt.Println("Digite o primeiro valor")
	fmt.Scanln(&v1)
	fmt.Println("Digite o segundo valor")
	fmt.Scanln(&v2)

	resultado = v1 + v2

	fmt.Println("O resultado da soma é", resultado)
}
```

## Comentários
Na aula de hoje nós conversamos sobre comentários.
Comentários nada mais são do que lembretes que adicionamos ao código para nos lembrarmos depois e/ou
ajudar eventual outra pessoa que for manusear o código.

Em Go , nós utilizamos o `//` para comentários de apenas uma linha ou então,
nós podemos utilizar o padrão `/*     */` para comentários de bloco.


## Capturando a entrada do usuários ( ou user input)
Entrada do usuário (ou User Input, em inglês) é o que o usuário digita e confirma ao apertar a tecla Enter.
Toda linguagem de programação, Go inclusive é capaz de fazer isso de múltiplas maneiras, tem uma maneira
de capturar essa informação e armazena-la em uma variável.
Para os nossos exemplos, vamos nos ater as maneiras mais simples, ou seja, usando o `fmt.Scanln`.
A função fmt.Scanln() na linguagem Go verifica os textos de entrada que são fornecidos na entrada padrão,
lê a partir daí e armazena os valores separados por espaço sucessivos em argumentos sucessivos.
Esta função interrompe a digitalização em uma nova linha (Enter) e após o item final, deve haver uma nova linha.
Você pode conferir no código acima como utilizamos a função `fmt.Scanln`.


## Interação matemática entre variáveis
Por fim nós escrevemos um programa que pede ao usuário para fornecer números e o programa retorna 
a soma desses números.


## Exercícios
Para praticar o uso do `fmt.Scanln`, escreva 3 novos programas.
1 programa que pede ao usuário para fornecer 2 números e retorna o resultado da subtração entre eles.
1 programa que pede ao usuário para fornecer 2 números e retorna o resultado da multiplicação entre eles.
1 programa que pede ao usuário para fornecer 2 números e retorna o resultado da divisão entre eles.


### Dica
Lembre-se que as variáveis possuem tipos e que elas apenas podem interagir entre si se elas forem do mesmo tipo.
Assim só pode executar operações matemáticas de `int` com `int` e `float64` com `float64`
