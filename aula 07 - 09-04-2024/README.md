# aula 07 - laços de repetição
Nessa aula nós trabalhmos o início dos laços de repetição.

- O laço `for` é usado quando sabemos quantas vezes queremos repetir um bloco de código.
- Ele possui a seguinte sintaxe:
```go
for inicialização; condição; incremento {
    // código a ser repetido
}
```
- Exemplo: Imprimir os números de 1 a 10
```go
for i := 1; i <= 10; i++ {
    fmt.Println(i)
}
```

- O incremento pode ser negativo, para isso basta decrementar a variável de controle.
- O incremento pode ser de mais de um, para isso basta incrementar a variável de controle com mais de um.
- O incremento pode ser omitido, para isso basta incrementar a variável de controle dentro do bloco de código.
- Exemplo:
```go
i := 1
for i <= 10 {
    fmt.Println(i)
    i++
}
```

- É possível usar o laço `for` sem condição, para isso basta omitir a condição.
- Exemplo: 
```go
i := 1
for {
    fmt.Println("Olá, mundo!")
    i++
    if i > 10 {
        break
    }
}
```
- O comando `break` é usado para sair do laço de repetição.


## Exercício
### Exercício 01
Escreva um programa em Go que solicite ao usuário um número inteiro positivo e, em seguida, faça uma contagem regressiva a partir desse número até zero. Cada número deve ser impresso na tela.

### Exercício 02
Faça um aplicativo que peça para o usuário digitar um número
entre 100 e 1000 e depois imprima todos os valores *pares* entre o número 1
e o número digitado pelo usuário.



