# Desafio 10

Décimo desafio do curso GoStack da Rocketseat.

## Descrição

Nesse desafio, você irá desenvolver mais uma aplicação, a GoRestaurant. Agora você irá praticar o que você aprendeu até agora no React.js junto com TypeScript, praticando o conceito de CRUD (Create, Read, Update, Delete).

Essa será uma aplicação que irá se conectar a uma fake API, e exibir os pratos de comida criados e permitir a criação, remoção e atualização desses pratos.

## Fake API

Os dados dos pratos a serem exibidos em tela foram disponibilizados junto ao template da aplicação, em uma fake API.

Para isso, foi instalado no  package.json uma dependência chamada json-server, e um arquivo chamado server.json que contém os dados para uma rota /foods. Para executar esse servidor execute o seguinte comando:

  `yarn json-server server.json -p 3333`

## Funcionalidades da aplicação

Com o template clonado e pronto para continuar, você deve verificar os arquivos da pasta src e completar onde não possui código, com o código para atingir os objetivos de cada rota.

-   [x] **`Listar os pratos de comida da sua API`**: Sua página `Dashboard` deve ser capaz de exibir uma listagem, com o campo `title`, `value`, `description` e `available` de todos os pratos de comida que estão cadastrados na sua API.

**Dica**: Para exibir se o prato de comida está disponível ou não, você pode validar o campo available que é retornado da API e exibir `Disponível` caso seja true, e `Indisponível` caso seja false.

-   [x] **`Adicionar novos pratos de comida a sua API`**: Em sua página Dashboard você deve abrir um modal ao clicar no botão `Novo Prato` no Header. Esse modal deve ser responsável por cadastrar uma nova food passando os campos `image`, `name`, `description`, `value`.

**Dica 1**: O campo image deve ser uma URL, deixamos três URL de imagens como exemplo no arquivo server.json.

**Dica 2**: Ao enviar o request para sua API para salvar a `food`, lembre-se sempre de setar o campo `available` como true.

-   [x] **`Editar pratos de comida da sua API`**: Em sua página Dashboard você deve abrir um modal ao clicar no botão `Editar Prato`. Esse modal deve ser responsável por editar uma `food` passando os campos `image`, `name`, `description`, `value`.

**Dica**: Ao editar um item, quando for envia-lo para o backend, lembre de copiar os dados anteriores como o `available` e o `id`, ou eles serão perdidos do seu arquivo server.json.

-   [x] **`Remover pratos de comida da sua API`**: Em sua página Dashboard você deve remover um prato de comida ao clicar no botão com ícone de lixeira no componente Food.

**Dica**: Após remover o item da sua API, lembre-se de remover ele também da listagem.

-   [x] **`Alterar disponibilidade dos pratos de comida da sua API`**: Em sua página Dashboard você deve alterar a disponibilidade de um prato de comida ao clicar no switch que é controlado pelo valor de `available`.

## Testes

-   [x] **`should be able to list all the food plates from your api`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados, toda os pratos de comidas que são retornadas da sua fake API.

-   [x] **`should be able to add a new food plate`**: Para que esse teste passe, você deve permitir que um prato de comida seja adicionado a sua api, adicionando-o também à listagem.

-   [x] **`should be able to edit a food plate`**: Para que esse teste passe, você deve permitir que um prato de comida seja editado na sua api, editando-o também na listagem.

-   [x] **`should be able to remove a food plate`**: Para que esse teste passe, você deve permitir que um prato de comida seja removido da sua api, removendo-o também da listagem.

-   [x] **`should be able to update the availibility of a food plate`**: Para que esse teste passe, em sua dashboard você deve permitir que o status do prato de comida seja alterado entre `Disponível` e `Indisponível`;

---

*Este repositório teve como base um template disponibilizado pela equipe da rocketSeat.
