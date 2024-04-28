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
- [1] - Cadastrar pessoas
- [2] - Pesquisar pessoa
- [3] - listar todas pessoas
- [e] - Sair do programa
- [R] - Resetar a base de dados

## [1] - Cadastrar usuário
Como o nome diz, esta opção vai cadastrar usuários.
Uma vez selecionada esta opção, será solicitado ao usuário que digite os itens.
Verifique cada entrada do usuário pois itens obrigatórios não podem ser aceitos com entradas vazias ('').

Se o usuário não fornecer um item obrigatório, mostre uma mensagem de erro e retorne ao menu.
Se todos os dados forem corretos, salve a pessoa e mostre uma mensagem de sucesso ao usuário.

Após isso retorne ao menu.

## [2] - Pesquisar pessoa
Se não houver nenhuma pessoa cadastrada ainda, o programa deve mostrar uma  mensagem de informado que não há pessoas cadastrdas e depois deve retornar ao menu.
Se houver pessoas cadastradas, pede para o usuário fornecer qual campo ele deseja pesquisar (nome, endereço,...).

Deverá se pedido ao usuário que forneça o valor exato a ser pesquisado e após isso, realizar pesquisa.
Se o valor solicitado for encontrado, mostrar todos dados na tela da pessoa e retorna ao menu.
Caso contrário, menssagem de não possível encontrar e retornar ao menu.

## [3] - listar todas pessoas
Se não houver nenhuma pessoa cadastrada ainda, mostrar menssagem de cadastro vazio e retornar ao menu.
Se houver, lista todas as pessoas na tela.

## [e] - Sair do programa
Pede para o usuário confirmar se quer sair mesmo.
Caso afirmativo, mostra mensagem de despedida e encerra o aplicativo.
Senão, volta para o Menu.

## [R] - Resetar a base de dados
Pede para o usuário confirmar que é isso que ele quer mesmo.
Caso afirmativo, apaga todos os usuários e retorna ao menu.
Caso negativo, apenas retorna ao menu.