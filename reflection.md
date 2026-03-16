# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
It looked like it was working fine then when I actually ran it, it started showing errors.
- List at least two concrete bugs you noticed at the start  
  (for example: "the secret number kept changing" or "the hints were backwards").
  -New game always used randint(1, 100) regardless of difficulty.
  -attempts was initialized to 1 but new game reset it to 0,
# causing the first-guess attempt count to differ between a fresh load and a new game.

---

## 2. How did you use AI as a teammate?
- I was able to actually go in and look through the code and understand the errors and ask AI to fix it as a beginner coder. The AI explained to me what it was doing and also asked me if I wanted to implement it.

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  Ai really catches mistakes faster then I would like the mistake with the difficulty level, it suggested a easy fix like adding a hard section. I then ran it and verified it.
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
Ai asked if I wanted to fix the guess points and I said yes but it gave a super complicated while loop. I then asked it to give me a more simple solution that would allow the code to run.

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
When it ran smoothly and looked easy to real
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
I used 0, 1, 10000, and 50 to run in the guess and I tried it and recorded my answers. This allowed me to understand all the levels.
- Did AI help you design or understand any tests? How? 
It helped me design by telling me if I was testing wrong when I asked how I didnt find the error.

---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
The random line allowed me to renerate new numbers each time.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
I would explain that streamlit takes the input and saved it each time you run the code 
- What change did you make that finally gave the game a stable secret number?
The if "secret" not in st.session_state: allows me to rerun the program and generates a new secret if one doesnt exist.

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
Asking ai to test for me to give me a template/
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
I would document better when I worked with others
- In one or two sentences, describe how this project changed the way you think about AI generated code.
It allowed me to understand and shed a better light on how to use AI for the good.
