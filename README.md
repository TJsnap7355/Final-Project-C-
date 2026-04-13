## Intro

This is a Casino program in C++ for a Programming 1 final
I hope that these games and future additions are enjoyable for whoever finds them
My aim for this program is for an offline interactive expeince that engages users cognitive functions


[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/TJsnap7355/Final-Project-C-/badge)](https://securityscorecards.dev/viewer/?uri=github.com/TJsnap7355/Final-Project-C-)

[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/12459/badge)](https://bestpractices.coreinfrastructure.org/projects/12459)
[![OpenSSF Best Practices](https://www.bestpractices.dev/projects/12459/badge)](https://www.bestpractices.dev/projects/12459)

## Overview

This project is a simple console-based casino game written in C++. It was created as a Programming 1 final project and is designed to be easy to run and easy to play. The program gives the player a starting chip count, lets them choose between multiple card games, updates chips based on wins and losses, and saves the final result when the session ends.

The game currently includes:
- Blackjack
- Casino War

The program is fully offline and uses standard console input and output.

## Features

- Text-based casino menu
- Player name input at startup
- Starting balance of 1000 chips
- Playable Blackjack mode
- Playable Casino War mode
- Input validation for menu choices and wagers
- Automatic card deck creation and shuffling
- Chip tracking across the play session
- Saves the player name and final chip count to `casino_results.txt`

## Description

### Blackjack
In Blackjack, the player places a wager, receives cards, and chooses whether to hit or stand. Face cards count as 10, aces can adjust from 11 to 1 when needed, and the dealer draws until reaching at least 17.

### Casino War
In Casino War, the player and dealer each draw one card. The higher card wins the round. If both cards are equal, the round ends in a draw.

## Project Structure

- `main.cpp` — program entry point and main casino menu
- `blackjack.cpp` — Blackjack game logic
- `casino_war.cpp` — Casino War game logic
- `carddeck.cpp` / `carddeck.h` — card and deck handling
- `player.h` — player data structure
- `games.h` — function declarations for game modes
- `CMakeLists.txt` — build configuration

## How to Run

### Option 1: Build with CMake

```bash
mkdir build
cd build
cmake ..
cmake --build .
./Final_Project_C_
