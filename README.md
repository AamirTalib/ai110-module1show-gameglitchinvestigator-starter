# 🎮 Game Glitch Investigator: The Impossible Guesser

## 🚨 The Situation

You asked an AI to build a simple "Number Guessing Game" using Streamlit.
It wrote the code, ran away, and now the game is unplayable. 

- You can't win.
- The hints lie to you.
- The secret number seems to have commitment issues.

## 🛠️ Setup

1. Install dependencies: `pip install -r requirements.txt`
2. Run the broken app: `python -m streamlit run app.py`

## 🕵️‍♂️ Your Mission

1. **Play the game.** Open the "Developer Debug Info" tab in the app to see the secret number. Try to win.
2. **Find the State Bug.** Why does the secret number change every time you click "Submit"? Ask ChatGPT: *"How do I keep a variable from resetting in Streamlit when I click a button?"*
3. **Fix the Logic.** The hints ("Higher/Lower") are wrong. Fix them.
4. **Refactor & Test.** - Move the logic into `logic_utils.py`.
   - Run `pytest` in your terminal.
   - Keep fixing until all tests pass!

## 📝 Document Your Experience

- [The games purpose it to have the player quess the secret number out of a certain ranfge of numbers] 

- [The bugs I found are as follows: Hints are inacurate, New game feature doesnt work, Number ranges and attempts are mismatched across difficulty levels, the scoring system also does not make any sense ]

- [ ] Explain what fixes you applied.

## 📸 Demo Walkthrough

## Demo Walkthrough

1. The user selects **Normal** difficulty, which gives a number range of 1 to 100 and eight attempts.
2. In this example, the secret number is 50. The user enters 40, and the game correctly identifies the guess as **Too Low** and tells the user to go higher.
3. The user then enters 70. The game correctly identifies the guess as **Too High** and tells the user to go lower.
4. The user enters an invalid value such as `hello`. The game displays an error message and does not use one of the player’s attempts.
5. The user enters 50, receives a winning message, and sees their final score.
6. The user clicks **New Game**, and the game resets the secret number, attempts, score, history, and game status so another game can begin.



## 🧪 Test Results

```
# Paste your pytest output here, e.g.:
# pytest tests/
# ========================= 4 passed in 0.01s =========================
```

## 🚀 Stretch Features

- [ ] [If you choose to complete Challenge 4, describe the Enhanced UI changes here — a screenshot is optional]
