---
# You can also start simply with 'default'
theme: bricks
background: https://cover.sli.dev
title: Introduction to Artificial Intelligence
info: |
  ## Intro to AI — Bridge to Calculus
  Week 1
class: text-center
drawings:
  persist: false
transition: slide-left
mdc: true
---

# Introduction to Artificial Intelligence

Raj Venkat

---
layout: section
transition: fade-out
---
<br>

# Introductions

::right::

- **What is your name**
- **Why did you choose to take the AI module**
- **Ice breaker question** : What song or album could you listen to on repeat?

---

# Turns out, AI comes in a few flavors

<v-clicks>

- **Makes new things** : words, pictures, video, music
- **Guesses an answer** : like "is this email spam or not?"
- **Learns by trying** : gets better the more it practices
- **Finds a path** : like Maps finding a route to school

</v-clicks>



---

# Let's try some AI

<div grid="~ cols-3 gap-6">
<div>

**Makes things**

- Words : [ChatGPT](https://chat.openai.com/) , [Gemini](https://gemini.google.com/) , [Claude](https://claude.ai/)
- Pictures : [Gemini](https://gemini.google.com/)
- Video : [PixVerse](https://app.pixverse.ai/creation/video)
- Music : [Suno](https://suno.com/)
- Design : [Recraft](https://www.recraft.ai/get-started)

</div>
<div>

**Sees**

- [Google Lens](https://lens.google/)
- [Teachable Machine](https://teachablemachine.withgoogle.com/)

</div>
<div>

**Finds answers**

- [Andi](https://andisearch.com/)
- [Perplexity](https://www.perplexity.ai/)

</div>
</div>

<br>

**Try together** : put the **same prompt** in ChatGPT, Gemini, and Claude. How do they differ? 
\
Ask one in your **second language**. Does it still make sense?



---
layout: quote
---
# What is an "AI agent"?

An **agent** is a helper that **sees**, **thinks**, then **does** something.

---

# AI is all around you

What does each see? How do they act based on that?
<div grid="~ cols-3 gap-4">
<div>

**Roomba** \
sees: walls, dirt \
does: turn, clean

</div>
<div>

**Netflix** \
sees: what you watched \
does:<span v-click> pick what's next</span>

</div>
<div>

**Google Maps** \
sees:<span v-click> roads, traffic</span> \
does: choose a route

</div>
<div>

**ChatGPT** \
sees:<span v-click> your words</span> \
does:<span v-click> guess the next words</span>

</div>
<div>

**Autocomplete** \
sees:<span v-click> what you typed</span> \
does:<span v-click> finish the word</span>

</div>
<div>

**Your idea?** \
sees: ? \
does: ?

</div>
</div>



---

# Before you go

Please fill out the quick question form for next class's activity  [Tuesday Activity](#) 

---
layout: statement
class: text-center
---

# Thank you!

See you tomorrow.

---
layout: cover
---

# Introduction to Artificial Intelligence

Raj Venkat

---
layout: quote
---

# Recap

AI is all around us. An agent **sees**, **thinks**, then **does**. \
It can **make** things, **guess** answers, and **find** paths.

---
layout: section
transition: fade-out
---

# Where did AI come from?

---

# The story of AI

<img src="./public/ai-timeline.png" class="w-full rounded shadow mt-2" alt="Timeline of AI history" />



---
layout: section
---

# Turing Test: spot the bot

We send the **same question** to a person and to an AI.
Can you tell which answer is the human's?

[ChatGPT](https://chat.openai.com/) 
\
[Claude](https://claude.ai/)

::right::

<div>
    <img src="/alan_turing.jpg" alt="Turing Test" class="w-full max-h-80 object-contain rounded shadow" />
  </div>


---

# Why does AI need huge computers?

<div grid="~ cols-2 gap-8">
<div>

**CPU:** \
A **few** workers doing one job after another

</div>
<div>

**GPU:** \
**A lot of** workers doing jobs **all at once**

</div>
</div>

AI does a *huge* number of tiny sums at the same time. \
It can run in a giant **data center** or on a single **GPU** on a desk.

*Think: how much electricity does each one use?*

<div class="flex justify-center mt-4">
  <iframe width="100%" height="250" style="max-height:60vh; margin:auto;" class="rounded border mb-6" src="https://www.youtube.com/embed/gJ84mx3HbY8?si=Lp9TTbiZskrxdjpN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy"></iframe>
</div>


---
layout: statement
class: text-center
---

# Thank you!

See you tomorrow.

---
layout: intro
---

# Introduction to Artificial Intelligence

Raj Venkat


---
layout: quote
---

# Recap

AI grew up over ~70 years, in waves. \
It needs lots of computing and lots of **electricity**!!!

---
layout: section
transition: fade-out
---

# Every problem is secretly a game

---

# A game has three components

<v-clicks>

- A **state** is a picture of how things are *right now*
- A **move** is a way to change the state
- A **goal** is the state you're trying to reach

</v-clicks>

<br>
<v-click>

Solving the game = finding a **path** of moves to the goal.

</v-click>



---

# Is this email spam? (play 10 questions)

```mermaid {scale: 0.7}
graph LR
  A[An email arrives] --> B{Asks for password<br/>or bank details?}
  B -->|Yes| S1[SPAM]
  B -->|No| C{Do you know<br/>the sender?}
  C -->|Yes| OK1[Probably OK]
  C -->|No| D{Lots of typos, or<br/>'You won a prize!'?}
  D -->|Yes| S2[SPAM]
  D -->|No| OK2[Probably OK]
```



---

# Some games are about rules

<div grid="~ cols-2 gap-6">
<div>

**N-Queens** Place queens so none can attack another.

<div style="height:350px; overflow:auto; display:flex; justify-content:center; border-radius:8px; margin-top:8px; border:1px solid #ccc;">
  <iframe width="800" height="800" style="display:block;" src="https://www.n-queens.com/" title="N-Queens puzzle"></iframe>
</div>

</div>
<div>

**Map coloring** 
\
Color regions so no two neighbors share a color.

[Open Map Coloring](https://mathigon.org/course/graph-theory/map-colouring){target="_blank" rel="noreferrer noopener"}

</div>
</div>

---

# Missionaries & cannibals

<div grid="~ cols-2 gap-6">
<div>

Get everyone across the river safely.

- A **state** = who is on each bank + where the boat is
- A **move** = one safe boat trip

[Play it online](https://plastelina.net/cannibals-missionaries/)

</div>
<div>

<iframe class="rounded border" width="100%" height="300" src="https://plastelina.net/cannibals-missionaries/" title="Missionaries and cannibals"></iframe>

</div>
</div>



---

# Connect the states → a map
```mermaid {scale: 0.8}
graph LR
  S((start)) --> A((s1)) --> C((s3)) --> G((goal))
  S --> B((s2)) --> C
  A --> D((s4)) --> G
```
Write states on paper, connect them with string. \
\
Solving = **finding a path** from start to goal.



---
layout: statement
class: text-center
---

# Thank you!

See you tomorrow.

---
layout: intro
---

# Introduction to Artificial Intelligence

Raj Venkat

---
layout: quote
---

# Recap

Every problem can be a **game**: states, moves, a goal. \
Connect the states and you get a **map** to search.

---
layout: section
transition: fade-out
---

# Finding the path = search

---

# Bigger maps

<div grid="~ cols-3 gap-4">
<div class="rounded border p-4 shadow-sm">

[**8-puzzle**](https://8puzzle.org/){target="_blank" rel="noreferrer noopener"}  
Slide tiles into order

</div>
<div class="rounded border p-4 shadow-sm">

[**Rubik's cube**](https://onlinecube.com/){target="_blank" rel="noreferrer noopener"}  
~43 quintillion states

</div>
<div class="rounded border p-4 shadow-sm">

[**Maze**](https://cariboutests.com/games/mazes.php?lang=en){target="_blank" rel="noreferrer noopener"}  
Start → Exit

</div>
</div>

<br>

The map is *huge*. Instead of guessing, find a smart way to reach the goal.



---


# Search = exploring step by step

An agent never sees the whole answer. It checks the closest states first, then the next ring, then the next — until it reaches the goal.

<div style="height: 350px; overflow: auto; border-radius: 8px; margin-top: 10px;" class="border">
  <iframe 
    src="https://qiao.github.io/PathFinding.js/visual/" 
    width="100%" 
    height="800" 
    scrolling="yes" 
    style="border: none;">
  </iframe>
</div>



---
layout: statement
class: text-center
---

# What do **you** want to build?


---
layout: statement
---

# Thank you!

See you next week.
