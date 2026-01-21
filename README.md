# Memory Light Game

## Website
[Memory Light Game](https://nkachalia1.github.io/Memory-Light-Game/)

## Description

Welcome to **Memory Light Game**, a browser-based interactive memory challenge inspired by the classic Simon game. Players must observe and repeat an increasingly long sequence of colored lights and sounds. The game tests memory, focus, and reaction speed, with a strict mode for added difficulty.

## Instructions

1. **Power On**: Toggle the power switch to ON.
2. **Start Game**: Press the START button to begin.
3. **Watch the Sequence**: The game will flash a sequence of colored lights with corresponding sounds.
4. **Repeat the Sequence**: Click the colored panels in the same order.
5. **Advance Levels**: Each round adds a new step to the sequence.
6. **Strict Mode (Optional)**: Enable STRICT mode to restart the game immediately after a mistake.

## Features

- **Interactive Game Board**: Four colored quadrants that light up and play tones.
- **Progressive Difficulty**: Sequence speed increases as the count grows.
- **Strict Mode**: Mistakes reset the game for an added challenge.
- **Visual Feedback**: LED-style counter displays the current step count.
- **Audio Feedback**: Web Audio API–generated tones for each color and error states.
- **Win Condition**: Successfully complete 20 steps to win the game.

## Usage

### Home Screen
<p align="center">
  <img src="home.png" width="400" alt="Memory Light Game – Home Screen">
</p>
Displays the game board, counter, control buttons, and power switch.

### Gameplay Preview
<p align="center">
  <img src="gameplay.gif" width="600" alt="Memory Light Game – Gameplay">
</p>
The game highlights each color in sequence. Players must repeat the exact pattern to continue.

### Strict Mode

When enabled, any incorrect input immediately restarts the game from the beginning.

*Alt text: Strict mode LED enabled*

## Technical Details

Memory Light Game is built using:

- **Languages**: JavaScript, HTML, CSS
- **Libraries**: jQuery
- **APIs**: Web Audio API for sound generation
- **Tools**: Git, GitHub, VS Code

## Feature Implementation

### Audio Generation

Each color uses an oscillator node with a unique frequency:

```js
var frequencies = [329.63, 261.63, 220, 164.81];
