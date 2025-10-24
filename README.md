# Gitignore Generator CLI

[![Node.js](https://img.shields.io/badge/Node.js-green?logo=node.js&logoColor=black)](https://nodejs.org/)

[![GitHub Issues](https://img.shields.io/github/issues/nishuR31/gitignore?logo=github&logoColor=black)](https://github.com/nishuR31/gitignore/issues)

> Interactive CLI tool to generate `.gitignore` files instantly from 1000+ templates using Node.js.

---

## Features

- Interactive template selection via terminal
- Supports **1000+ templates** (Node, React, Python, Java, Laravel, Rust, etc.)
- Suggests templates if input is incomplete or slightly wrong
- Automatically fetches and creates `.gitignore`
- Clean removal of temporary folders after execution

---

## Demo

```bash
npm start
```

```
Enter template (e.g., node, react, python): py
Template not found.
Did you mean: python, pythonvanilla
Enter template (e.g., node, react, python):
```

Once selected, `.gitignore` will be created in your project root.

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/nishuR31/gitignore.git
cd gitignore
```

2. Start the CLI:

```bash
npm start
```

---

## Usage

The CLI will prompt you to enter a **template name**:

```bash
Enter template (e.g., node, react, python):
```

- If exact template exists → generates `.gitignore`
- If template is ambiguous → suggests closest matches

Example:

```bash
Enter template (e.g., node, react, python): react
Template selected: react
.gitignore for react created!
```

---

## Templates

Supports **templates** from [Toptol](https://www.toptal.com/developers/gitignore/api/list) api including:

- Node, React, Vue, Angular, Python, Django, Laravel
- Rust, Go, Java, Kotlin, PHP, Ruby
- Docker, Visual Studio, IntelliJ, PyCharm, WebStorm
- …and many more

> Full list available in the `templates` array inside `index.js`.

---

## How It Works

1. Prompts user for a template name
2. Validates input against supported templates
3. Fetches `.gitignore` content from [Toptal Gitignore API](https://www.toptal.com/developers/gitignore)
4. Writes `.gitignore` to your project root
5. Cleans up temporary directories if needed

---

## Contributing

1. Fork the repo
2. Create a branch: `git checkout -b feature/YourFeature`
3. Commit your changes: `git commit -m "Add some feature"`
4. Push to branch: `git push origin feature/YourFeature`
5. Open a Pull Request

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Author

**nishuR31** - [GitHub](https://github.com/nishuR31)
