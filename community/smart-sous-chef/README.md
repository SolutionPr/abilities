# Smart Sous Chef 🍳

Smart Sous Chef is a voice-first cooking assistant built for the OpenHome platform.  
It uses the Spoonacular API to fetch real recipes and guides users step-by-step through cooking — completely hands-free.

---

## 🎯 What It Does

Smart Sous Chef allows users to:

- Search for real recipes by name
- Follow step-by-step cooking instructions
- Say “next” or “repeat” to control flow
- Ask ingredient questions like “How much garlic?”
- Set multiple named kitchen timers
- Ask for nutrition information
- Exit anytime with “stop” or “exit”

Designed specifically for voice speaker environments.

---

## 🗣 Example Voice Commands

**Starting a Recipe**
- “Start cooking roasted beef.”
- “I want to cook pasta.”

**Navigation**
- “Next”
- “Repeat”
- “What step are we on?”
- “Stop”

**Ingredient Questions**
- “How much salt?”
- “How much garlic?”

**Timers**
- “Set oven timer for 20 minutes.”
- “How much time left?”
- “Cancel oven timer.”

**Nutrition**
- “How many calories?”
- “Protein?”

---

## 🏗 How It Works

Smart Sous Chef:

1. Accepts a recipe name from the user
2. Calls the Spoonacular API
3. Retrieves structured recipe data
4. Enters guided cooking mode
5. Reads one instruction at a time
6. Waits for user navigation commands

It uses:

- OpenHome SDK (`MatchingCapability`)
- Asynchronous session tasks for timers
- `urllib` for API calls (sandbox-safe)
- Voice-optimized short responses

---

## 🧠 Design Principles

- Voice-first experience
- Short 1–2 sentence responses
- Hands-free usability
- Clear exit paths
- Graceful error handling
- Single clear purpose: guided cooking

---

## 🔐 Setup

1. Get a free API key from:  
   https://spoonacular.com/food-api

2. Replace in `main.py`:
with your actual key.

---

## 🚀 Installation (OpenHome)

1. Go to: https://app.openhome.com
2. Create a new Custom Ability
3. Paste `main.py`
4. Set trigger words like:
   - "smart chef"
   - "start cooking"
   - "kitchen assistant"
5. Test in Live Mode

---

## 📦 Project Structure

smart-sous-chef/
│
├── main.py
└── README.md