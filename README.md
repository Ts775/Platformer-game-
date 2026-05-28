# Platformer-game-

An endless vertical platformer built with **Python** and **Pygame** where the player jumps across moving platforms, collects coins, and climbs for the highest score possible.

---

#  Preview

Project structure:

```text id="w4u2ok"
main.py
background.png
player.png
platform.png
coin.png
```

The game includes:

* Animated scrolling gameplay
* Moving platforms
* Coin collection
* Score tracking
* Infinite procedural platform generation
* Custom sprite assets

---

#  Features

* Smooth movement physics
* Variable jump height
* Infinite scrolling world
* Random platform generation
* Moving platforms
* Coin collectibles
* Score system
* Screen wrap-around movement
* Custom graphics and background

---

#  Requirements

Install Python and Pygame:

```bash id="hn2tdm"
pip install pygame
```

---

#  Running the Game

Run the game using:

```bash id="a7o4zn"
python main.py
```

---

# 🎮 Controls

| Key           | Action     |
| ------------- | ---------- |
| ⬅ Left Arrow  | Move Left  |
| ➡ Right Arrow | Move Right |
| Space         | Jump       |
| Release Space | Short Jump |

---

#  Game Mechanics

## Player Physics

The player movement uses:

* Acceleration
* Velocity
* Friction

to create smoother and more natural movement.

```python id="qzz5gm"
self.acc.x += self.vel.x * FRIC
```

---

## Jump System

The player can only jump while standing on a platform.

Holding the jump key gives a higher jump, while releasing early creates a shorter jump.

```python id="n2vt95"
self.vel.y = -15
```

---

## Infinite Scrolling

When the player reaches the upper third of the screen:

* Platforms move downward
* Coins move downward
* Old objects are removed
* New platforms are generated

This creates an endless climbing effect.

---

## Moving Platforms

Some platforms move horizontally across the screen.

If the player stands on a moving platform, they move together with it.

```python id="e6g5j9"
P1.pos += (self.speed, 0)
```

---

## Coins & Scoring

Coins spawn above stationary platforms.

Collecting a coin gives:

```text id="hj8k8m"
+5 points
```

Additional points are earned by surviving and climbing higher.

---

#  Code Structure

## Classes

### `Player`

Handles:

* Movement
* Jumping
* Gravity
* Collision detection
* Score tracking

---

### `Platform`

Handles:

* Random platform spawning
* Horizontal movement
* Coin spawning

---

### `Coin`

Handles:

* Coin rendering
* Collision detection
* Score rewards

---

#  Assets

The project uses custom image assets:

| File             | Purpose          |
| ---------------- | ---------------- |
| `background.png` | Background image |
| `player.png`     | Player sprite    |
| `platform.png`   | Platform sprite  |
| `coin.png`       | Coin collectible |

---

#  Game Over

The game ends when the player falls below the screen.

A red screen briefly appears before the application closes.

---

#  Concepts Used

This project demonstrates:

* Object-Oriented Programming (OOP)
* Pygame sprites
* Collision detection
* Physics simulation
* Procedural generation
* Game loops
* Sprite rendering
* Scrolling camera systems

---

#  Possible Improvements

Ideas for future upgrades:

* Sound effects 
* Main menu 
* High score saving 
* Enemy mobs 
* Power-ups 
* Double jump 
* Particle effects 
* Animated sprites 
* Mobile support 

---

# 🛠️ Built With

* Python
* Pygame


