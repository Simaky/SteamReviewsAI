# SteamReviewsAI

**SteamReviewsAI** is a tool that fetches recent user reviews of a Steam game and uses a local LLM (e.g., Mistral) to generate a smart, structured summary including pros, cons, and a final recommendation.  
It supports both step-by-step interaction via Jupyter Notebook.

---

## 🧠 Features

- Extracts up to 100 recent reviews (English only) from any Steam game.
- Chunks and summarizes reviews using an open-source LLM without relying on external APIs.
- Outputs a clean, markdown-formatted summary with:
  - 📄 Summary  
  - ✅ Pros  
  - ❌ Cons  
  - 🕹️ Final Recommendation
- Optimized for both interactive (Google Colab) and automated (terminal script) use.

---

## 📁 Files

- `steam_reviews_ai.ipynb` – interactive notebook for step-by-step analysis in Colab or Jupyter.

---

## ⚙️ Requirements

Install dependencies via pip before proceed with the next steps.

**Minimum:** Python 3.11+, `transformers`, `torch`, `requests`, `beautifulsoup4`, and optionally `accelerate`, `bitsandbytes` for quantized model support.

---

## 🚀 How to Run

### #1 Run interactively (Colab or Jupyter)

Open `steam_reviews_ai.ipynb` in Google Colab or locally and follow the step-by-step instructions.

### #2 Open Google link with prepared script

Open [this link](https://colab.research.google.com/drive/1R_6iUcplaLBBGvSZxJEUnSaVfwviMwa0?usp=sharing), duplicate it to your drive and run step by step.


The script will:

1. Parse the app ID from the Steam URL
2. Fetch recent English reviews
3. Analyze and summarize them using your chosen local LLM
4. Print a markdown-style output to the terminal

---

## 💡 Example Output

```
🎮 Steam Game Analysis
Summary: Cyberpunk 2077 is a game that has received mixed reviews from players, 
with some praising its story, open-world, and character development, 
while others have found its interface, driving mechanics, and design choices disappointing. 
The game has seen significant improvements since its release, with patches and expansions 
addressing many of the initial issues.

Pros:

Engaging story with memorable characters
Immersive open-world with lots of interactions
Improved gameplay with updates and expansion

Cons:

Confusing interface and driving mechanics
Design choices that some players find disappointing
Difficult to learn and immersion issues due to scuffed pacing
Final Recommendation: Yes, I would recommend Cyberpunk 2077 to those who appreciate a well-developed story, interesting characters, 
and an immersive open-world experience. 
However, those who are sensitive to interface, driving, or pacing issues may find the game frustrating.
```

---
