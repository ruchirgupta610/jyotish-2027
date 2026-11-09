# Jyotish 2027: Vedic Planetary Transits & Kundli Simulator

An open-source, client-side ephemeris visualizer and interactive North Indian Kundli simulator for the complete calendar year **2027**. 

Built with zero external libraries or runtime dependencies, the engine visualizes 91 verified celestial events, featuring real-time house renumbering, dynamic planetary dignity markers, combustion effects, eclipse simulations, and high-fidelity animations.

---

## 🌟 Key Features

- **Accurate Astronomical Baseline (Jan 1, 2027):**
  - Calibrated strictly to the **Nirayana (Lahiri Ayanamsha)** ephemeris.
  - Positioned using standard **Mean Nodes** (*Madhyama Rahu & Ketu*), with Rahu in Capricorn (*Makara = 10*) and Ketu in Cancer (*Karka = 4*).
  - High-frequency Moon (*Chandra*) transits are intentionally omitted from event logs to prevent clutter, keeping the focus on structural planetary cycles.

- **Chronological 91-Event Engine:**
  - Cross-verified with Drik Panchang ephemeris tables.
  - Covers all 12 Solar Sankrantis (*unbroken Leo $\rightarrow$ Virgo $\rightarrow$ Libra sequence*).
  - All 18 planetary combustion (*Asta*) and rising (*Udaya*) phases for Mercury, Venus, Jupiter, and Saturn.
  - All retrograde (*Vakri*) and progressive (*Margi*) stations.
  - Both 2027 Solar Eclipses (*Annular on Feb 6 & Total on Aug 2, complete with onset and Moksha phases*) and Penumbral Lunar Eclipses.

- **Dual-Panel Responsive Workspace:**
  - **Left Panel (40%):** Interactive North Indian (*Bhava-Fixed*) Diamond Kundli stage. Houses automatically rotate and renumber based on your selected Ascendant (*Lagna*) or Moon sign. Includes timeline scrub controls and dynamic house transit predictions.
  - **Right Panel (60%):** Live, tabular planetary dashboard. Displays current Rashi, occupied House, motion status, dignity, combustion state, and eclipse involvement, with real-time row illumination for active event subjects.
  - **Bottom Row:** Complete, responsive 91-event grid with multi-select Graha filter chips and category toggles.

- **Dynamic Visual Feedback:**
  - **Dignities:** Large, high-visibility badges for Exalted (**⬆ Uchcha**) and Debilitated (**⬇ Neecha**) states.
  - **Combustion:** Smooth CSS blur (`filter: blur(3px)`) and opacity drop to `0.22` with a pulsing ember icon (`⋆`).
  - **Eclipses:** Smoothly scaling and fading dark umbra disc (`🌑`) obscuring the Sun during *Surya Grahan*, receding cleanly upon *Grahan Moksha*.
  - **Concentric Ripples:** Material Design expanding shockwaves emitted across the stage during state-change events.

---

## 📁 Repository Structure

```text
.
├── index.html        # Complete single-page application (HTML, CSS, SVG, JavaScript)
└── README.md         # Documentation and deployment manual
```

---

## 🚀 Local Development

Because this project is self-contained in a single file with zero dependencies, no package managers (`npm`, `yarn`) or bundlers (`vite`, `webpack`) are required.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ruchirgupta/jyotish-2027.git
   cd jyotish-2027
   ```

2. **Open the application:**
   - Simply double-click `index.html` to open it in any modern browser (Chrome, Firefox, Safari, Edge).
   - Alternatively, serve it locally using Python:
     ```bash
     # Python 3
     python3 -m http.server 8000
     ```
     Then navigate to `http://localhost:8000`.

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
| :--- | :--- |
| `→` (Right Arrow) | Step forward to the next chronological event |
| `←` (Left Arrow) | Step backward to the previous event |
| `Spacebar` | Toggle auto-playback (*Play / Pause*) |

---

## 📜 License

Released under the [MIT License](LICENSE).

```text
© 2026 Ruchir Gupta.
Nirayana Lahiri Ephemeris & Gochara Engine. Built for fun & open-source exploration.
```