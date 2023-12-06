<p align="center">
  <a href="https://github.com/wnhedaxx/venom-blockchain.github.io">
    <img src="https://avatars.githubusercontent.com/u/70830772?s=400&u=2ed023fa0865132977919170696b9503aa8a2107&v=100" alt="Logo" width="1024" height="1024">
 <h1># degods.venom

Hello everyone, twitter id oxdoxo
</h1> </a>
</p>
#GAME
<!-- # ⭕ Tic-Tac-Toe -->

[//]: # (<img alt="workshop/tictactoe" width="1412" src="../.resources/tictactoe.png">)

<marquee>A standard game of Tic-Tac-Toe in venom.</marquee>

⭕ ❕ ⭕ ❕ ❌

➖ ➕ ➖ ➕ ➖

⭕ ❕ ⁣❌ ❕ ⭕

➖ ➕ ➖ ➕ ➖

❌ ❕ ❌ ❕ ⭕

## Representing State
venom allows users to define composite data types with the `struct` keyword. 
The game board is represented by a struct called `Board`, which contains three `Row`s.
An alternative representation would be to use an array, however, these are not yet supported in venom.

## Language Features
- `struct` declarations
- conditional statements
- early termination. Leo allows users to return from a function early using the `return` keyword.

## Running the Program

venom provides users with a command line interface for compiling and running Leo programs.
Users may either specify input values via the command line or provide an input file in `inputs/`.

### Providing inputs via the command line.
1. Run 
```bash
venom run <function_name> <input_1> <input_2> ...
```
See `./run.sh` for an example.


### Using an input file.
1. Modify `inputs/tictactoe.in` with the desired inputs.
2. Run
```bash
venom run <function_name>
```

## Executing the Program
```bash
venom execute <function_name> <input_1> <input_2> ...
```

## Playing the Game

### 1. Create a new game board
```bash
venom run new
```
|   |   |   |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 0 | 0 |
| 0 | 0 | 0 |

### 2. Player 1 makes a move
```bash
venom run make_move 1u8 1u8 1u8 "{ r1: { c1: 0u8, c2: 0u8, c3: 0u8 }, r2: { c1: 0u8, c2: 0u8, c3: 0u8 }, r3: { c1: 0u8, c2: 0u8, c3: 0u8 } }"
```
|   |   |   |
|---|---|---|
| 1 | 0 | 0 |
| 0 | 0 | 0 |
| 0 | 0 | 0 |

### 3. Player 2 makes a move
```bash
venom run make_move 2u8 2u8 2u8 "{ r1: { c1: 1u8, c2: 0u8, c3: 0u8 }, r2: { c1: 0u8, c2: 0u8, c3: 0u8 }, r3: { c1: 0u8, c2: 0u8, c3: 0u8 } }"
```
|   |   |   |
|---|---|---|
| 1 | 0 | 0 |
| 0 | 2 | 0 |
| 0 | 0 | 0 |
# venom
# is
# love


# The Venom Knowledge Base

## Table of Contents

- [About](#about)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## About
This website serves as [the official documentation](https://docs.venom.foundation/) for the Venom Blockchain. Here, you can find guides, tutorials, and documentation to help you get started with building on the Venom Blockchain. 

## Getting Started

To get started with the Venom Blockchain, you can visit the [official website](https://venom.foundation/) for more information. You can also join our [community chat](https://discord.venom.foundation/dev) to connect with other developers and ask questions.

## Usage

### Local Development

This website is built using [Docusaurus 2](https://docusaurus.io/), a modern static website generator.

### Installation

```
$ yarn
```

### Run

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

## Contributing

We welcome contributions to the The Venom Knowledge Base! If you notice any issues or errors, feel free to open an issue or submit a pull request.

## License

This project is licensed under the CC-BY-SA-4.0 License - see the [LICENSE](LICENSE) file for details.
