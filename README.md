Here is a complete, professional, and visually appealing `README.md` tailored for your **MUGI CSS Library** repository. It includes all the documentation details, the White Language companion tool, and uses the **ISC License** as you requested.

***

```markdown
<div align="center">

# 🎨 MUGI CSS Library

### *A lightweight, customizable CSS library sitting perfectly between Bootstrap's rigidity and Tailwind's utility-only approach.*

[🌐 Live Website](https://mugi-css.web.app) • [📖 Documentation](https://mugi-css.web.app/docs) • [📄 White Language](https://mugi-css.web.app/white) • [🐛 Report Bug](https://github.com/OzmaKa/MUGI/issues) • [✨ Request Feature](https://github.com/OzmaKa/MUGI/issues)

<br />

![Version](https://img.shields.io/badge/Version-1.0.0-6366f1?style=for-the-badge&logo=none)
![License](https://img.shields.io/badge/License-ISC-22c55e?style=for-the-badge&logo=none)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

</div>

<br />

## 📖 Table of Contents

- [About The Project](#-about-the-project)
- [Key Features](#-key-features)
- [Installation & Setup](#-installation--setup)
- [Theming System](#-theming-system)
- [Core Modules](#-core-modules)
- [White Language (Companion)](#-white-language)
- [The Team](#-the-team)
- [License](#-license)

<br />

## 🚀 About The Project

**MUGI** is an open-source CSS library designed to help developers build fast, responsive, and flexible UIs without the clutter. 

Our clean interface allows developers to navigate with ease, finding the styles they need in seconds. Whether you need predefined components, layout utilities, or a robust theming system, MUGI provides all the essentials for styling without overwhelming details. 

> *"Focus on creating stunning projects while we handle the styling."*

<br />

## ✨ Key Features

* 🧩 **Pre-built Components:** Buttons, Cards, Footers, NavBars, Inputs, and Notifications ready to use.
* 📐 **Layout Utilities:** Comprehensive Flexbox, CSS Grid, Margin/Padding, and Positioning utilities.
* 🎨 **Theming System:** Built-in support for **Light**, **Dark**, and **Ocean** themes using CSS variables.
* 📱 **Fully Responsive:** Flawlessly adapts to any device or screen size out of the box.
* ⚡ **Lightweight & Fast:** No bloat. Just clean, modern CSS architecture.
* 🛠️ **Modern CSS Reset:** Includes a modern reset and global styles for a consistent foundation.

<br />

## 📦 Installation & Setup

You can easily install MUGI via your favorite package manager:

```bash
# npm
npm install OzmaKa/MUGI

# yarn
yarn add OzmaKa/MUGI

# pnpm
pnpm add OzmaKa/MUGI
```

### ⚡ Quick Start

After installing, simply import the main CSS file into your project's entry point or stylesheet:

```javascript
import "mugi/main.css";
```

#### 💡 Vite Users
If you are using MUGI in a Vite project, add this alias to your `vite.config.js` to ensure paths resolve correctly:

```javascript
import path from 'path';

export default defineConfig({
  resolve: {
    alias: {
      mugi: path.resolve(__dirname, 'node_modules/mugi/src'),
    },
  },
});
```

#### 🌐 HTML5 Users
You can also link it directly in your HTML `<head>`:

```html
<link rel="stylesheet" href="./node_modules/mugi/src/main.css">
```

<br />

## 🌗 Theming System

MUGI supports multiple built-in themes. You can easily switch between **Light**, **Dark**, and **Ocean** themes by adding the `data-theme` attribute to your `<body>` tag:

```html
<body data-theme="dark">
  <!-- Your content here -->
</body>
```

You can also implement live theme switching using JavaScript and persist user preferences using `localStorage`. Check the [Documentation](https://mugi-css.web.app/docs) for advanced theming guides.

<br />

## 🧱 Core Modules

MUGI is organized into several powerful modules:

1. **Base:** Modern CSS reset, global typography, and CSS variables.
2. **Components:** 
   * **Buttons:** Solid, outline, sizes, FAB, social media, 3D, and glow effects.
   * **Cards:** Variations, overlays, horizontal layouts, and grids.
   * **Inputs:** Classic, minimal, rounded, floating labels, and gradient borders.
   * **NavBars & Footers:** Light, dark, floating, and gradient variations.
3. **Layout:** Displays, Flexbox, Grid, Margin & Padding, Positions, and Spacing.
4. **Utilities:** Colors (bg, text, border, hover, gradient), Text formatting, Typography, and Visibility/Opacity controls.

<br />

## 📄 White Language

MUGI comes with a companion tool: **White Language**. 

White is a lightweight, Python-based markup language designed to help developers create clean, structured, and styled HTML pages effortlessly. Instead of writing verbose HTML and CSS, you can use White's simplified syntax, and the compiler automatically generates beautiful, responsive HTML/CSS.

### Installation
```bash
git clone https://github.com/MagdeIssa/White.git
cd White
```

### Usage Example
Create a `.white` file and write:
```text
paragraph "Hello World" color:primary bg:light padding:10 radius:5
```

Compile it using Python:
```bash
python compiler.py ./my-white-files
```

👉 [Explore Full White Language Docs](https://mugi-css.web.app/white)

<br />

## 👨‍💻 The Team

Meet the dedicated professionals who crafted MUGI:

| Name | Role | Links |
| :--- | :--- | :--- |
| **Shaheen Sharba** | Backend Developer | [LinkedIn](https://www.linkedin.com/in/shaheen-sharba-51a90b388/) • [Portfolio](https://shaheensharba.netlify.app/) |
| **Oussamah Kabalan** | AI-Augmented Software Engineer | [LinkedIn](https://www.linkedin.com/in/oussamah-kabalan-9618923a2/) • [Portfolio](https://oussamah-kabalan.netlify.app/) |
| **Majdi Issa** | Backend Developer | - |

<br />

## 📜 License

Distributed under the **ISC License**. 

```text
ISC License

Copyright (c) 2024 MUGI CSS Library

Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
PERFORMANCE OF THIS SOFTWARE.
```

<br />

<div align="center">

**If you find MUGI useful, please consider giving this repository a star! ⭐**

[⬆ Back to Top](#-mugi-css-library)

</div>
```
