# C Chess Engine

An original Chess engine written in C, inspired by Dr. Robert Hyatt's "Crafty". The project explores classical chess engine design and optimization techniques, supporting both console play and GUI integration.

## Features

✅ 120-square array board representation  
✅ Bitboard data structures for fast move generation  
✅ Alpha-Beta pruning with Quiescence search  
✅ MVV/LVA move ordering, killer move heuristic, and history table  
✅ Zobrist hashing for position tracking  
✅ Polyglot opening book support  
✅ Two supported communication protocols (WinBoard/XBoard, custom CLI)

## Technical Overview

### Board Representation

- **120-square mailbox** layout to simplify edge detection.
- Core board operations are optimized using bitboards for each piece type.

### Search

- Recursive **Alpha-Beta pruning** engine
- **Quiescence search** to avoid horizon effect
- Move ordering via **MVV/LVA**, **killer heuristic**, and **history tables**

### Hashing

- Implements **Zobrist hashing** with hash tables
- Supports **FEN-based position lookups** for fast state recovery

### Communication Protocols

- Compatible with **WinBoard** and other GUI protocols
- Also playable via terminal for debugging/testing

## Build Instructions

```sh
make
./chess_engine
