# React GraphQL Pokédex App
This is a simple React application that fetches data from the Pokémon GraphQL API and displays information about Pokémon. The app is built using React, Apollo Client for GraphQL integration, and styled with CSS.

## Features
Displays basic information about Pokémon such as name, image, maximum HP, maximum CP, and special attacks.
Utilizes Apollo Client for fetching data from the GraphQL API.
Dynamically renders Pokémon data in a responsive layout.
Prerequisites

## Before running the application, make sure you have the following installed:

Node.js
npm or yarn package manager

## Installation

Clone this repository:
```bash
cd react-graphql-pokedex
```

Navigate to the project directory:
```bash
cd react-graphql-pokedex
```
Install dependencies:
```bash
npm install
# or
yarn install
```






## Usage
Start the development server:

```
npm start
or
yarn start
```

## GraphQL Query
The application sends a GraphQL query to fetch Pokémon data. The query is defined in the GET_POKEMONS constant in get-pokemons.js file.

```
query pokemons($first: Int!) {
    pokemons(first: $first) {
        id
        name
        image
        maxHP
        maxCP
        attacks {
            special {
                name
                damage
            }
        }
    }
}

```
## License

[MIT](https://choosealicense.com/licenses/mit/)
