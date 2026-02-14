# Code Cards - VS Code Extension

A VS Code extension that displays code in a modular, card-based interface for easier navigation and comprehension.

## 🎯 The Problem

Traditional code editors show files as a "wall of text," which is hard to navigate, especially when trying to understand code structure quickly.

## ✨ The Solution

Code Cards parses your code and displays functions/methods/classes as individual, swipeable cards with:
- 🃏 Clean, focused view of one code unit at a time
- ⌨️ Keyboard navigation (↑↓ or j/k)
- 🎯 Quick jump to code in editor
- 🌍 Multi-language support (via VS Code's language servers)
- 📋 Card and list view modes

## 🚀 Features

- **Card View**: Focus on one function at a time
- **List View**: See all functions in a scrollable list
- **Keyboard Navigation**: Use arrow keys or vim-style (j/k) to navigate
- **Jump to Code**: Click or press Enter to jump to function in editor
- **Auto-Update**: Updates automatically as you edit code
- **Multi-Language**: Works with JavaScript, TypeScript, Python, Java, Go, Rust, and more
- **Theme-Aware**: Respects your VS Code theme

## 📦 Installation

### From VS Code Marketplace (Coming Soon)
1. Open VS Code
2. Go to Extensions (Ctrl+Shift+X)
3. Search for "Code Cards"
4. Click Install

### From Source
```bash
git clone https://github.com/Bobovinow/code-cards-vscode.git
cd code-cards-vscode
npm install
npm run build
# Press F5 to test in Extension Development Host
```

## 🎮 Usage

1. Open any code file
2. Run command: `Code Cards: Show Cards` (Ctrl+Shift+P)
3. Navigate with:
   - ↑↓ or j/k: Move between cards
   - Enter: Jump to code
   - Mouse: Click buttons to navigate

## 🏗️ Tech Stack

- **Extension Host**: TypeScript
- **UI**: React + TypeScript
- **Parsing**: VS Code Document Symbol Provider
- **Build**: Webpack
- **Styling**: CSS with VS Code theme variables

## 🛠️ Development

### Prerequisites
- Node.js >= 16
- npm >= 8
- VS Code >= 1.85

### Setup
```bash
npm install
```

### Build
```bash
npm run compile      # Compile TypeScript
npm run webpack      # Bundle React
npm run build        # Both
```

### Watch Mode
```bash
npm run watch        # Watch extension
npm run webpack:watch # Watch webview
```

### Test
Press F5 in VS Code to launch Extension Development Host

## 📁 Project Structure

```
code-cards-vscode/
├── package.json              # Extension manifest
├── tsconfig.json            # TypeScript config
├── webpack.config.js        # Webpack config
├── src/
│   ├── extension.ts        # Extension entry point
│   └── webview/
│       ├── index.tsx       # React entry
│       ├── App.tsx         # Main component
│       ├── styles.css      # Styles
│       └── types.ts        # TypeScript types
└── out/                    # Compiled output
```

## 🗺️ Roadmap

- [x] Basic card view
- [x] List view
- [x] Keyboard navigation
- [ ] Search/filter functions
- [ ] Function call relationships
- [ ] Collapsible code sections
- [ ] Custom keybindings
- [ ] Settings panel

## 🤝 Contributing

Contributions welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) first.

## 📄 License

MIT License - see [LICENSE](LICENSE) file

## 🔗 Related

- **Mobile Version**: [code-cards-mobile](https://github.com/Bobovinow/code-cards-mobile) - Kotlin/Compose mobile IDE (coming soon)

## 💡 Inspiration

This project aims to make code reading more modular and digestible, especially useful for:
- Code reviews
- Learning new codebases
- Understanding complex logic
- Mobile/tablet development (future)

---

Made with ❤️ by [@Bobovinow](https://github.com/Bobovinow)