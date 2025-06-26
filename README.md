# mmdConv

A simple and configurable tool to convert Mermaid `.mmd` files into `SVG`, `PNG`, or `PDF`.

---

## 🔧 System Requirements

Before you begin, make sure your system has the following libraries installed:

<details>
<summary>📦 OS-level Dependencies (Linux)</summary>

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

<details> <summary>🛠️ Setup</summary>

Clone the repository and install dependencies:

bash
git clone https://github.com/bongshinc/mmdConv.git
cd mmdConv
npm install
</details>

<details> <summary>🚀 Usage</summary>

Using the Bash script
bash
./convert.sh -i your-diagram.mmd           # Converts to your-diagram.svg
./convert.sh -i diagram.mmd -f png         # Converts to diagram.png
./convert.sh -i file.mmd -f pdf -o output.pdf
Using the Node.js script
bash
node mmdConv.js -i file.mmd -f svg -d td
Supported options:

-i: input .mmd file (required)
-f: output format (svg, png, pdf) — default is svg
-o: output filename (optional)
-d: layout direction (td, lr, bt, rl) — modifies graph direction

</details>

<details> <summary>📁 File Structure</summary>

mmdConv/
├── convert.sh                # Bash wrapper
├── mmdConv.js                # Node.js converter with spinner & CLI
├── puppeteer-config.json     # Headless Chromium config for mmdc
├── diagram-style.css         # Custom Mermaid style overrides
├── examples/
│   └── book-manager.mmd
└── README.md
</details>
