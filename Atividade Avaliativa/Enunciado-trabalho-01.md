# Atividade Avaliativa - Modelo 01

Crie um aplicativo em Go(lang) que faça o que se pede abaixo.

## Contexto
A ideia aqui é cadastrar e consultar pessoa
Uma pessoa deve possuir:
- Nome*
- Sobrenome
- Idade* 
- Endereço* 
- Email 
- Telefone 
- Time de futebol*
Os itens marcados com * são itens obrigatórios.

## Primeiramente, o Menus de opções
O programa deve começar mostrando um menu na tela bem bonito com as
seguintes opções:
[1] - Cadastrar pessoas
[2] - Pesquisar pessoa
[3] - listar todas pessoas
[e] - Sair do programa
[R] - Resetar a base de dados

## [1] - Cadastrar usuário
Como o nome diz, esta opção vai cadastrar usuários.
um vez selecionada ela vai pedindo para o usuário digitar os itens.
Verifique cada entrada do do usuário pois itens obrigatórios não podem aceitar entradas vazias.
Se o usuário não fornecer um item obrigatório, mostre uma mensagem de erro e retorne ao menu.
Se todos os dados forem corretos, salve a pessoa e mostre uma mensagem de sucesso ao usuário.
após isso retorne ao menu.

## [2] - Pesquisar pessoa
Se não houver nenhum cadastro ainda, mostra menssagem de cadastro vazio e retorna ao menu.
Se houver pessoas cadastradas, pede para o usuário fornecer qual campo ele deseja pesquisar (nome, endereço,...)
Pede pro usuário fornecer o valor exato a ser pesquisado e realiza pesquisa.
Se encontrar, mostrar todos dados na tela da pessoa e retorna ao menu.
Caso contrário, menssagem de não possível e retorn ao menu.
## [3] - listar todas pessoas
Se não houver nenhum cadastro ainda, mostra menssagem de cadastro vazio e retorna ao menu.
Se houve, lista todas as pessoas na tela.

## [e] - Sair do programa
Pede para o usuário confirmar se quer sair mesmo.
Caso afirmativo, mostra mensagem de despedida e encerra o aplicativo.
Senão, volta para o Menu.

## [R] - Resetar a base de dados
Pede para o usuário confirmar que é isso que ele quer mesmo.
Caso afirmativo, apaga todos os usuários e retorna ao menu.
Caso negativo, apenas retorna ao menu.