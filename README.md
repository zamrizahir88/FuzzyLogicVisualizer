# 🧠 FuzzyLogic Visualizer v2.5

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![Firebase](https://img.shields.io/badge/Firebase-039BE5?style=for-the-badge&logo=Firebase&logoColor=white)
![Cloudflare Workers](https://img.shields.io/badge/Cloudflare_Workers-F38020?style=for-the-badge&logo=Cloudflare&logoColor=white)

**A lightweight, browser-based IDE for designing, simulating, and exporting Mamdani Fuzzy Inference Systems.**

🚀 **[Try the Live Web App Here!](https://zamrizahir.github.io/YOUR_REPO_NAME/)** *(Replace with your actual link)*

---

## ✨ Key Features

* **Visual Membership Function Editor:** Easily create Triangular, Trapezoidal, Gaussian, Bell, and Sigmoidal shapes with real-time validation.
* **Real-Time Simulation Engine:** Drag input sliders and watch the math happen instantly. Features live visual overlays of the aggregated fuzzy set and defuzzification line.
* **Rule Editor & Inference Trace:** Build complex IF/THEN rules with global AND/OR logic. View exactly how rules are evaluated step-by-step.
* **1-Click Code Generation:** Export your entire system into working code for:
  * 🐍 **Python** (`skfuzzy` scripts)
  * 📐 **MATLAB** (`.m` scripts & `.fis` files)
  * ⚡ **C++ / Arduino** (For ESP32 and embedded microcontrollers)
* **🧭 Guided Steps:** A progress bar (Variables → MFs → Rules → Check → Simulate → Export) shows students what to do next.
* **🔴 Live Simulation:** Results update instantly while editing; input sliders sit right above the charts.
* **✏️ Drag-to-Edit MFs:** Turn on "Edit shape" on a chart and drag the points of a membership function (snapping, undo, Esc to cancel; no accidental edits when off).
* **▦ Rule Table (FAM):** Edit 2-input rule bases as a grid; gaps and conflicts are highlighted.
* **📊 Rule Viewer:** Mini charts for every rule in the Inference Trace, like MATLAB's Rule Viewer.
* **✅ Rule-Base Checker:** Automatically finds gaps (input combinations with no rule), conflicting or duplicate rules, unused variables/MFs, and input ranges no membership function covers. One click creates a rule for a gap.
* **🗻 Control Surface:** Rotatable 3D surface (2+ inputs) or control curve (1 input) showing the output for every input combination.
* **📄 PDF Report:** One-click report with settings, MF charts, rules, rule check, example simulation and control surface.
* **🤖 AI Assistant (Dr. Zamri):** An embedded AI tutor powered by Groq (via a secure Cloudflare Worker proxy) to help students design fuzzy systems. It only answers questions about fuzzy logic and this website.
* **☁️ Hybrid Cloud Saves:** Save files locally as `.fuzzyjson`, or log in with Google (Firebase) to save projects to a personal cloud dashboard.

---

## 📸 Screenshots

> **Figure 1:** The main workspace showing variables, live graphs, and the rule editor.

> **Figure 2:** Real-time simulation trace showing rule firing strengths and defuzzification.

---

## 🛠️ Tech Stack & Architecture

This project is built with a **"Vibe Coded" Serverless Architecture**. 
* **Frontend:** A single `index.html` file using vanilla JavaScript, CSS3, and [Chart.js](https://www.chartjs.org/) for rendering graphs.
* **Backend / AI:** A [Cloudflare Worker](https://workers.cloudflare.com/) 
* **Database / Auth:** [Firebase v9](https://firebase.google.com/)

---

## 🚦 Quick Start for Users

1. Open the [Live Web App](https://zamrizahir88.github.io/FuzzyLogicVisualizer/main.html).
2. Click **💡 Examples** in the top menu to load a pre-built system (e.g., *Auto Braking System* or *Smart Fan Controller*).
3. Open the **🔬 SIMULATION** panel on the right side.
4. Click **▶️ RUN SIMULATION** and adjust the sliders to see the fuzzy logic in action!

---

## 👨‍🏫 Author
Developed by **Dr. Zamri** *Universiti Malaysia Perlis (UniMAP)* [View My CV/Portfolio](https://zamrizahir88.github.io/cv/main.html)
