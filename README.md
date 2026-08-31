# ⚡ MathBlitz

> **Fast mental math. Build your streak. Beat your best.**

MathBlitz is a fast-paced, interactive mental-math game built for the browser. Choose your difficulty, customize the types of problems you want to practice, and challenge yourself to solve as many questions as possible while maintaining accuracy and speed.

The game combines **mental-math practice with gamification**, featuring XP, levels, streaks, combo multipliers, lives, timers, challenge modes, hints, sound effects, read-aloud support, and end-of-game performance review.

---

## 🎮 Features

### 🧠 Multiple Math Topics

Practice a variety of mathematical concepts:

* ➕ Addition
* ➖ Subtraction
* ✖️ Multiplication
* ➗ Division
* 🔢 Algebra
* √ Square Roots
* 🧩 Factorization
* 📊 Percentages
* 📝 Word Problems
* ^ Powers / Exponents
* 🔄 BODMAS
* Ⅰ Roman Numerals

Problem types can be enabled or disabled from the start screen.

---

## 🎯 Difficulty Levels

MathBlitz provides three primary difficulty levels:

| Level     | Range |       Time |
| --------- | ----: | ---------: |
| 🟢 Easy   |  1–20 | 60 seconds |
| 🟡 Medium |  1–50 | 45 seconds |
| 🔴 Hard   | 1–100 | 30 seconds |

The game also allows you to select the digit size used for generated problems, from **1-digit through 4-digit numbers**.

---

## ⚔️ Challenge Modes

Choose how you want to play:

### 🎯 Normal

Standard gameplay with a timer and lives.

### 💀 Sudden Death

Make one mistake and the game is over.

### ⚡ Blitz

Complete **20 questions as quickly as possible**.

These modes are available directly from the game setup screen.

---

## 🔥 Streak & Combo System

Correct answers build your streak.

The combo multiplier increases as your streak grows:

| Streak | Multiplier |
| -----: | ---------: |
|    0–2 |         ×1 |
|    3–4 |         ×2 |
|    5–7 |         ×3 |
|     8+ |         ×4 |

This encourages consistent accuracy and rewards players who can maintain long answer streaks.

---

## ⭐ XP & Level System

Every correct answer contributes XP.

MathBlitz includes:

* Base XP
* Streak XP bonuses
* Level progression
* XP progress bar
* Level-up notifications
* Persistent XP between sessions

## The project uses **100 XP as the base level threshold** and stores the player's XP and level using browser `localStorage`.

## ⚡ Speed Bonuses

Answer quickly to earn additional rewards.

The game tracks how quickly each question is answered and provides a **Speed Bonus** when the answer is submitted with sufficient time remaining.

---

## 💡 Hint System

MathBlitz includes a built-in hint system that can provide step-by-step guidance.

Hints can explain concepts such as:

* Percentages
* Exponents
* BODMAS
* Roman numerals
* Other supported problem types

For example, BODMAS hints explain the order:

**Brackets → Orders → Division → Multiplication → Addition → Subtraction**.

---

## 📊 Performance Tracking

During gameplay, MathBlitz displays:

* Current score
* Current streak
* Accuracy
* Question number
* Remaining time
* XP progress
* Current level
* Combo multiplier
* Remaining lives

At the end of a session, players receive a performance summary including:

* Final score
* Accuracy
* Best streak
* XP earned
* Leaderboard
* Question-by-question review

---

## 🏆 Leaderboard

The end screen includes a leaderboard section designed to compare the current performance with other recorded scores.

A question review section is also provided so players can see which questions they answered correctly or incorrectly.

---

## 🎨 Modern UI

MathBlitz uses a modern dark gaming interface featuring:

* Responsive layout
* Gradient accents
* Glass/surface-style cards
* Animated feedback
* Progress bars
* Toast notifications
* Confetti effects
* Particle effects
* Answer animations
* Timer warning states
* Light mode

The UI is designed around a compact game-card experience with a maximum content width of approximately 560px.

---

## 🔊 Sound & Voice

MathBlitz includes browser-based audio and speech features.

### Sound Effects

Different sounds are used for:

* Correct answers
* Wrong answers
* Level ups
* Combo achievements

Sound can be enabled or disabled from the interface.

### 🔊 Read Aloud

The game can read questions aloud using the browser's **Web Speech API**.

Players can:

* Enable/disable read aloud
* Select an available system voice
* Hear mathematical symbols interpreted as spoken words

---

## 💾 Persistent Preferences

MathBlitz uses browser `localStorage` to remember user preferences.

Stored preferences include:

* Difficulty
* Digit size
* Enabled math topics
* Factorization difficulty
* Timer setting
* Read-aloud preference
* Sound preference
* Selected voice
* XP and level
* Theme

---

## ⌨️ Keyboard Support

MathBlitz supports keyboard shortcuts for quickly selecting multiple-choice answers.

Use:

```text
1 → Choice 1
2 → Choice 2
3 → Choice 3
4 → Choice 4
```

This makes the game faster to play without constantly using the mouse.

---

## 🧩 Smart Question Generation

Questions are generated dynamically rather than relying on a fixed question list.

The generator selects from the enabled problem types and attempts to prevent duplicate questions within the same session.

Supported generators include:

```text
Arithmetic
Algebra
Square Roots
Factorization
Percentages
Word Problems
Exponents
BODMAS
Roman Numerals
```

The generated questions can be presented as multiple-choice questions for supported problem types.

---

## 📈 Adaptive Difficulty

MathBlitz includes an automatic scaling mechanism that can adjust difficulty based on the player's recent performance.

The system tracks:

* Correct-answer streaks
* Wrong-answer streaks
* Current scaling level

The difficulty can scale upward after sustained success and downward after repeated mistakes.

---

## 🛠️ Technology

MathBlitz is built using standard browser technologies:

* **HTML5**
* **CSS3**
* **JavaScript**
* **Web Audio API**
* **Web Speech API**
* **LocalStorage**
* **CSS Animations**

No backend or external framework is required for the core game.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/mathblitz.git
```

### 2. Open the project

Navigate into the project directory:

```bash
cd mathblitz
```

### 3. Run the game

Because MathBlitz is a client-side browser application, you can open the HTML file directly in a modern browser.

For the best development experience, use a local development server such as **VS Code Live Server**.

---

## 📁 Project Structure

A simple version of the project can be organized as:

```text
MathBlitz/
│
├── index.html
├── README.md
│
├── assets/
│   ├── icons/
│   └── images/
│
├── css/
│   └── style.css
│
└── js/
    └── game.js
```

> If the current project is still maintained as a single HTML file, the CSS and JavaScript can remain embedded until the project is refactored.

---

## 🎯 Game Flow

```text
                 ┌───────────────┐
                 │   Start Game  │
                 └───────┬───────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Select Difficulty   │
              │ & Problem Types     │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Select Challenge    │
              │ Mode                │
              └──────────┬──────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Generate        │
                │ Question        │
                └────────┬────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Answer Question     │
              └──────────┬──────────┘
                         │
                  ┌──────┴──────┐
                  │             │
                Correct       Wrong
                  │             │
                  ▼             ▼
              XP + Streak    Lose Life /
              + Combo        Break Streak
                  │             │
                  └──────┬──────┘
                         │
                         ▼
                  Next Question
                         │
                         ▼
                   End Condition
                         │
                         ▼
              ┌─────────────────────┐
              │ Results & Review    │
              │ Score / XP / Streak │
              └─────────────────────┘
```

---

## 🌟 Why MathBlitz?

MathBlitz is designed to turn traditional arithmetic practice into a **fast, engaging challenge**.

Instead of simply answering math questions, players are encouraged to improve:

**Speed + Accuracy + Consistency**

The combination of streaks, XP, levels, challenge modes, timers, and performance review makes each session feel more like a game than a worksheet.

---

## 🔮 Future Improvements

Potential improvements for future versions include:

* 🌐 Online leaderboard
* 👤 User profiles
* 📱 Progressive Web App support
* 📈 Detailed performance analytics
* 🏅 Achievements and badges
* 📅 Daily challenges
* 🔥 Daily streak tracking
* 🎓 Topic-specific practice
* 🧠 Difficulty personalization
* 🌍 Multi-language support
* ☁️ Cloud-based progress synchronization
* 🎮 Multiplayer mode

---

## 🤝 Contributing

Contributions, ideas, and improvements are welcome.

If you'd like to contribute:

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature/my-new-feature
```

3. Make your changes
4. Commit your changes

```bash
git commit -m "Add new math challenge"
```

5. Push the branch

```bash
git push origin feature/my-new-feature
```

6. Open a Pull Request

---

## 📄 License

Add your preferred license here.

For example:

```text
MIT License
```

---

## 👨‍💻 Author

**Manikandan R**

Built with ❤️ and JavaScript.

---

### ⚡ MathBlitz

**Think fast. Calculate faster.**

> **Ready to Blitz?**
