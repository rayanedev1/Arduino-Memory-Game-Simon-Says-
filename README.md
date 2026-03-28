# 🧠 Arduino Memory Game (Simon Says) - Official Version 🛠️

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=4285f4&height=220&section=header&text=SIMON%20SAYS%20ENGINEERING&fontSize=45&animation=fadeIn" width="100%" />
</p>

## 📖 Introduction
This project is an electronic memory game. The Arduino generates a sequence of random lights and sounds, and the player must reproduce it by pressing the corresponding buttons. This is an excellent project for understanding electronics and programming at the 3AC level!

---

## 🛠️ Precise Hardware Architecture

Here is the table of **exact** connections based on my Tinkercad schematic:

### 📋 Pin Configuration (Arduino Pins)

| Component | Arduino Pin | Wire Color | Role |
| :--- | :---: | :--- | :--- |
| 🟢 **Green LED** | `PIN 13` | Light Blue | Light Signal 1 |
| 🔵 **Blue LED** | `PIN 10` | Light Green | Light Signal 2 |
| 🟡 **Yellow LED** | `PIN 5` | Yellow | Light Signal 3 |
| 🔴 **Red LED** | `PIN 3` | Red | Light Signal 4 |
| 🟢 **Green Button** | `PIN 12` | Dark Green | Player Input 1 |
| 🔵 **Blue Button** | `PIN 9` | Dark Blue | Player Input 2 |
| 🟡 **Yellow Button** | `PIN 6` | Yellow | Player Input 3 |
| 🔴 **Red Button** | `PIN 2` | Red | Player Input 4 |
| 🔊 **Buzzer (+)** | `PIN 7` | Black | Audio Signal |
| 🔊 **Buzzer (-)** | `PIN 4` | Black | Ground / GND |

---

## 💡 Tech Talk for My Friends (Technical Corner)

Hey guys! Here is how my project works step-by-step:

### 1️⃣ Why 200Ω Resistors?
The Arduino outputs **5V**. That is too much energy for a small LED! The $200\,\Omega$ resistor acts like a "brake" to limit the current (Amperes). Without it, the LED would burn out instantly.

### 2️⃣ The `INPUT_PULLUP` Secret
Normally, every button needs a physical resistor to avoid electrical "noise" (floating states). To save space on my breadboard and make the project cleaner, I use the **hidden internal resistors** of the Arduino thanks to the `INPUT_PULLUP` command in the code!

### 3️⃣ Synesthesia (Sight + Sound)
To help your memory, every color has its own musical note. When the Red LED lights up, the buzzer makes a low sound. When the Green LED lights up, it makes a high sound. Your brain remembers the **music** and the **color** at the same time!

---

## 🧠 Code Logic (Algorithm)
The program runs in a loop (`void loop()`):
1. **Generation:** It chooses a LED at random.
2. **Display:** It plays the sequence (Light + Sound).
3. **Listening:** It waits for the player to press the buttons.
4. **Verdict:** If correct $\rightarrow$ Move to the next level. If wrong $\rightarrow$ Game Over!

---

## 👨‍💻 Developer
**Rayan_Dev** 🇲🇦  
> "Embedded engineering at the service of intelligent interaction."

<p align="center">
  <a href="mailto:rayanedev1@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" /></a>
  &nbsp;
  <a href="https://github.com/rayanedev1"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" /></a>
</p>

---
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=4285f4&height=30&section=footer" width="100%" />
  <br>
  <i>Status: 100% OPERATIONAL | Schematic and Pins precisely verified</i>
</p>
