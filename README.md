# 🧠 mmdConv – Your Mermaid Diagram Power Tool
A lightweight CLI toolkit to convert .mmd (Mermaid) files into beautiful SVG, PNG, or PDF diagrams — with styling, layout control, and zero guesswork.

# 🚀 Why mmdConv?
Mermaid is powerful, but let’s be honest — the CLI can be clunky. You find yourself:
Manually tweaking layout directions
Forgetting CLI flags every time
Wishing for better font sizes and styling
Wondering if it’s even working when it hangs

## mmdConv fixes all that with:
🌀 A Bash wrapper that prompts and guides you
🧭 Direction control (TD, LR, etc.) via flags
🎨 Custom CSS styling for bold, readable diagrams
⏱️ Spinner + duration feedback so you’re never left guessing

# 🛠️ Installation
## <details> <summary>📦 OS-level Dependencies (Linux)</summary>
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
