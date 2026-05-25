# 🚀 ToDesktop Landing Page Clone

A pixel-perfect, highly responsive clone of the premium **ToDesktop** business landing page. This project showcase modern frontend design principles using **Tailwind CSS (v4)**, vanilla JavaScript, and smooth scroll animations.

---

## ✨ Features

- **📱 Fully Responsive Layout:** Seamless experience across Mobile, Tablet, and Desktop screens.
- **✨ Interactive Mobile Navigation:** Sliding overlay menu for mobile devices.
- **🔄 Dynamic Scroll-Linked Animations:** Brand logo rows that shift left and right horizontally as the user scrolls, powered by the JavaScript `IntersectionObserver` API.
- **❓ Interactive Accordion FAQs:** Expandable and collapsible sections with smooth chevron rotations.
- **🗂 Bento Grid Details Section:** A modern grid layout highlighting product offerings with elegant hover states and subtle border styles.
- **🎨 Premium Design System:** Customized typography using the Google Fonts *Poppins* (for headings) and *Inter* (for body copy), along with a curated palette of indigo, amber, and neutral tones.

---

## 🛠 Tech Stack

*   **HTML5:** Semantic architecture for improved accessibility and SEO.
*   **Tailwind CSS (v4.x):** For styling, leveraging utility classes and the latest Tailwind import directive.
*   **Vanilla JavaScript (ES6+):** Lightweight, dependency-free code handling scroll observers and interactive states.
*   **Font Awesome:** Vector icons for all features and navigation elements.

---

## 📂 Project Structure

```text
bisness_website/
├── assets/             # Brand logos, icons, and illustrations
├── sourcecode/         # Alternative layout designs and script backups
│   ├── index2.html
│   └── script2.js
├── src/
│   ├── input.css       # Tailwind source entry point (@import "tailwindcss")
│   └── output.css      # Compiled production stylesheet
├── index.html          # Main HTML entry point
├── script.js           # Core JS for animations and menu interaction
├── style.css           # Custom styles overriding/extending Tailwind
└── README.md           # Project documentation
```

---

## 🚀 Getting Started

### 1. Run Locally
Since this is a static webpage, you can run it directly:
*   Simply open the `index.html` file in your preferred web browser.
*   *Recommended:* Use an extension like **Live Server** in VS Code to enable hot reloading.

### 2. Working with Tailwind CSS (v4)
To make styling changes and recompile the CSS, you can run the Tailwind CLI:

Make sure you have Node.js installed, then execute:
```bash
# Watch for file changes and rebuild output.css automatically
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
```

---

## 🧠 Behind the Logic

*   **Scroll Observers (`script.js`):** Uses `IntersectionObserver` to track when brand lists (`#line1`, `#line2`, etc.) enter the viewport. Once active, a `scroll` listener computes the bounding rectangle relative to the viewport height to apply clean horizontal translations (`translateX`) with configurable speeds.
*   **FAQ Accordion toggles:** Uses standard accessibility references like `aria-controls` to link headers with collapsible body text and handles rotations using CSS transitions.
