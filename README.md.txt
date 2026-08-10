# 🦎 Chameleon Calculator (by Bhavyarjun Mishra)

A sleek, responsive, and aesthetically adaptable web calculator. Built with vanilla HTML5, CSS3, and JavaScript, it features a unique real-time theme engine that allows users to shift the calculator’s palette dynamically, echoing its namesake.

🚀 **[Live Interactive Demo](https://yourusername.github.io/chameleon-calculator/)**

---

## 📸 Presentation

<p align="center">
  <img src="images/default-theme.png" width="45%" alt="Chameleon Calculator Default Theme" />
  <img src="images/custom-theme.png" width="45%" alt="Chameleon Calculator Custom Chameleon Theme" />
</p>

---

## 🌟 Professional Features & Improvements

This project addresses key security, usability, and architecture gaps common in basic JavaScript calculator tutorials:

### 🛠️ Technical Implementation
*   **🛡️ Safe Expression Evaluation:** Replaced vulnerable raw `eval()` usage with a strict input sanitization engine (`regex` filtering) paired with an isolated `new Function()` context.
*   **⌨️ Full Keyboard Support:** Implemented global `keydown` listeners, binding physical digits, operators (`+`, `-`, `×`, `/`, `%`), `Enter`, `Backspace`, and `Escape` natively.
*   **💾 State Persistence:** Uses `localStorage` to save user-defined custom color palettes and preset theme choices across browser sessions.
*   **🧮 Enhanced Percentage Logic:** Implemented math syntax normalization (e.g., handles `50 * 10%` correctly as `5`. Modulo `%` was remapped as a percentage divisor `/100`).

### 🎨 Design & UX
*   **🦎 Dynamic Theme Engine:** Utilizes CSS Custom Properties (`vars()`) and real-time JavaScript DOM manipulation to instantly apply live color updates from color pickers to the interface.
*   **⚡ Live Preview:** An auxiliary display provides an instataneous preview of the result as the user constructs complex arithmetic expressions.
*   **📱 Responsive & Accessible:** Fully responsive design optimized for mobile touchscreens and high-DPI (Retina) displays. Utilizes ARIA landmarks and live regions for accessibility compliance.

---

## 🛠️ Built With

*   **HTML5:** Semantic structure and ARIA compliant accessibility regions.
*   **CSS3:** Custom Properties (Variables), Flexbox, Grid Layout, and responsive `@media` queries.
*   **JavaScript (ES6+):** Vanilla DOM manipulation, Keyboard Event handling, Strict execution contexts, and LocalStorage API.

---

## 🚀 Running Locally

No installation or build tools are required.

1.  Clone the repository:
    ```bash
    git clone [https://github.com/yourusername/chameleon-calculator.git](https://github.com/yourusername/chameleon-calculator.git)
    ```
2.  Navigate into the directory:
    ```bash
    cd chameleon-calculator
    ```
3.  Open `index.html` in any modern web browser.