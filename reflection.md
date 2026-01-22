# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it? 
- List at least two concrete bugs you noticed at the start  
  (for example: "the secret number kept changing" or "the hints were backwards").
  
  When first running the game it looked normal until I started submitting my guesses. The game was not accurately representing is my guess was higher or lower than the the secret number. Also, my guesses weren't being paresed through accurately. I noticed I would submit a number but it wouldn't be used until the next index when I submitted another number.

---
## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion you accepted and why.
- Give one example of an AI suggestion you changed or rejected and why.

For this project I used Copilot and Claude as my teammates. I ran out of attempts with Copilot so I used Claude to actually help me. The most notably suggestion I took from AI was to resest the scaor, status, and history for the new game. An AI suggestion I reject was it's insitial fix for the check_guess fuction was to give me and except statement but the only issue that needed to be corrected was changing GO HIGHER to GO LOWER and vice versa. It over complicated the problem and I wasn't thinking strategically at first. 

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

I decided the bug was fixed after testing manually. I reran the test on the localhost and checked to make sure that the expected outputs were correct. A test I ran manually was the checking to makign sure that the "show hint" was producing the expected output. AI helped me to understand that test and actually be weary to what I was checking when I enetered my own input to check. 
---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
- What change did you make that finally gave the game a stable secret number?

The secret number was changing in the original apps becuase the iteration to the next attmept occured before the guess was submitted instead of after so the index was off. Streamlit reruns is a constant refresher of your code anytime you add something new small or large change it reruns the entire code over again like statring new with no previous input. Session state is a backlog of the information the you may have inserted as a unput of a test check before. Its a for a history. The final change made to fix the bug was moving them attmept count to after it was to have an accurate reflection on what attempt number the user was on. 
 
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.

One strategy from this project I would like to reuse in the furutre in the explain feature in copilot. Also, AI does something and even if it doesn't fix the exact issue I was looking for I atleast know how it interpeted my prompt and let to outputputed solution. I would persoanlly not use the Agent mode. I don't like that it changes the code for you. Even though you can deny the code it feels like the code is forced onton me to use when it pops up in the file rather than in the chat section. this project has changed the way I think about AI genrated code because if you as a human don't fully understand your task or assignment AI can over coplicated to issues you are trying to fix. Also, with AI generated code 9/10 it will probably run with no errors but that doesn't mean it actualy works for your project. 