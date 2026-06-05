# CLI Hangman

A terminal-based Python implementation of Hangman with modular data seperation and ASCII state rendering 

#Architecture $ Tech Stack 
* **Language:** Python 3.x
* **Modularity:** Isolates the read-only word bank into `wordslist.py` to keep the execution script clean.
* **Data Structures:** Uses tuples for memory-efficient immutable word storage, dictionaries to map penalty states to ASCII art, and sets for O(1) lookups of guessed letters.

## Logic & Validation
* **Input Validation:** Restricts inputs using `isalpha()` and length checks to block numeric or multi-character inputs.
* **State Management:** Tracks game state through an array (`hint`), updating localized indices upon correct guesses.
* **Fail State Mechanics:** Evaluates consecutive wrong guesses against the length of the ASCII dictionary to trigger loss conditions.

## Execution
```bash
git clone [https://github.com/MauryaAG07/cli-hangman.git](https://github.com/MauryaAG07/cli-hangman.git)
cd cli-hangman
python src/hangman.py
