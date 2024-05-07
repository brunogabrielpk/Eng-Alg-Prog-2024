## Funções em GO

As funções, também conhecidas como  sub-rotinas, são muito utilizadas em programação. Um dos grandes benefícios é não precisar copiar o código todas as vezes que precisar executar aquela operação, além de deixar a leitura do código mais intuitiva.

A ideia básica de uma função, implementada em alguma linguagem de programação, é encapsular um código que poderá ser invocado/chamado por qualquer outro trecho do programa. Seu significado e uso são muito parecidos com o de funções matemáticas, ou seja, existe um nome, uma definição e posterior invocação à função.

### Sintaxe das funções em Go(Lang)
Primeiramente, para podermos criar nossas próprias funções na Golang, precisamos entender qual a sintaxe utilizada para realizar a definição de uma função.

Para criarmos uma função utilizamos a palavra reservada `func`. Uma função em Go e na maioria das linguagens de programação é composta por quatro partes, sendo elas:

- **Nome**: o nome da função, esse nome é o que iremos utilizar para podermos executar essa função posteriormente ao longo do nosso código;
- **Parâmetros**: os parâmetros são onde definimos quais são os dados que precisam ser passados para que a nossa função possa funcionar corretamente, podemos passar mais de um parâmetro, desde que esses parâmetros estejam separados por vírgula;
- **Retorno**: no retorno nós definimos qual será o tipo de dado retornado pela nossa função ao término do seu processamento;
- **Corpo**: o corpo da função é onde iremos colocar o código que irá realizar o processamento da função, ou seja, é onde colocamos o código que iremos reaproveitar.

### Exemplo
```go
func validarCpf(cpf string) bool {
	// Condigo onde teremos a validação do cpf
}
```

No código acima nós temos a definição de uma função chamada `validarCpf`, essa função recebe um parâmetro chamado `cpf` que deve ser do tipo `string` e ao término de sua execução irá retornar um dado do tipo `bool`

### Funções sem parâmetros e/ou sem retorno
Parâmetros e Retornos são itens opcionais.

```go
package main

import "fmt"

func boasVindas() {
	fmt.Println("Boas-vindas ao meu programa escrito em Go!")
}

func main() {
	boasVindas()
}
```
No exemplo acima nós temos duas funções sem parâmetro e sem retorno, são as funções `main` e `boasVindas`. Na função `boasVindas` temos o comando para exibir no terminal o texto “Boas-vindas ao meu programa escrito em Go!”. Enquanto na nossa função `main` nós temos a execução da função `boasVindas`, para podermos executar uma função basta colocarmos o nome da função seguida da abertura e fechamento de parênteses.

### Funções com parâmetro
```go
package main

import "fmt"

func boasVindas(nome string) {
	fmt.Println("Boas-vindas", nome)
}

func main() {
	boasVindas("Cleyson")
}
```
Veja que agora nossa função `boasVindas` recebe um parâmetro chamado `nome` do tipo `string`. Esse parâmetro `nome` está sendo utilizado para podermos alterar o comportamento de nossa função, fazendo assim que a mensagem impressa no terminal difira conforme o valor do parâmetro passado.

Por fim, uma função pode receber quantos parâmetros sejam necessários, desde que, eles sejam separados por vírgula.

```go
package main

import "fmt"

func somar(x int, y int) {
	resultado := x + y
	fmt.Println(resultado)
}

func main() {
	somar(1, 2)
}
```

### Funções com retorno
#### Retornando um único valor
```go
package main

import "fmt"

func somar(x int, y int) int {
  resultado := x + y
  return resultado
}

func main() {
  resultado := somar(1, 2)
  fmt.Println(resultado)
}
```
No exemplo acima, a função `somar` recebe dois parâmetros do tipo `int` e retorna um valor do tipo `int`. Ao chamarmos a função somar podemos armazenar o valor retornado em uma variável.

#### Retornando mais de um valor
```go
package main

import "fmt"

func somarESubtrair(x int, y int) (int, int) {
  soma := x + y
  subtracao := x - y
  return soma, subtracao
}

func main() {
  soma, subtracao := somarESubtrair(1, 2)
  fmt.Println(soma, subtracao)
}
```
No exemplo acima, a função `somarESubtrair` recebe dois parâmetros do tipo `int` e retorna dois valores do tipo `int`. Ao chamarmos a função `somarESubtrair` podemos armazenar os valores retornados em variáveis.

Caso queiramos ignorar um dos valores retornados, podemos utilizar o caractere `_` (underscore) para ignorar o valor.
```go
package main

import "fmt"

func somarESubtrair(x int, y int) (int, int) {
  soma := x + y
  subtracao := x - y
  return soma, subtracao
}

func main() {
  soma, _ := somarESubtrair(1, 2)
  fmt.Println(soma)
}
```ß


