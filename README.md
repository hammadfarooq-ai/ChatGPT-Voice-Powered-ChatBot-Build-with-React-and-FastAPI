# React Betting Game

A simple betting simulation game built with React, TypeScript, and Tailwind CSS. Users can place bets on whether a random number will be high (≥50) or low (<50).

## Features

- 🎲 Random number generation using random.org API
- ⬆️⬇️ Up/Down betting direction selection
- 🎯 Win/Loss result display
- ⚡ Built with Vite for fast development
- 🎨 Styled with Tailwind CSS

## How It Works

1. Select your bet direction (Up or Down)
2. Click "Place Bet" button
3. A random number (1-100) is fetched from random.org API
4. **Win conditions:**
   - If number ≥ 50 and you bet "Up" → **WINNER** ✅
   - If number < 50 and you bet "Down" → **WINNER** ✅
   - Otherwise → **BAD LUCK** ❌

## Tech Stack

- React 18
- TypeScript
- Vite
- Tailwind CSS
- Axios

## Installation

```bash
yarn install
```

## Development

```bash
yarn dev
```

## Build

```bash
yarn build
```

## Preview

```bash
yarn preview
```
