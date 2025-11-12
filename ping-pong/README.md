# 🎮 Real-Time Ping Pong Game

This project is a **terminal-based ping pong game** developed using **Python and Pygame**.  
It introduces the fundamentals of **interactive game design**, including **object-oriented programming**, **real-time graphics**, and **player-AI interaction**.

---

## 🧩 Overview

A partially functional version of the game is provided.  
It includes the following features:

- A player-controlled paddle  
- An AI-controlled opponent paddle  
- Ball mechanics with initial collision handling  
- Live score tracking  

Your objective is to **analyze**, **collaborate with an AI assistant (ChatGPT)**, and **debug or enhance** the code to achieve a fully working version of the game.

---

## 💻 Getting Started

### Installation & Setup

1. Clone this repository or download the project folder.  
2. Ensure **Python 3.10 or later** is installed.  
3. Install the required dependencies using:

   ```bash
   pip install -r requirements.txt
   ```
4. To run the game, use:

   ```bash
   python main.py
   ```

---

## 🚀 Using ChatGPT for Assistance

When beginning, you can use this **initial LLM prompt** to understand and work on the project effectively:

```
I’m working on a real-time Ping Pong game using Python and Pygame. I have a partially working project structure. Please help me understand how the logic is organized and guide me on implementing missing features. Review any code I send to ensure it aligns with the expected behavior.
```

---

## ⚙️ Quick Start Prompts for Tasks

To help you move faster, ready-to-use prompts for each development task are provided below.  
Copy the relevant one into ChatGPT to get guided code suggestions.  
Make sure you carefully review and test the generated code before finalizing any changes — small edge cases are intentional to strengthen your debugging and reasoning skills.

---

## 🎯 Tasks to Complete

Each task must be completed **iteratively** with help from ChatGPT and your own review.

### 🧱 Task 1: Refine Ball Collision

> Problem: The ball occasionally goes through paddles at high speeds.  
> Goal: Improve accuracy of paddle-ball collision detection.

**Prompt:**
```
Help me fix ball collision in my ping pong game. The ball passes through paddles sometimes. I need to check if the ball's rectangle overlaps with paddle rectangles and reverse velocity_x when it happens. Just add the collision check right after moving the ball, that should work perfectly for high speeds.
```

---

### 🏁 Task 2: Implement Game Over Condition

> Problem: No proper game-ending logic.  
> Goal: Display a “Game Over” screen when one side reaches the target score.

**Prompt:**
```
I need a game over screen when a player reaches 5 points. Create a method that checks if either score equals 5, then display "Player Wins!" or "AI Wins!" on screen. Make sure to keep the game loop running so players can see the message. Add a small delay before closing pygame.
```

---

### 🔁 Task 3: Add Replay Option

> Problem: Game ends abruptly.  
> Goal: Allow players to restart and choose match length (best of 3, 5, or 7).

**Prompt:**
```
Add a replay feature after game over. Show options for "Best of 3", "Best of 5", "Best of 7", or "Exit". Wait for user input (keys 3, 5, 7, or ESC). When they choose, update the winning score target and reset the ball position. That should let them play again.
```

---

### 🔊 Task 4: Add Sound Effects

> Problem: No audio feedback for in-game actions.  
> Goal: Add sound cues for paddle hits, wall bounces, and scoring events.

**Prompt:**
```
Add sound effects to my pygame ping pong game. Load .wav files for paddle hit, wall bounce, and scoring using pygame.mixer.Sound(). Play the sounds whenever ball.velocity_x or ball.velocity_y changes. Initialize pygame.mixer at the start of the file.
```

---

## ✅ Expected Game Behavior

- Smooth paddle control using `W` and `S` keys  
- AI automatically tracks and returns the ball  
- Accurate rebound physics on walls and paddles  
- Live score display for both player and AI  
- Game ends when a score limit is reached, followed by replay or exit options  

---

## 📁 Folder Layout

```
pygame-pingpong/
├── main.py
├── requirements.txt
├── game/
│   ├── game_engine.py
│   ├── paddle.py
│   └── ball.py
└── README.md
```

---

## 🧾 Submission Checklist

Before submission, ensure that:

- [ ] All 4 tasks are implemented  
- [ ] The game runs without bugs or crashes  
- [ ] Scores display and update correctly  
- [ ] The Game Over screen works as intended  
- [ ] Replay functionality is functional  
- [ ] Dependencies are listed properly in `requirements.txt`  
- [ ] The README setup steps have been verified  
- [ ] The final code is clean, modular, and easy to follow  
- [ ] Chat/LLM interaction log (with ChatGPT) is included as part of submission  
