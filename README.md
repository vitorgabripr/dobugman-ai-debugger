# Dobugman: AI-Powered Typo & Logic Bug Detector for Code

Dobugman is an experimental AI tool that helps developers catch **typos** and **logic errors** in source code — even when there are no syntax errors. It analyzes the code using natural language understanding to detect mistakes that are often overlooked by compilers and traditional linters.

---

## 💡 Why Dobugman?

Many bugs hide in plain sight:

- A wrong variable name that *looks* similar to the correct one.
- A loop that *runs* fine but does the wrong thing.
- A condition that never triggers due to a logic error.

Dobugman uses AI to **understand your code** and what it’s trying to do, helping you debug faster and smarter.

---

## 🧠 Features

- ✅ Detects **typos** in variable, function, and class names.
- 🧠 Identifies **logical errors** even if the code is syntactically valid.
- 🗂️ Supports code snippets, single files, and full projects.
- 🗣️ Provides **natural-language explanations** of possible issues.
- 💻 Works with **Node.js** code (JavaScript, TypeScript).
- 🔄 CLI for quick checks and automation.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/dobugman-ai-debugger.git
cd dobugman-ai-debugger
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set your API key

Create a `.env` file in the root:

```env
OPENAI_API_KEY=your-openai-key
```

> You can use any compatible LLM API.

### 4. Run Dobugman on a JavaScript or TypeScript file

```bash
node dobugman.js path/to/your/file.js
```

---

## 📂 Example

```js
function claculateArea(wdith, hight) {
    return wdith * hight;
}

console.log(claculateArea(5, 10));
```

Dobugman will output:

```
[!] Possible typo in function name: 'claculateArea' → 'calculateArea'
[!] Possible typo in variable: 'wdith' → 'width'
[!] Possible typo in variable: 'hight' → 'height'
[⚠] Logic seems correct, but the output may be wrong due to misspellings.
```

---

## 🔧 Configuration

Dobugman can be configured with a `config.json` file:

```json
{
  "language": "javascript",
  "confidenceThreshold": 0.7,
  "output": "console"
}
```

---

## 🧪 Supported Languages

| Language     | Typo Detection | Logic Analysis |
|--------------|----------------|----------------|
| JavaScript   | ✅              | ✅              |
| TypeScript   | ✅              | ✅              |
| Python (soon)| 🔜              | 🔜              |

---

## 🤝 Contributing

Feel free to open issues or pull requests. Contributions are welcome!

---

## 📄 License

MIT License © 2025 Vitor Peroza

---

🧠 *"Don't just debug — Dobugman it!"*
