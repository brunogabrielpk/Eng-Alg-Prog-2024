# Resumo da aula 

Primeiramente eu gostaria de agradecer ao feedback de todos. 
Acredito que essa ideia de montar um diário das aulas e disponibilizar on-line tenha sido uma ideia agradável.

Sempre que possível vou atualizar as páginas aqui e também tentar deixar links úteis,
assim como os exercícios para serem resolvido em casa.

## Exercícios
### exercício 01 - Faça seu próprio Hello World
Eu presumo que você já instalou o editor VScode e a linguagem de programção GoLang

Agora é hora de replicar o que foi feito em sala de aula e criar o seu hello world.


Crie uma pasta com o nome hello-world (o nome da pasta em si não é tão importante, pode mudar se desejar)

se você quiser usar o terminal(Windows PowerShell) para criar a pasta use o comando abaixo:
```
mkdir hello-world

```

com isso a pasta será criada. 
Se você tem dificuldade usando o terminal, vou deixar aqui uns comandos bem básicos.
para saber onde você se encontra, utilize o comando abaixo:
```
pwd

```
pwd é um sigla para "Print Work Directory". Ele vai mostrar a pasta onde o seu terminal se encontra.

Para listar o coteúdo da pasta onde você se encontra, utilize o comando: 
```
ls

```
ls, abreviação de "list" vai listar todos os arquivos e pastas que estão na pasta onde você se encontra.

Nesse momento, se você usou o mkdir ali em cima, a pasta hello-world deve estar listada.

Portanto, nos resta agora adentra essa pasta. o comando para entrar na pasta é o comando `cd`:
```
cd hello-world
```
Para confirmar que você entrou na pasta, utilize o comando `pwd` novamente.

A partir de agora já pode usar o comando `go mod init`:
```
go mod init hello-world
```
Se você usou outro nome para sua pasta, ao usar o `go mod init` você deve substituir o hello-world no comando acima pelo nome da sua pasta.

Agora você está pronto para montar o código do seu hello world. 
Abra essa pasta onde você se encontra no Vscode. 
O Vscode possibilita que você crie arquivos, portanto crie um arquivo nessa pasta com o nome `main.go`
Então, preencha esse arquivo com o código do seu hello-world:
```
package main

import "fmt"

func main() {
	fmt.Println("Hello, World")
}
```
Ótimo, vc escreveu o seu primeiro programa.
Mas ainda precisa testar ele. 

Lembre-se, que o Go é uma linguagem compilada. 
Isso que dizer que é necessário converter esse arquivo em um arquivo binário para que o seu sistema operacional possa executá-lo.

Para fazer isso, volte ao terminal e use o comando abaixo para criar o arquivo binário:
```
go build main.go
```
Com isso, deve ser criado na pasta um arquivo com o nome main.exe.
Esse arquivo é executável
No terminal, utilize o comando abaixo para executar esse arquivo:
```
./main.exe
```
Com isso o seu programa deve ser executado :) 

### Execício 02
Ao criar o nosso primeiro programa, nós utilizamos a função `fmt.Println` para imprimir texto tela.
Porém, essa não é a única função que faz isso. Dentre outras, também temos a `fmt.Printf`.
Então, para esse exercício, pesquise pelas diferenças entra as funções `fmt.Println` e `fmt.Printf` e tente fazer um
hello world usando o `fmt.Printf`.




