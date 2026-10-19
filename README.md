# 📄 README Generator

A Node.js command-line application that generates a polished, professional `README.md` file from user input. Answer a series of prompts in the terminal and the app writes a fully formatted README — complete with badges, license section, and table of contents — in seconds.

---

## 📖 Overview

Good documentation starts with a good README, but writing one from scratch is repetitive work. This CLI tool prompts for all the standard README sections, then assembles and writes the file automatically so you can spend more time coding.

---

## ✨ Features

- 📋 Prompts for all key README sections: title, description, installation, usage, contributing, tests, and license
- 🏷️ Automatically generates a **license badge** and **license section** based on your choice (MIT, Apache 2.0, GPL 3.0, and more)
- 📑 Generates a **Table of Contents** with working anchor links to each section
- 💾 Writes the finished `README.md` to the project root
- 🔗 Adds a Questions section with GitHub profile link and contact email

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Runtime | Node.js |
| CLI Prompts | Inquirer |
| File Output | Node.js `fs` module |
| Format | Markdown |

---

## 🚀 Getting Started

### Prerequisites

- Node.js (v18+)

### Installation

```bash
git clone https://github.com/Voobane/Readme-Generator.git
cd Readme-Generator
npm install
```

### Running the App

```bash
node index.js
```

Answer each prompt. When all questions are answered, `README.md` is written to the current directory.

---

## 📁 Project Structure

```
Readme-Generator/
├── utils/
│   └── generateMarkdown.js  # Builds the Markdown string from user input
├── index.js                 # Inquirer prompt definitions + fs.writeFile call
├── package.json
└── README.md
```

---

## 💡 What I Learned

- Building an **Inquirer prompt chain** that collects structured input from a user
- Using a **template literal** to assemble a multi-section Markdown document programmatically
- Dynamically inserting **license badge URLs** and anchor text based on a selection
- Writing files asynchronously with **`fs.writeFile`** and handling errors gracefully
- Thinking about **developer experience** — what makes a README genuinely useful

---

## 📸 Screenshots

> _Add a terminal walkthrough screenshot or a sample generated README to this section._

---

## 👤 Author

**Matt (Voobane)**
- GitHub: [@Voobane](https://github.com/Voobane)
