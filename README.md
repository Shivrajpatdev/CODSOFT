# CODSOFT
CODSOFT AI Internship

> Artificial Intelligence projects built during the **CodSoft AI Internship Program**

![AI](https://img.shields.io/badge/Artificial%20Intelligence-Projects-blueviolet?style=for-the-badge)
![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📋 Table of Contents

- [Overview](#overview)
- [Task 1 — Tic-Tac-Toe AI](#task-1--tic-tac-toe-ai)
- [Task 2 — Recommendation System](#task-2--recommendation-system)
- [Task 3 — Image Captioning](#task-3--image-captioning)
- [How to Run](#how-to-run)
- [Technologies Used](#technologies-used)

---

## Overview

This repository contains **3 Artificial Intelligence projects** completed as part of the CodSoft Internship. Each task demonstrates a different area of AI — game-playing agents, recommendation algorithms, and computer vision with natural language processing.

---

## Task 1 — Tic-Tac-Toe AI

📁 `Task1-TicTacToe/tic_tac_toe_ai.html`

### Description
An AI agent that plays Tic-Tac-Toe against a human player. The AI is **mathematically unbeatable** — the best outcome a human can achieve is a draw.

### Algorithm
- **Minimax Algorithm** — the AI recursively explores all possible future game states and selects the move that maximizes its chance of winning while minimizing the opponent's chance.
- **Alpha-Beta Pruning** — optimizes Minimax by skipping branches of the game tree that cannot possibly affect the final decision, making the AI faster and more efficient.

### Features
- ✅ Unbeatable AI (Hard Mode) using Minimax + Alpha-Beta Pruning
- ✅ Easy AI mode with randomized moves
- ✅ Score tracker across multiple games
- ✅ Winning combination highlight animation

### How It Works
```
Human plays X  →  AI evaluates all possible moves via Minimax
               →  Alpha-Beta Pruning skips redundant branches
               →  AI picks the optimal move as O
               →  Repeat until win or draw
```

---

## Task 2 — Recommendation System

📁 `Task2-RecommendationSystem/recommendation_system.html`

### Description
A **content-based filtering** recommendation system that suggests skincare products based on a user's personal preferences and skin profile.

### Algorithm
**Content-Based Filtering** — each product in the database is tagged with attributes (skin type, concern, budget, ingredient preference). The system scores every product against the user's profile by matching attributes, then ranks and displays the top matches.

```
Score Formula:
  Skin Type match   → 40 points
  Concern match     → 35 points
  Budget match      → 15 points
  Preference match  → 10 points
  ─────────────────────────────
  Total             → 100 points max
```

### Features
- ✅ 4-step interactive preference quiz
- ✅ 15 skincare products in the database (cleansers, serums, moisturizers, SPF, masks)
- ✅ Match percentage shown for each recommendation
- ✅ Filters by skin type, concern, budget, and ingredient preference

### Product Categories
| Category | Products |
|----------|----------|
| Cleansers | Salicylic Acid Cleanser, Ceramide Gentle Wash, Rose Hip Micellar Water |
| Serums | Niacinamide 10%, Hyaluronic Acid Boost, Vitamin C Glow, Retinol Night Repair, Centella Calm |
| Moisturizers | Oil-Free Gel, Shea Butter Rich Cream, Peptide Luxe Cream |
| Sunscreen | Invisible Mineral SPF 50, Mattifying Sunscreen SPF 40 |
| Masks | Kaolin Clay Detox Mask, Honey Glow Sleeping Mask |

---

## Task 3 — Image Captioning

📁 `Task3-ImageCaptioning/image_captioning.html`

### Description
An AI-powered image captioning system that combines **computer vision** and **natural language processing** to analyze images and generate intelligent captions, detected objects, and scene tags.

### How It Works
The app uses Claude's **Vision Transformer model** via the Anthropic API — which functions as a feature extraction + language decoder pipeline (equivalent to a ResNet/VGG + RNN/Transformer architecture):

```
Input Image
    ↓
Vision Transformer (Feature Extraction)
    ↓
NLP Decoder (Language Generation)
    ↓
Output: Caption + Objects + Scene Tags
```

### Features
- ✅ Upload any image (JPG, PNG, WEBP)
- ✅ Drag and drop support
- ✅ 5 caption styles — Descriptive, Poetic, Technical, Simple, Storytelling
- ✅ Detected object tags + scene classification
- ✅ Caption history of last 6 analyzed images
- ✅ One-click copy caption

### Caption Styles
| Style | Description |
|-------|-------------|
| 📝 Descriptive | Factual, detailed one-to-two sentence caption |
| 🎭 Poetic | Emotional, metaphorical interpretation |
| 🔬 Technical | Composition, lighting, color palette analysis |
| 💬 Simple | Clear, accessibility-friendly description |
| 📖 Story | Narrative-style caption with imagined context |

> **Note:** Requires an Anthropic API key to run. Get one free at [console.anthropic.com](https://console.anthropic.com)

---

## How to Run

All three projects are **single HTML files** — no installation or dependencies needed.

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/CODSOFT.git
   ```

2. Navigate to any task folder and open the `.html` file in your browser:
   ```bash
   cd Task1-TicTacToe
   open tic_tac_toe_ai.html
   ```

3. For Task 3 (Image Captioning), enter your Anthropic API key when prompted.

---

## Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 / CSS3 | Structure & Styling |
| Vanilla JavaScript | Game logic, filtering algorithm, API calls |
| Minimax + Alpha-Beta Pruning | Tic-Tac-Toe AI decision making |
| Content-Based Filtering | Skincare recommendation engine |
| Claude Vision API (Anthropic) | Image feature extraction + caption generation |
| Transformer Architecture | NLP-based caption decoding |

---

## 👩‍💻 Author

**Internship Program:** CodSoft AI Internship
**Batch:** 2024–2025

---

> *Built with ❤️ as part of the CodSoft AI Internship Program*
> 
