# Aplicativo Web Pokédex

Este é um simples aplicativo web que simula uma Pokédex, exibindo informações sobre diversos Pokémon. O aplicativo obtém dados de uma API de Pokémon e os apresenta em um layout em forma de grade. Os usuários têm a possibilidade de carregar mais Pokémon à medida que percorrem a lista.

## Funcionalidades

- Exibição de uma lista de Pokémon com seus respectivos números, nomes, tipos e imagens.
- Filtragem de Pokémon de acordo com seus tipos, com a aplicação de diferentes cores de fundo.
- Carregamento de mais Pokémon quando o final da lista é alcançado.

## Tecnologias Utilizadas

- **HTML**: Estrutura da página web.
- **CSS**: Estilo da página e das entradas dos Pokémon.
- **JavaScript**: Interação e obtenção de dados.
- **[Normalize.css](https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css)**: Reset CSS para renderização consistente.
- **Google Fonts** ([Fira Code](https://fonts.google.com/specimen/Fira+Code), [Roboto](https://fonts.google.com/specimen/Roboto)): Utilizadas para tipografia.
- **[PokéAPI](https://pokeapi.co/)**: API que provê dados de Pokémon.

## Como Utilizar

1. Clone este repositório para sua máquina local.
2. Abra o arquivo `index.html` em um navegador web.
3. Role a página para ver a lista de Pokémon e suas informações.
4. Clique no botão "Carregar Mais" no final para carregar mais Pokémon.

## Estrutura do Código

- **index.html**: Estrutura HTML principal da página web.
- **styles/**: Diretório contendo arquivos CSS para estilização do aplicativo.
  - `global.css`: Estilos globais para todo o aplicativo.
  - `pokedex.css`: Estilos específicos para a seção da Pokédex.
- **scripts/**: Diretório contendo arquivos JavaScript para interatividade e obtenção de dados.
  - `pokemon-model.js`: Modelo básico de dados para Pokémon.
  - `poke-api.js`: Funções para obtenção de dados de Pokémon da API.
  - `main.js`: Lógica principal para renderização de Pokémon e interações.

## Funcionamento

1. O aplicativo inicia carregando um conjunto inicial de Pokémon usando a função `loadPokemonItems`, que obtém dados da API de Pokémon utilizando funções da `pokeApi`.
2. Os dados dos Pokémon obtidos são dinamicamente adicionados à página web, onde cada Pokémon é representado por um elemento `<li>` com estilos apropriados.
3. Os tipos de Pokémon são utilizados como classes CSS para aplicar cores de fundo diferentes com base no tipo.
4. O botão "Carregar Mais" permite aos usuários obter e exibir Pokémon adicionais conforme rolam pela lista. Quando todos os Pokémon são carregados, o botão é removido.

## Agradecimentos

- Este projeto utiliza dados da **[PokéAPI](https://pokeapi.co/)**, uma API abrangente de Pokémon.
- A estilização da página é baseada no **[Normalize.css](https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css)** e nas fontes do **Google Fonts** ([Fira Code](https://fonts.google.com/specimen/Fira+Code), [Roboto](https://fonts.google.com/specimen/Roboto)).
- O JavaScript gerencia a obtenção de dados e a renderização das informações dos Pokémon.

Sinta-se à vontade para usar e modificar este projeto como ponto de partida para criar sua própria aplicação web de Pokédex!
