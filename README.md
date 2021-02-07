## Tic Tac Toe Random

A Tic Tac Toe Random Algorithm NPM module in typescript to find random index on a given board 

![Node.js CI](https://github.com/chokonaira/tictactoe-minimax/workflows/Node.js%20CI/badge.svg)

### NPM Package

[NPM Random](https://www.npmjs.com/package/tictactoe-random)


### Installation

#### Random Module

`npm install tictactoe-random --save`

#### [Board Module](https://github.com/chokonaira/tictactoe-board)

`npm install tictactoe-board --save`

#### Usage

`import Random from 'tictactoe-random'`

`import Board from 'tictactoe-board'`



#### Intialize an instance object of the Random and Board 

```
const board = new Board();

const random = new Random(board);
```

You can pass in an `optional` custom Array of Strings as parameter to the Board
```
Example:
 
board = new Board(['X', 'X', '', '', 'O', 'O', '', '', ''])

now board.grid = ['X', 'X', '', '', 'O', 'O', '', '', '']

instead of default grid = ['', '', '', '', '', '', '', '', '']
```

### Method

### `random.findRandomMove(board)`

This returns the best winning index of the given board
```
Example sceenerio:

const baord = new Board();

random.findRandomMove(board) = random index

This means position on the board is a random index from the available board index's 
