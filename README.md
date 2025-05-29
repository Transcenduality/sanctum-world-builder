# 🌌 Sanctum World Builder

**Sanctum World Builder** is a single-player, AI-powered storytelling engine where players co-create unique fantasy worlds and narratives with a responsive narrator.

Inspired by classic **text adventures**, **MUDs**, and **choose-your-own-adventure** books, Sanctum allows each player to define their own world, make meaningful choices, and shape an evolving story - all guided by GPT-4.

---

## 🧠 Features

### 🎮 Hybrid Interface
- **Pygame** provides a live, scrollable, immersive narrative window.
- **Tkinter** offers popup GUIs for:
  - Creating or loading a world
  - Viewing your inventory, quests, and discovered creatures

### 🌱 Evolving World State
- Every player choice is saved persistently in a `.json` file.
- Inventory, quests, and discovered entities evolve in real time.
- Side windows auto-refresh every second, showing live updates.

### 📖 AI as Dynamic Narrator
- GPT-4 responds with rich narrative text based on:
  - Player name
  - World description and theme
  - Game history, creatures, quests, and inventory
- Metadata is parsed from responses to automatically:
  - Add new quests and creatures
  - Update quest status
  - Track items picked up or lost

### 💾 Save System
- Manage up to 5 save slots with a simple wizard.
- Delete and recreate worlds easily.
- Each world has its own unique personality and storyline.

### 🛡️ Graceful API Handling
- If OpenAI credit runs out or errors occur, the narrator gracefully pauses the story without breaking the game or corrupting your save.

---

## 🚀 Getting Started

### ⚡️ Quick Start

Download the latest release, set your OpenAI API key as described below, and run the executable:

- No installation required
- Works on Windows (Python not needed)
- Saves persist to the `saves/` folder

### Set Your OpenAI API Key

Sanctum uses the GPT-4 API from OpenAI. You must set your API key as a system environment variable.

#### On Windows:
1. Open the **Start Menu**, search “Environment Variables”.
2. Under **User Variables**, click **New**.
3. Set:
   - **Variable name**: `OPENAI_API_KEY`
   - **Variable value**: your OpenAI key (starts with `sk-...`)
4. Restart any command prompt or Python editors.

---

## ✍️ How to Play

1. Enter:
   - Your world name
   - Your name
   - A theme/style for narration
   - A description of your world

4. Begin typing your actions (e.g., “I look around the valley.” or “I pick up the strange disc.”)

The narrator responds. Your journey begins.

---

## 🤝 Acknowledgements

Built with love and purpose by Marshall, for the dreamers and world-builders.  
Powered by [OpenAI](https://openai.com), and inspired by the golden age of imagination.

---

Welcome, World Builder.  
The story begins with you.
