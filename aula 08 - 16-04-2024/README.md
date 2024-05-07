# Vetores ( ou array)
Em Go, vetores (ou arrays) são estruturas de dados que permitem armazenar um conjunto fixo de elementos do mesmo tipo. Eles são como listas ordenadas de informações. Vou explicar de forma simples:
## Vetores (Arrays):
- São coleções de dados com tamanho fixo.
- Todos os elementos de um vetor devem ser do mesmo tipo.
- A memória para um vetor é alocada apenas uma vez.
- Ótimo para situações em que você sabe exatamente quantos elementos precisa.
- Por exemplo, um vetor de notas de alunos com 10 posições:`[7.5, 8.0, 6.5, ...]`.

## Fatias (Slices):
- São como versões flexíveis de vetores.
- Permitem variação de comprimento.
- Mais versáteis e amplamente usadas em Go.
- Por exemplo, uma fatia de números inteiros: `[]int{1, 2, 3, ...}`.


# Inicializando um Vetor(Array)
```go
var meuVetor [5]int
meuVetor = [5]int{10,20,30,40,50}
// ou você pode atribuir os valores a cada índice (posição)
meuVetor[0] = 10
meuVetor[1] = 20
meuVetor[2] = 30
meuVetor[3] = 40
meuVetor[4] = 50
```

# Inicializando uma Fatia(Slice)
```go
minhaFatia := []int{1, 2, 3, 4, 
5}
minhaFatia[0] = 10
minhaFatia[1] = 20
minhaFatia[2] = 30
minhaFatia[3] = 40
minhaFatia[4] = 50
minhaFatia[5] = 60
```
## Função len
A função `len()` em Go é usada para retornar o tamanho (ou quantidade de elementos) de uma coleção de dados, como um vetor, fatia, mapa, string ou canal.

## Função range
A função `range()` em Go é usada para iterar sobre elementos em uma variedade de estruturas de dados, como vetores, fatias, strings, mapas ou canais.

# Exemplos
## Percorrendo um vetor ou fatia
```go
for i := 0; i < len(meuVetor); i++ {
    fmt.Println(meuVetor[i])
}
```


## Percorrendo um vetor ou fatia com range
```go
for i, valor := range meuVetor {
    fmt.Println(i, valor)
}
```

## Percorrendo um vetor ou fatia com range ignorando o índice
```go
for _, valor := range meuVetor {
    fmt.Println(valor)
}
```

## Percorrendo um vetor ou fatia com range ignorando o valor
```go
for i := range meuVetor {
    fmt.Println(i)
}
```

## Percorrendo um vetor ou fatia com range ignorando o valor
```go
for i := range meuVetor {
    fmt.Println(i)
}
```

## Percorrendo um vetor ou fatia com range ignorando o valor
```go
for i := range meuVetor {
    fmt.Println(i)
}
```

## Percorrendo um vetor ou fatia com range ignorando o valor
```go
for i := range meuVetor {
    fmt.Println(i)
}
```