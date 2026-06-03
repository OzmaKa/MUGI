---
```markdown
# 🎨 MUGI CSS Library

> **A lightweight, customizable CSS library** — sitting perfectly between Bootstrap's rigidity and Tailwind's utility-only approach. Predefined components + robust theming + layout utilities + White Language companion.

[![Version](https://img.shields.io/badge/Version-1.0.0-6366f1?style=flat-square)](https://mugi-css.web.app)
[![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg?style=flat-square)](https://opensource.org/licenses/ISC)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![React](https://img.shields.io/badge/React-18+-61DAFB?style=flat-square&logo=react)](https://react.dev/)
---
## 🚀 Quick Start

```bash
# Install via npm
npm install OzmaKa/MUGI

# Import in your main CSS or JS file
import "mugi/main.css";
```

---

## ✨ Features

### 🧩 Pre-built Components

- **Buttons**: Solid, outline, sizes, FAB, social media, 3D, and glow effects.
- **Cards**: Variations, overlays, horizontal layouts, grids, and hover effects.
- **Inputs**: Classic, minimal, rounded, floating labels, and gradient borders.
- **NavBars & Footers**: Light, dark, floating, and gradient variations.
- **Notifications**: Semantic alerts (error, warning, success, note).

### 📐 Layout Utilities

- **Flexbox & Grid**: Comprehensive utilities for rows, columns, justification, and alignment.
- **Spacing**: Systematic margin and padding classes (`m-1` to `m-5`, `px-2`, etc.).
- **Displays & Positions**: Block, inline, flex, grid, absolute, fixed, and sticky controls.

### 🎨 Theming System

- Built-in support for **Light**, **Dark**, and **Ocean** themes.
- Powered by CSS variables (`--mugi-primary`, `--mugi-bg`, etc.) for instant global updates.
- Live theme switching with `localStorage` persistence support.

### ✍️ White Language (Companion)

- A lightweight, Python-based markup language for effortless HTML/CSS generation.
- Attribute-based styling (e.g., `paragraph "Hello" color:primary padding:10`).
- Automatic compilation into clean, semantic HTML with injected CSS classes.

### 🛠 Developer Experience

- Zero-config CSS import with modern resets and global typography.
- Fully responsive out of the box across all devices.
- Comprehensive documentation website built with React and Vite.

---

## 📦 Installation

### Via npm (Recommended)

```bash
npm install OzmaKa/MUGI
```

### Via Yarn or pnpm

```bash
yarn add OzmaKa/MUGI
# or
pnpm add OzmaKa/MUGI
```

---

## 🎯 Usage

### Basic CSS Import

```javascript
// In your main entry file (e.g., main.jsx or index.js)
import "mugi/main.css";
```

### Vite Configuration

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

### HTML5 Direct Link

You can also link it directly in your HTML `<head>`:

```html
<link rel="stylesheet" href="./node_modules/mugi/src/main.css">
```

### White Language Setup

To use the companion White Language compiler:

```bash
# Clone the White repository
git clone https://github.com/MagdeIssa/White.git
cd White

# Run the compiler on your .white files
python compiler.py ./my-white-files
```

---

## ⚙️ Configuration & Theming

### Applying Themes

MUGI supports multiple built-in themes. Apply a theme by adding the `data-theme` attribute to your `<body>` tag:

```html
<body data-theme="dark">
  <!-- Your content here -->
</body>
```

### Live Theme Switching

Implement dynamic theme switching with JavaScript and persist user preferences:

```html
<button onclick="setTheme('ocean')">Ocean Theme</button>

<script>
function setTheme(theme) {
  document.body.setAttribute('data-theme', theme);
  localStorage.setItem('mugi-theme', theme);
}

// Load saved theme on startup
(function () {
  const saved = localStorage.getItem('mugi-theme');
  if (saved) document.body.setAttribute('data-theme', saved);
})();
</script>
```

---

---

## 🧪 Example Usage & Output

### MUGI Components

Combine utility classes and components for rapid UI development:

```html
<!-- Primary Button -->
<button class="btn btn-primary btn-lg">Get Started</button>

<!-- Card with Hover Effect -->
<div class="card card-primary card-hover">
  <div class="card-body">
    <h3>Card Title</h3>
    <p>Build faster, look better.</p>
    <button class="btn btn-primary">Go somewhere</button>
  </div>
</div>
```

### White Language Compilation

Write simplified markup in a `.white` file:

```text
paragraph "Hello World" color:primary bg:light padding:10 radius:5
```

**Compiled HTML Output:**

```html
<p class="ws1">Hello World</p>
<!-- In <head> -->
<style>
  .ws1 { 
    color: #3498db; 
    background-color: #f8f9fa; 
    padding: 10px; 
    border-radius: 5px; 
  }
</style>
```

---

## 🛠 Development

### Prerequisites

- Node.js 18+
- npm 9+
- Git

---

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. **Fork** the repository
2. **Create a feature branch**: `git checkout -b feat/amazing-feature`
3. **Commit your changes**: `git commit -m 'feat: add amazing feature'`
4. **Push to the branch**: `git push origin feat/amazing-feature`
5. **Open a Pull Request**

### Guidelines

- Follow existing code style (Prettier + ESLint)
- Test your CSS components across multiple browsers and screen sizes
- Update documentation for new components or utilities
- Use [Conventional Commits](https://www.conventionalcommits.org/) for commit messages

### Reporting Issues

- Use the [GitHub Issues](https://github.com/OzmaKa/MUGI/issues) tab
- Include: Browser version, OS, and steps to reproduce
- Attach screenshots or code snippets when helpful

---

## 👥 The Team

Meet the dedicated professionals who crafted MUGI:

| Name                       | Role                           | Links                                                                                                               |
| :------------------------- | :----------------------------- | :------------------------------------------------------------------------------------------------------------------ |
| **Shaheen Sharba**   | Backend Developer              | [LinkedIn](https://www.linkedin.com/in/shaheen-sharba-51a90b388/) • [Portfolio](https://shaheensharba.netlify.app/)      |
| **Oussamah Kabalan** | AI-Augmented Software Engineer | [LinkedIn](https://www.linkedin.com/in/oussamah-kabalan-9618923a2/) • [Portfolio](https://oussamah-kabalan.netlify.app/) |
| **Majdi Issa**       | Backend Developer              | [White Language Creator](https://github.com/MagdeIssa/White)                                                           |

---

## 📄 License

Distributed under the **ISC License**. See [`LICENSE`](LICENSE) for more information.

---

## 🙏 Acknowledgments

- [React](https://react.dev/) — Frontend library for the documentation UI
- [Vite](https://vitejs.dev/) — Next generation frontend tooling
- [React Router](https://reactrouter.com/) — Declarative routing for React
- [React Hot Toast](https://react-hot-toast.com/) — Smoking hot React notifications

## 📬 Support

- 🌐 **Live Website**: [mugi-css.web.app](https://mugi-css.web.app)
- 📖 **Documentation**: [mugi-css.web.app/docs](https://mugi-css.web.app/docs)
- 📄 **White Language**: [mugi-css.web.app/white](https://mugi-css.web.app/white)
- 🐛 **Bug Reports**: [GitHub Issues](https://github.com/OzmaKa/MUGI/issues)

---

> **Made with ❤️ by the MUGI Team**
> *Helping developers build faster, cleaner, and more stylish web applications.* 🚀

```

```
