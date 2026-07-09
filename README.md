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
- **Load switches** — let the user manually set (preload) the starting time on each counter, independent of the clock pulse

## 🧠 Design Process
1. Determine the number and type of counters needed based on each section's counting range
2. Draw the state table for each counter and derive equations using Karnaugh maps
3. Initial implementation with **D flip-flops**
4. Final migration to **JK flip-flops** to simplify set/reset logic and fix issues with the minute-to-hour carry
5. Add **load logic** to each counter so the clock's time can be manually set/preloaded rather than only counting up from zero
6. Connect the tens and units components together to form the final clock circuit

## ⏱️ Setting/Loading the Time
Besides counting automatically, the clock supports **loading a custom start time**. Each counter includes a load key, built into the JK flip-flop's set/reset logic, so a desired value can be forced into the counter directly instead of waiting for it to count up from zero. This made the design of each stage uniform and simplified wiring the load feature across all counters (seconds, minutes, and hours).

## 📁 Repository Contents
- full project report including explanations, state tables, and circuit diagrams
- Circuit images designed in Proteus

## 🛠️ Tools Used
- Proteus (circuit design and simulation)

---

*This project was completed for the Digital Logic Circuits course, under Prof. Monazah.*
