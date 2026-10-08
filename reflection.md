# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
 - (for example: "the hints were backwards").
 -  Starting a "New Game" doesn't match the difficulty you picked. If you're on Easy or Hard, the sidebar tells you the range is 1–20 or 1–50, but after hitting "New Game" a few times you'll notice guesses that should be out-of-range (like guessing 80 on Easy) still get accepted/behave oddly — the game quietly stopped respecting the difficulty you selected.
 - supposed to get 8 attempts but you only have 7 bc it starts with 1 attempt made
**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

```markdown
| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
| Guess of 60 (secret is 50) | "Too High" → "Go LOWER" | "Too High" → "Go HIGHER" (backwards) | none |
| New Game on Easy, then guess 80 | Rejected, out of 1–20 range | Accepted, ignores difficulty | none |
| Fresh load, Normal difficulty (8 attempts) | Attempts left: 8 | Attempts left: 7 | none |
```

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
- claude was used
- when it fixed that the score started at 1 instead of 0, i tested it myself after the fix
- it was fine the entire time
---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
