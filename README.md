# Digital Logic Circuits Course Project — Prof. Monazah

Implementation of a **digital clock** using sequential logic circuits and flip-flops, designed in **Proteus**.

## 👥 Team Members
- Ashkan Kowsari
- Amirmohammad Kaheh
- Sina Motamedinejad

## 📋 About the Project
This project designs and implements the logic needed to build a digital clock (seconds, minutes, hours) using sequential counters. The main focus is deriving the counter equations from state tables and implementing them with flip-flops.

## ⚙️ Main Circuit Components
- **Mod-10 counter** — for seconds units, minutes units, and hours units
- **Mod-6 counter** — for seconds tens and minutes tens
- **Mod-3 counter** — for hours tens
- **24-hour reset logic** — automatically resets the clock to zero
- **JK flip-flops** with reset and load key logic

## 🧠 Design Process
1. Determine the number and type of counters needed based on each section's counting range
2. Draw the state table for each counter and derive equations using Karnaugh maps
3. Initial implementation with **D flip-flops**
4. Final migration to **JK flip-flops** to simplify set/reset logic and fix issues with the minute-to-hour carry
5. Connect the tens and units components together to form the final clock circuit

## 📁 Repository Contents
- full project report including explanations, state tables, and circuit diagrams
- Circuit images designed in Proteus

---

*This project was completed for the Digital Logic Circuits course, under Prof. Monazah.*
