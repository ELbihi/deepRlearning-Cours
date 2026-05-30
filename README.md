# Deep Reinforcement Learning — ENIAD 2025-2026
 
**Brahim Bassor** · IA2 · Pr. BOUTAHIR Mohamed Khalifa

**Interactive educational dashboard for Deep Reinforcement Learning**  
Practical submission — Deep Reinforcement Learning course

---

## 📋 Description

**Deep RL Explorer** is a single-file interactive web application (`drl-explorer-light.html`) that serves as a complete study and revision tool for Deep Reinforcement Learning algorithms. It was built as a practical project for a university DRL course.

The app covers the four main algorithms studied in the course, with interactive visualizations, mathematical formulas, comparative analysis, and a full quiz system.

---

## 🚀 How to Run

No installation required. The project is a **single self-contained HTML file**.

1. Download `drl-explorer-light.html`
2. Open it in any modern web browser (Chrome, Firefox, Edge, Safari)
3. That's it — no server, no dependencies to install

> External dependencies loaded via CDN: **Chart.js 4.4.0** and **Google Fonts** (Plus Jakarta Sans, JetBrains Mono). An internet connection is needed on first load for fonts and charts to render correctly.

---

## 📚 Content & Features

### 🗂️ Pages / Sections

| Section | Content |
|---|---|
| **Accueil** | Overview dashboard with algorithm summary cards and key stats |
| **Fondamentaux** | Core RL concepts: Agent, State, Action, Reward, TD vs Monte Carlo, ε-Greedy slider |
| **Q-Learning** | Off-Policy · Model-Free · Value-Based · TD Learning |
| **SARSA** | On-Policy · Model-Free · TD Learning — State-Action-Reward-State-Action |
| **PPO** | Proximal Policy Optimization · Actor-Critic architecture |
| **Dyna-Q** | Model-Based planning with internal simulation |
| **Comparaison** | Side-by-side comparison table + Chart.js learning curves |
| **Quiz** | 20 interactive multiple-choice questions with instant feedback |

### ⚙️ Interactive Features

- **ε-Greedy Slider** — visualizes exploration vs exploitation balance in real time
- **Learning curves** — animated Chart.js charts (reward over steps, convergence episodes per algorithm)
- **Algorithm cards** — clickable cards that navigate to each algorithm's detail page
- **Quiz system** — 20 questions, color-coded correct/wrong answers, score tracker, reset button
- **Smooth sidebar navigation** — fixed sidebar with active state tracking
- **Fade-in animations** — entrance animations on page load

---

## 🤖 Algorithms Covered

### Q-Learning
- **Type:** Off-Policy, Model-Free, Value-Based, TD Learning
- **Update rule:** `Q(s,a) ← Q(s,a) + α × [R + γ · max_a' Q(s',a') − Q(s,a)]`
- Key concept: uses the **theoretical best future action** (bold/risk-taking behavior)

### SARSA
- **Type:** On-Policy, Model-Free, Value-Based, TD Learning
- **Update rule:** `Q(s,a) ← Q(s,a) + α × [R + γ · Q(s',a') − Q(s,a)]`
- Key concept: uses the **actually chosen next action** (cautious behavior)

### PPO (Proximal Policy Optimization)
- **Type:** On-Policy, Model-Free, Policy-Based, Actor-Critic
- Developed by **OpenAI (2017)**
- Introduces a **clipping mechanism** to prevent catastrophic forgetting from large policy updates
- Handles **continuous action spaces** (e.g. steering angle)

### Dyna-Q
- **Type:** Off-Policy, **Model-Based**, Value-Based
- Builds an **internal model** `Model(S,A) = (R, S')` to simulate experiences
- Combines real interactions + N simulated planning steps → faster convergence

---

## 📊 Key Concepts Illustrated

| Concept | Description |
|---|---|
| **TD Learning** | Updates after each step (Q-Learning, SARSA, Dyna-Q) |
| **Monte Carlo** | Updates after full episode (REINFORCE) |
| **ε-Greedy** | Balances exploration (random) vs exploitation (learned policy) |
| **ε-decay** | Gradually reduces ε from 1.0 → ~0.05 over training |
| **On-Policy vs Off-Policy** | SARSA learns from actual actions; Q-Learning from theoretical best |
| **Model-Free vs Model-Based** | Dyna-Q builds an internal world model; others learn by trial-and-error |
| **Actor-Critic** | PPO combines policy gradient (Actor) + value estimation (Critic) |

---

## 🛠️ Technical Stack

| Technology | Usage |
|---|---|
| **HTML5** | Structure — single-file application |
| **CSS3** | Custom design system with CSS variables, responsive layout |
| **Vanilla JavaScript** | Navigation, quiz logic, slider interactivity |
| **Chart.js 4.4.0** | Learning curve charts (line) and convergence bar chart |
| **Plus Jakarta Sans** | UI font (Google Fonts) |
| **JetBrains Mono** | Mathematical formula display (Google Fonts) |

---

## 📁 File Structure

```
drl-explorer-light.html   ← Single self-contained file (HTML + CSS + JS)
README.md                 ← This file
```

---

## 🎓 Academic Context

This project was submitted as a practical work for the **Deep Reinforcement Learning** module.  
Submission deadline: **30 May 2026, 23:59**

The app was designed to consolidate and present course knowledge in an innovative, interactive format covering all four DRL algorithms studied during the semester.

---


#
