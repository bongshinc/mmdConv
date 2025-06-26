# 🧠 mmdConv – Convert Mermaid Diagrams with Ease

A lightweight CLI tool that helps you convert `.mmd` files created with [Mermaid](https://mermaid-js.github.io/) into `SVG`, `PNG`, or `PDF` formats. 

mmdConv simplifies diagram generation by providing:

- 🧭 Customizable layout direction (`TD`, `LR`, etc.)
- 🎨 Optional CSS styling for consistent output
- 🧰 Bash and Node.js scripts for flexible workflows
- ⏱️ Feedback during processing so you know what's happening

It's handy when you want quick, reliable diagram exports — without memorizing long `mmdc` commands.


# 🛠️ Installation
## <details> <summary>📦 OS-level Dependencies (Linux)</summary>
```bash
sudo apt update
sudo apt install -y \
  libasound2t64 \
  libnss3 \
  libatk-bridge2.0-0 \
  libxss1 \
  libasound2 \
  fonts-liberation \
  libu2f-udev \
  libgbm1
</details>

## <details> <summary>📦 Project Setup</summary>
```bash
git clone https://github.com/bongshinc/mmdConv.git
cd mmdConv
npm install
chmod +x convert.sh
</details>

# ⚙️ Usage
## <details> <summary>🖥️ Bash Script</summary>
./convert.sh -i diagram.mmd                 # Outputs diagram.svg
./convert.sh -i diagram.mmd -f png          # Outputs diagram.png
./convert.sh -i diagram.mmd -f pdf -o out.pdf
If -i is not provided, it will prompt you interactively.

</details>

## <details> <summary>🧠 Node.js Script</summary>

node mmdConv.js -i diagram.mmd -f svg -d td

Supported flags:
-i input file (required)
-f format: svg (default), png, pdf
-o output file (optional)
-d direction: td, lr, bt, rl

</details>

# 🎨 Styling & Config
diagram-style.css: Customize font size, weight, and colors

puppeteer-config.json: Chromium config with --no-sandbox and timeout settings

# 📁 Project Structure
mmdConv/
├── convert.sh                # Bash wrapper
├── mmdConv.js                # Node.js CLI with spinner
├── puppeteer-config.json     # Puppeteer config
├── diagram-style.css         # Mermaid CSS overrides
├── examples/
│   └── book-manager.mmd
└── README.md

# 🪪 License
MIT — free to use, modify, and share.
