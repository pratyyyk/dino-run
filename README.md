# 🦕 dino-Run

An AI agent that learns to play the Chrome Dino endless runner game using neuroevolution (NEAT).

No hard-coded rules.  
No human input.  
Just evolution, bad decisions, and gradual improvement.

---

## 🧩 Overview

Dino-Run is a Python project that recreates the Chrome Dino game using **Pygame** and trains an AI agent to play it using the **NEAT** algorithm.

The agent observes basic game information and decides when to jump in real time.  
Over generations, better-performing agents survive and improve.

---

## 🧠 Learning Approach

Each dinosaur is controlled by a **feed-forward neural network** evolved by NEAT.

### Inputs
- Dinosaur’s vertical position  
- Distance to the next obstacle  

### Output
- A single value determining whether the dinosaur should **jump** or **continue running**

The network structure starts minimal and grows in complexity through evolution.

---

## ⚙️ Training Configuration

- Population size: 15 agents per generation  
- Fitness function: Distance survived  
- Activation function: tanh  
- Topology: Evolved dynamically  

Configuration parameters are defined in `config.txt`.

---

## 🕹️ Gameplay

- Infinite runner with increasing difficulty  
- Obstacles include cacti and birds  
- Speed increases as the score grows  
- No player controls — the AI handles everything

---

## 🛠️ Tech Stack

- **Python**
- **Pygame** – game logic and rendering
- **neat-python** – neuroevolution framework

---

## 📂 Installation

### Prerequisites
- Python 3.6+
- pip

### Setup

---

## 📌 Notes

- The agent starts with no knowledge of the game  
- Performance improves over generations  
- Results may vary due to randomness in evolution

---

## 🪪 License

MIT License

1. Clone the repository
2. Install dependencies
3. Ensure the `Assets/` folder exists in the root directory
4. Run:

