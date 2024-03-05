# Resumo da aula
Bom, antes de mais nada eu gostaria de inserir um disclaimer aqui.
Eu não consegui subir esse resumo antes por conta de contratempos. sorry :(


## Agora sim, o resumo
Nessa aula, nós falamos sobre variáveis e tipos de variáveis.
Em Go, para declarar uma variável, utilizamos a palavra-chave var seguida do nome da variável e do seu tipo.

Considere o exemplo abaixo:
```
package main
import "fmt"

func main() {
    var nome string
    nome = "Gopher"
    fmt.Println(nome)
}
```
`var nome string` é a declaração da variável nome do tipo string.
O tipo de variável string é uma sequência de caracteres.
`nome = "Gopher"` é a atribuição do valor "Gopher" à variável nome.
`fmt.Println(nome)` é a impressão do valor da variável nome.

Existem outros tipos de variáveis em Go, como int, float64, bool, entre outros.
Nós vamos trabalhar com esses tipos de variáveis mais a frente.

Outro tópico que discutimos foram os parametros da função `fmt.Println()`.
Essa função é utilizada para imprimir valores no console/terminal.
Ela aceita um número *variável* de parametros, ou seja, você pode passar quantos parametros quiser para ela.
Exemplo:
Considerando o exemplo anterior, podemos reescrever o código da seguinte forma:
```
package main
import "fmt"

func main() {
    var nome string
    nome = "Gopher"
    fmt.Println("O nome armazenado na variável nome é: ", nome)
}
```
Dessa vez, ao invés de passar apenas um parametro para a função `fmt.Println()`, passamos dois parametros.

## Operador :=
- O operador `:=` é usado para inicializar uma variável e atribuir um valor a ela ao mesmo tempo.
Ele é frequentemente usado para criar novas variáveis dentro de uma função.
- A sintaxe é a seguinte:
```
nome_da_variável := valor
```
- O Go infere automaticamente o tipo da variável com base no valor atribuído.

### Exemplos
```
package main

import "fmt"

func main() {
    // Exemplo 1: Inicializando uma variável int
    idade := 30
    fmt.Println("Idade:", idade)

    // Exemplo 2: Inicializando uma variável string
    nome := "Alice"
    fmt.Println("Nome:", nome)

    // Exemplo 3: Inicializando uma variável float
    altura := 1.75
    fmt.Println("Altura:", altura)
}
```

Observação: O operador `:=` não pode ser usado para reatribuir valores a variáveis já declaradas.


## Exercício 
1. Replique os exemplos mencionados no resumo e brinque com eles. Tente criar novas variáveis e atribuir valores a elas. Tente também reatribuir valores a variáveis já declaradas.
2. Faça uma aplicação que receba 2 números do usuário e imprima a soma deles. Utilize a função `fmt.Scanln()` para receber os números do usuário.
