# 😺 Human Friendly Meow Clock (Worst UI Alarm)

A deliberately frustrating, cat-themed alarm clock UI made for a **Worst UI Contest**.  
It looks cute, but it’s designed to be annoying: the snooze button runs away, the alarm gets louder over time, and stopping the alarm requires solving a tiny “coding” challenge.

---

## ✨ What this project is
**Human Friendly Meow Clock** is a single-page web UI (HTML/CSS/JS) that simulates an alarm clock with:
- A big analog clock (shows real current time)
- Shadowed, bordered “retro card” UI panels
- A globe-based alarm setter (spin the Earth to set the alarm)
- A chaotic alarm flow with runaway snooze + a final challenge to stop the alarm

This project is optimized for **screen recording** (demo video submission).

---

## 🧩 Core Features

### 🕒 Real-time analog clock
- Shows **current time** immediately on load
- Hour / minute / seconds hands update continuously
- Tick marks touch the clock border for a bold, “toy clock” look

### 🌎 Set alarm by spinning the Earth
- Drag to rotate the globe and marker
- Rotation maps to alarm time:
  - **0.25° = 1 minute**
  - **15° = 1 hour**
- An **alarm hand** appears on the clock and updates with the globe rotation

### 🔔 Alarm behavior
When alarm time hits:
- A popup appears with **STOP** and **SNOOZE**
- **SNOOZE runs away** across the entire screen when your cursor gets close
- Alarm sound plays from `alarmsound.mp3`
- Every **5 seconds**, the sound becomes **2× louder**

### 🧠 “Stop” triggers a coding challenge (Worst UI final boss)
- Pressing **STOP** does **not** immediately stop the alarm  
- Instead, STOP opens a challenge panel with a code screenshot and answer inputs
- If answers are wrong:
  - Attempt #1 shows a “try again” reaction image
  - Attempt #2 shows a “failed again” reaction image
- Only the correct answers **(a = 4, b = 16)** stop the alarm

---

## 📁 Project Structure

Typical files in this repo:

- `index.html` (or your main `.html` file)
- `alarmsound.mp3` (alarm audio)
- Images used in UI:
  - Clock / globe / cat graphics
  - Challenge header images (smile/flower cats)
  - Challenge code screenshot
  - Feedback reaction images (worried / cry cats)

> The project uses **relative paths**, so keep assets in the same folder unless you update the `src=""` references.

---

## ▶️ How to Run
No build tools needed.

1. Download/clone the repo
2. Open the HTML file in Chrome:
   - Double click it  
   **or**
   - Right click → Open with → Chrome

> If your browser blocks audio until interaction: click anywhere once to “unlock” audio.

---

## 🎥 Demo Tips (for contest video)
- Spin the globe to set the alarm close to the current time
- Let the alarm ring
- Try to click **SNOOZE** and show it running away
- Press **STOP** to reveal the challenge
- Enter wrong answers twice to trigger both reactions
- Finally enter **4** and **16** to stop it

---

## 🛠️ Built With
- **HTML** (single page)
- **CSS** (shadowed retro card UI)
- **Vanilla JavaScript**
- No frameworks, no dependencies

---

## ⚠️ Notes
- This UI is intentionally bad. Any frustration is a feature.
- Audio volume increases aggressively; lower your system volume before testing.

---

## 📜 License
This project is for fun / contest use.  
If you want to add an explicit license, choose one (MIT is common) and include `LICENSE`.

---

## 🙌 Credits
Made for a **Worst UI Contest** with a cat-powered design and evil interactions.
