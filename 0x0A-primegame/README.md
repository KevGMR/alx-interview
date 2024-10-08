# 0x0A. Prime Game

## Tasks
### [0. Prime Game](./0-prime_game.py)

Maria and Ben are playing a game. Given a set of consecutive integers starting from `1` up to and including `n`, they take turns choosing a prime number from the set and removing that number and its multiples from the set. The player that cannot make a move loses the game.

They play `x` rounds of the game, where `n` may be different for each round. Assuming Maria always goes first and both players play optimally, determine who the winner of each game is.

- [x] Prototype: `def isWinner(x, nums)`
- [x] where `x` is the number of rounds and `nums` is an array of `n`
- [x] Return: name of the player that won the most rounds
- [x] If the winner cannot be determined, return `None`
- [x] You can assume `n` and `x` will not be larger than 10000
- [x] You cannot import any packages in this task
Example:

- [x] `x` = `3`, `nums` = `[4, 5, 1]`

First round: 4

- [x] Maria picks 2 and removes 2, 4, leaving 1, 3
- [x] Ben picks 3 and removes 3, leaving 1
- [x] Ben wins because there are no prime numbers left for Maria to choose

Second round: 5

- [x] Maria picks 2 and removes 2, 4, leaving 1, 3, 5
- [x] Ben picks 3 and removes 3, leaving 1, 5
- [x] Maria picks 5 and removes 5, leaving 1
- [x] Maria wins because there are no prime numbers left for Ben to choose

Third round: 1

Result: Ben has the most wins