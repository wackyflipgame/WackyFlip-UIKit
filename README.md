# 🎨 WackyFlip-UIKit

Shared UI Components & Design System
Reusable components, theming, and layout logic powering the consistent visual experience across all Wacky Flip interfaces — including Web, Mobile, and internal tools.

---

## 🧩 Overview

`WackyFlip-UIKit` is the **central source of truth for UI design and interaction patterns** used throughout the [Wacky Flip](https://wackyflip.com/) ecosystem. This library promotes consistency, accessibility, and rapid development by providing ready-to-use components, standardized tokens (color, spacing, typography), and utility logic for responsive design.

Whether you're building tournament dashboards, mobile menus, or developer tools — this UI kit ensures everything looks and feels like Wacky Flip.

---

## 🌟 Features

* ✅ **Reusable UI Components**
  Buttons, modals, dropdowns, sliders, inputs, tabs, avatars, tooltips, and more.

* 🎨 **Theme System**
  Centralized color palette, typography styles, shadows, spacing, and breakpoints.

* 📱 **Responsive Design**
  Mobile-first, grid-based layouts with support for scaling and flexible screen sizes.

* 💻 **Cross-Platform Ready**
  Works with `WackyFlip-Web`, `WackyFlip-Mobile`, and `WackyFlip-DevTools`.

* 🌈 **Customization Support**
  Easily theme for seasonal events (e.g., Halloween, Rainbow Obby) using variant tokens.

* ♿ **Accessibility-Focused**
  Keyboard navigation, ARIA roles, and contrast-friendly defaults.

---

## 📁 Directory Structure

```
WackyFlip-UIKit/
├── src/
│   ├── components/
│   │   ├── Button/
│   │   ├── Modal/
│   │   ├── Dropdown/
│   │   └── ...
│   ├── theme/
│   │   ├── colors.ts
│   │   ├── typography.ts
│   │   ├── spacing.ts
│   │   └── breakpoints.ts
│   ├── utils/
│   │   └── responsive.ts
│   └── index.ts
├── docs/
│   └── Storybook components & usage guides
├── .storybook/
├── README.md
└── LICENSE
```

---

## 🚀 Installation

### Using npm:

```bash
npm install @wackyflip/uikit
```

### Using yarn:

```bash
yarn add @wackyflip/uikit
```

---

## 🔧 Usage Example

```tsx
import { Button, Modal } from '@wackyflip/uikit';

function Example() {
  return (
    <>
      <Button onClick={() => setOpen(true)}>Join Tournament</Button>
      <Modal isOpen={open} onClose={() => setOpen(false)}>
        <h2>Ready to Flip?</h2>
      </Modal>
    </>
  );
}
```

---

## 📖 Component Library

We use **Storybook** to document and test components. To run it locally:

```bash
npm install
npm run storybook
```

Available components include:

* ✅ Button
* ✅ Modal
* ✅ Avatar
* ✅ Tabs
* ✅ Tooltip
* ✅ ProgressBar
* ✅ Card
* ✅ Dialog
* ✅ Toast
* ✅ Spinner

> Want a new component? Create an issue or PR!

---

## 🧪 Used In

* [`WackyFlip-Web`](https://github.com/wackyflipgame/WackyFlip-Web)
* [`WackyFlip-Mobile`](https://github.com/wackyflipgame/WackyFlip-Mobile)
* [`WackyFlip-DevTools`](https://github.com/wackyflipgame/WackyFlip-DevTools)

All projects pull from this design system for visual consistency and performance.

---

## 🌐 Theming

You can override the default theme by wrapping your app with `ThemeProvider`:

```tsx
import { ThemeProvider, defaultTheme } from '@wackyflip/uikit';

<ThemeProvider theme={{ ...defaultTheme, colors: { primary: '#FF00FF' } }}>
  <App />
</ThemeProvider>;
```

---

## 📦 Tech Stack

* React + TypeScript
* Tailwind CSS
* Storybook
* Vite / Rollup for builds
* ESLint + Prettier for style consistency

---

## 🤝 Contributing

We welcome your PRs for new components, bug fixes, and design enhancements. Please:

* Follow the component naming conventions
* Include Storybook stories and tests
* Document your props and variants

> See `CONTRIBUTING.md` for full guidelines.

---

## 🧾 License

MIT License © Wacky Flip Studios
