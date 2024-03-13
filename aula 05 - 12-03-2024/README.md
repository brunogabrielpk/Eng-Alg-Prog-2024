## Resumo da aula de hoje
Hoje nós começamos a trabalhar com estrutura condicionais.
Estrutura condicionais permitem que os algoritmos "tomem decisões" para direcionar o fluxo da aplicação

Abaixo está o código que foi trabalhado em sala de aula.

```
package main

import "fmt"

func main() {

	var operacao string

	fmt.Println("Digite a operação desejada: ")
	fmt.Println("Digite 'soma' para somar")
	fmt.Println("Digite 'sub' para subtrair")
	fmt.Println("Digite 'mult' para multiplicar")
	fmt.Println("Digite 'div' para dividir")
	fmt.Scanln(&operacao)

	if operacao == "soma" {
		var n1 int
		var n2 int
		var resultado int
		fmt.Println("Digite o primeiro número: ")
		fmt.Scanln(&n1)
		fmt.Println("Digite o segundo número: ")
		fmt.Scanln(&n2)

		resultado = n1 + n2
		fmt.Println("O resultado da soma é: ", resultado)
	}

	if operacao == "sub" {
		var n1 int
		var n2 int
		var resultado int

		fmt.Println("Digite o primeiro número: ")
		fmt.Scanln(&n1)
		fmt.Println("Digite o segundo número: ")
		fmt.Scanln(&n2)

		resultado = n1 - n2

		fmt.Println("O resultado da subtração é: ", resultado)
	}

	if operacao == "mult" {
		var n1 int
		var n2 int
		var resultado int

		fmt.Println("Digite o primeiro número: ")
		fmt.Scanln(&n1)
		fmt.Println("Digite o segundo número: ")
		fmt.Scanln(&n2)

		resultado = n1 * n2

		fmt.Println("O resultado da multiplicação é: ", resultado)
	}

	fmt.Println("Encerrando o programa...")
}
```


Obs: Este exemplo trabalhado em sala de aula foi criado tentando representar a maneira mais simples de demostrar as condições através do `if` porém lembre-se que existem maneiras melhores de se executar essa tarefa. 
Você pode, como exercício melhorar esse código e reescrevê-lo sem precisar declarar tantas variáveis.


## Exercício 01
Faça um programa que pergunte a idade do usuário e responda se ele é apto a votar e se o voto dele é obrigatório ou opcional.