# Struct

Nós já vimos variáveis, vetores e fatias (slices)
As structs, a grosso modo, são estruturas para agrupar esses itens
mencionados anteriormente.


Vamos pular direto para um exemplo.
Digamos que eu queira cadastrar 10 carros
e suponha que um carro tenha as seguintes características:
- Modelo (Uno, Pálio, Gol)
- Marca (Fiat, Tesla, Ford)
- Cor (Verde, Azul, Amarelo)

Eu poderia criar 3 vetores, um para cada característica:
- var carroModelo [10]string
- var carroMarca [10]string
- var carroCor [10]string

Após isso eu poderia fazer um loop (for) e pedir para o usuário
inserir os dados de cada carro e armazena-los sequencialmente.
Assim, por exemplo, você poderia acessar todas informações de cada carro
baseado na posição dos dados nos vetores: carroModelo[2], carroMarca[2],
carroCor[2], para acessar os dados do terceiro carro 
(lembrarModelo que começa em 0 a indexação)

Ok, isso aí pode tem funcionar mas tem sérias chances de dar errado.
Desse jeito, é melhor usar structs

Abaixo um exemplo
```go
package main

import "fmt"


type Carro struct{
  Modelo string 
  Marca string
  Cor string
}


func main(){
  var entrada string
  var carros []Carro
  for{
    fmt.Println("Deseja cadastrar um carro")
    fmt.Println("Digite sim para cadastrar ou qualquer outra coisa para sair")
    fmt.Scanln(&entrada)
    if entrada == "sim" {
      carro := Carro{}
      fmt.Println("Digite o modelo do carro")
      fmt.Scanln(&carro.Modelo)
      fmt.Println("Digite a marca do carro")
      fmt.Scanln(&carro.Marca)
      fmt.Println("Digite o Cor do carro")
      fmt.Scanln(&carro.Cor)

      carros = append(carros, carro)
    } else {
      break
    }
  }
  
  fmt.Println("Lista de carros")
  for _, carro := range carros{
    fmt.Println("Modelo: ", carro.Modelo)
    fmt.Println("Marca: ", carro.Marca)
    fmt.Println("Cor: ", carro.Cor)
  }

}

```
O código pode ser longo mas vamos com calma

Lá no começo eu declarei a struct usando a palavra `type`
`type` significas tipo. Ela sere para criar tipos de variáveis 
(int, float64 e string são tipos de variáveis). Embora outros tipos de variáveis possam
ser criadas, vamo só foca no tipo `struct`.

Portanto, eu declarei a struct usando 
`type Carro struct`. Ou seja, eu pedi ao compilador do golang
para "criar" essa estrura chamada Carro.

Logo em seguida eu defino o "corpo" (ou atributos) da `struct`
```go
type Carro struct{
  Modelo string 
  Marca string
  Cor string
}
```
Assim, ficou definido que minha struct tem 3 atributos (Modelo, Marca e Cor).
Uma vez definida essa estrutura, agora ela é parte do código e podemos então
declarar variáveis desse tipo dentro do código.

No meu exemplo eu já fui direto declarando uma slice de carros
```go
  var carros []Carro
```
Ou seja, um coleção de de carros.

depois disso eu pergunto se o usuário deseja cadastrar um carro.
Se ele disse sim, eu declaro um variável do tipo carro
```go
carro := Carro{}
```

Aqui as coisa ficam um pouco confusas. mas calma que tudo tem explicação.
`carro` é o nome da variável que criei do tipo Carro ( carro é nome e Carro é tipo, coloquei inicial 
maiúscula no tipo e minúscula no nome para ficar melhor de diferenciar. Recomendávels mas não
obrigatório).

Eu poderia ter digitado `var carro Carro`
Em ambos casos eu estaria inicializando uma variável de carro vazia.

Então, eu peço para o usuário ir digitando os dados do carro e note que para
cada item eu já uso um fmt.Scanln direto para o atributo.
A sintaxe do ponto (.) me permite acessar os atributos como fiz ali no código, por exemplo
em `fmt.Scanln(&carro.Modelo)` a leitura da entrada do usuário foi direcionada diretamente
ao atributo Modelo da variável carro.

Embora eu não tenha utilizado isso, mas também é possível já inicializar um struct já
com valores nas propriedades.
Seria algo assim (considerando a mesma struct)
```go
carro := Carro{Modelo: "Uno", Marca: "Fiat", Cor: "verde"}
```
Ou até mesmo assim
```go
carro := Carro{"Uno", "Fiat", "verde"}
```


Continuando o exemplo, após inicializada e "preenchida", eu então anexo a variável de nome carro
a slice de nome carros usando o comando `append`
`carros = append(carros, carro)`

Por fim, quando o usuário termina de cadastrar os carros, eu mostro todos os resultados
iterando sobre todos os valores armaedos na slice carros:
```go
fmt.Println("Lista de carros")
  for _, carro := range carros{
    fmt.Println("Modelo: ", carro.Modelo)
    fmt.Println("Marca: ", carro.Marca)
    fmt.Println("Cor: ", carro.Cor)
  }
```


Bom, esse é o basicão. Mas já é suficiente para ajudar na confecção do trabalho :)

Disclaimer: Depois eu corrijo os erros de português, o importante é que o código já está aí
para a turma possa utilizar.
