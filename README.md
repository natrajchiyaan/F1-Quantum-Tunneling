# ⚛️ F1 Quantum Tunneling

An interactive web-based quantum physics simulation that demonstrates the concept of **Quantum Tunneling** using an engaging **Formula 1 racing analogy**.

The project visualizes how a particle can pass through an energy barrier even when it does not have enough classical energy to cross it, making an abstract quantum-mechanical concept easier to understand through animation and interaction.

---

## 🚀 Overview

**F1 Quantum Tunneling** is a frontend educational simulation built with **React and Vite**.

The application represents a quantum particle as an F1-style racing car approaching an energy barrier.

Users can start the experiment and watch the simulation progress through multiple stages:

* Particle approaching the barrier
* Climbing the energy barrier
* Particle analysis
* Quantum tunneling
* Successful tunneling event

The project combines **quantum physics concepts, interactive UI, CSS animation, and a Formula 1 visual analogy** to create an engaging learning experience.

---

## ✨ Features

### ⚛️ Interactive Quantum Experiment

Start the experiment using the **START EXPERIMENT** button and observe the simulated tunneling sequence.

### 🏎️ F1 Racing Analogy

An F1-style car is used as a visual representation of the particle, making the concept of quantum tunneling easier to understand.

### ⚡ Energy Barrier Visualization

The simulation contains a clearly defined **Energy Barrier** representing the potential barrier that the particle must overcome.

### 🔬 Experiment Stages

The simulation progresses through different states:

```text
READY
   ↓
APPROACHING BARRIER
   ↓
CLIMBING ENERGY BARRIER
   ↓
ANALYZING PARTICLE
   ↓
QUANTUM TUNNELING
   ↓
TUNNELING EVENT DETECTED
```

### 📊 Experiment Parameters

The interface displays important simulation parameters:

| Parameter             |  Value |
| --------------------- | -----: |
| Particle Energy       |  40 eV |
| Barrier Height        |  70 eV |
| Barrier Width         |   2 nm |
| Tunneling Probability | 18.73% |

### 🧮 Mathematical Model

The application introduces the tunneling probability relationship:

**T ≈ e⁻²κa**

This demonstrates that tunneling probability is influenced by factors such as:

* Particle energy
* Barrier height
* Barrier width
* Particle mass

### 🖥️ Modern Scientific Interface

The application uses a futuristic laboratory-style interface with:

* NOVA branding
* System status indicator
* Experiment sections
* Parameter cards
* Simulation visualization
* Mathematical model section
* Observation section

---

# 🧠 Quantum Tunneling Explained

In classical physics, if a particle does not have enough energy to cross a barrier, it cannot pass through it.

Quantum mechanics behaves differently.

A quantum particle has a probability of being detected on the other side of an energy barrier even when its energy is lower than the barrier height.

For example:

```text
Particle Energy      = 40 eV
Barrier Height       = 70 eV
```

Classically:

```text
40 eV < 70 eV

❌ Particle cannot cross
```

Quantum mechanically:

```text
40 eV < 70 eV

✅ Non-zero tunneling probability
```

This phenomenon is known as **Quantum Tunneling**.

---

# 🏎️ F1 Analogy

The project uses an F1 racing scenario to simplify the concept.

Imagine an F1 car approaching a large mountain-like energy barrier.

Normally:

```text
          ENERGY BARRIER
               ▲
               │
      🏎️  ────╱╲────
```

If the car does not have enough energy, classical physics says it cannot cross the barrier.

Quantum mechanics introduces another possibility:

```text
      🏎️  ────╱╲──────→
                    ✨
                 TUNNEL
```

The F1 car therefore acts as a visual analogy for a quantum particle.

> **Important:** The F1 car is a visualization analogy. It is not a literal physical representation of a quantum particle.

---

# 🔬 How the Simulation Works

The experiment is controlled using React state.

The application maintains two primary states:

```javascript
const [experimentRunning, setExperimentRunning] = useState(false);
const [phase, setPhase] = useState("ready");
```

When the user starts the experiment, the application progresses through timed phases.

### Phase 1 — Ready

```text
READY
```

The simulation waits for the user to start the experiment.

### Phase 2 — Approach

After starting:

```text
APPROACHING BARRIER
```

The F1 car begins moving toward the energy barrier.

### Phase 3 — Climb

After approximately 2.5 seconds:

```text
CLIMBING ENERGY BARRIER
```

The simulation changes its visual state.

### Phase 4 — Analysis

After approximately 5 seconds:

```text
ANALYZING PARTICLE
```

The simulation represents the particle being analyzed.

### Phase 5 — Tunneling

After approximately 7 seconds:

```text
QUANTUM TUNNELING
```

The simulation represents the quantum tunneling event.

### Phase 6 — Complete

After approximately 9 seconds:

```text
TUNNELING EVENT DETECTED
```

The experiment is completed.

---

# 🛠️ Technologies Used

## Frontend

* **React 19**
* **React DOM 19**
* **JavaScript**
* **HTML5**
* **CSS3**

## Development Tools

* **Vite 8**
* **Oxlint**
* **npm**
* **Node.js**

---

# 📦 Project Structure

```text
F1-Quantum-Tunneling/
│
├── public/
│   ├── favicon
│   └── icons
│
├── src/
│   ├── assets/
│   │   ├── ...
│   │
│   ├── App.css
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── .gitignore
├── .oxlintrc.json
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

---

# ⚙️ Installation

## 1. Clone the Repository

```bash
git clone https://github.com/natrajchiyaan/F1-Quantum-Tunneling.git
```

Navigate into the project:

```bash
cd F1-Quantum-Tunneling
```

---

## 2. Install Dependencies

Run:

```bash
npm install
```

This installs the required React, Vite and development dependencies.

---

# ▶️ Run the Application

Start the development server:

```bash
npm run dev
```

Vite will provide a local development address similar to:

```text
http://localhost:5173/
```

If port 5173 is already being used, Vite automatically selects another available port.

For example:

```text
http://localhost:5174/
```

Open the displayed address in your browser.

---

# 🏗️ Build for Production

To create a production build:

```bash
npm run build
```

The production files will be generated inside:

```text
dist/
```

---

# 🔍 Preview Production Build

After building the project:

```bash
npm run preview
```

---

# 🧹 Code Quality

The project uses **Oxlint** for linting.

Run:

```bash
npm run lint
```

---

# 📊 Experiment Configuration

The current simulation displays the following experiment values:

```text
Particle Energy       : 40 eV
Barrier Height        : 70 eV
Barrier Width         : 2 nm
Tunneling Probability : 18.73%
```

These values are presented as part of the educational visualization.

---

# 🧮 Mathematical Concept

The project introduces the simplified tunneling relationship:

```text
T ≈ e⁻²κa
```

where tunneling probability decreases exponentially as the effective barrier becomes wider or more difficult to cross.

The simulation therefore demonstrates an important principle of quantum mechanics:

```text
Higher / Wider Barrier
        ↓
Lower Tunneling Probability
```

and:

```text
Lower / Narrower Barrier
        ↓
Higher Tunneling Probability
```

---

# 🎯 Learning Objectives

This project demonstrates:

* Basic quantum tunneling concepts
* Energy barriers in quantum mechanics
* Probability-based quantum behavior
* Interactive scientific visualization
* React state management
* Timed UI state transitions
* CSS-based visual simulation
* Component-based frontend development
* Modern web application development

---

# 🌍 Real-World Applications of Quantum Tunneling

Quantum tunneling is an important phenomenon in several areas of science and technology.

Examples include:

### 🔬 Scanning Tunneling Microscopes

Quantum tunneling allows extremely small electrical currents to be measured between a sharp probe and a surface.

### ☀️ Nuclear Fusion

Quantum tunneling contributes to the ability of particles to overcome effective energy barriers inside stars.

### 💻 Semiconductor Technology

Quantum tunneling plays a role in several semiconductor and nanoscale electronic phenomena.

### ⚛️ Radioactive Decay

Alpha decay can be understood using quantum tunneling through a nuclear potential barrier.

---

# 🔮 Future Improvements

Potential future versions could include:

* Real-time probability calculations
* Adjustable particle energy
* Adjustable barrier height
* Adjustable barrier width
* Particle mass selection
* Interactive probability graphs
* Wave-function visualization
* Probability-density animation
* Multiple experiment configurations
* Real quantum-mechanical calculations
* Responsive mobile optimization
* Educational explanations for each experiment phase
* Reset experiment functionality
* Experimental data logging

---

# 📱 Responsive Design

The application is designed as a modern web experience and can be further optimized for:

* Desktop browsers
* Laptop screens
* Tablets
* Mobile devices

---

# 💡 Project Highlights

| Category              | Details                        |
| --------------------- | ------------------------------ |
| Project Type          | Interactive Physics Simulation |
| Domain                | Quantum Physics                |
| Frontend              | React                          |
| Build Tool            | Vite                           |
| Language              | JavaScript                     |
| Styling               | CSS                            |
| Visualization         | F1 Racing Analogy              |
| Simulation            | Quantum Tunneling              |
| Particle Energy       | 40 eV                          |
| Barrier Height        | 70 eV                          |
| Barrier Width         | 2 nm                           |
| Displayed Probability | 18.73%                         |

---

# 🚀 Quick Start

```bash
git clone https://github.com/natrajchiyaan/F1-Quantum-Tunneling.git

cd F1-Quantum-Tunneling

npm install

npm run dev
```

Then open the local Vite URL shown in the terminal.

---

# 👨‍💻 Author

**Natarajan D**

---

# ⭐ Project Purpose

This project was created as an educational and interactive way to demonstrate one of the fascinating concepts of quantum mechanics.

Instead of presenting quantum tunneling only through equations, the application uses an **F1 racing analogy and animated visualization** to make the concept more intuitive and engaging.



