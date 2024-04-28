## Atividade Avaliativa - Modelo 2

## Contexto
A ideia aqui é fazer um aplicativo para auxiliar em uma oficina mecânica.

O sistema deve permitir que o usuário realize as seguintes operações:

- [1] - Cadastro de Clientes:
    - O usuário pode adicionar novos clientes à base de dados da oficina.
    - Cada cliente deve ter um nome*, telefone e endereço.
- [2] Agendamento de Serviços:
    - O usuário pode agendar serviços para os clientes.
    - Cada serviço deve ter uma descrição, data, hora e o nome do cliente.
- [3] - Controle de Estoque:
    - O usuário pode adicionar e remover peças do estoque.
    - Cada peça deve ter um nome, quantidade e preço.
- [4] - Relatórios:
    - O usuário pode gerar relatórios com informações sobre os clientes, serviços agendados e estoque.


## menu
Um menu deverá ser exibido para o usuário com as 4 opções mencionadas acima.
além disso deverá conter mais um opção para sair do aplicativo.

### [1] - Cadastro de cliente
Ao escolher a opção o 1 o usuário deverá ser levado para a tela de cadastro do usuário.
Deve ser solicitado ao usuário que digite os dados do Cliente. O nome é obrigatório.
Ao final o Cliente deve ser salvo e o programa deve perguntar para o usuário se ele deseja
cadastrar mais um cliente.
Se ele responder afirmativamente, repita o processo.
Se não, retorne ao menu inicial.


### [2] - Cadastro de Atendimento
Ao escolher essa opção, ao usuário será solicitado a cadastrar um novo atendimento.
A primeira informação a ser solicitada é o nome do cliente.
Se não houver um cliente cadastrado com o nome fornecido, o programa deverá mostrar
uma mensagem de erro e retornar ao menu principal.
Caso exista um cliente com esse nome cadastrado, o programa deve solicitar a descrição
 a data e a hora para o usuário, então salvar o atendimento e retornar ao menu.

### [3] - Cadastro de Estoque
Esta opção deverá cadastrar peças.
A primeira informação a ser solicitada deve ser o nome da peça.
Caso uma peça com esse nome já esteja cadastrada, o programa deve mostrar uma mensagem de error e então retornar ao menu.
Caso não haja peça com esse nome cadastrada, solicitar quantidade e preço por peça.
Salvar a peça e retornar ao menu principal.


### [4] - Relatório
Ao selecionar essa opção o programa deverá mostrar de maneira ordenada e visualmente agradável, os clientes, os atendimentos e as peças na tela.

### [S] - Sair
Ao selecionar essa opção o programa deverá mostrar uma mensagem perguntando se o usuário deseja sair.
Caso positivo, encerre o programa.
Caso negativo, retorne ao menu principal.
