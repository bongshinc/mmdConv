# mmdConv
Mermaid mmd file to SVG, PNG, or PDF file.

## 🔧 System Requirements

Before you start, make sure your system includes:


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

<summary>🛠️ Setup</summary>
Clone the repository and install dependencies:

```bash
git clone https://github.com/bongshinc/mmdConv.git
cd mmdConv
npm install

<summary>🚀 Usage</summary>
Convert via Bash script
``bash
./convert.sh -i your-diagram.mmd           # Outputs your-diagram.svg
./convert.sh -i file.mmd -f png            # Outputs file.png

Convert via Node CLI
```bash
node mmdConv.js -i file.mmd -f svg -d td

<summary>📁 File Structure</summary>

📁 File Structure
mmdConv/
├── convert.sh
├── mmdConv.js
├── puppeteer-config.json
├── diagram-style.css
├── examples/
│   └── sample.mmd
└── README.md

This block makes it easy to follow and visually appealing on GitHub. Just paste it wherever you want in your `README.md`, hit “Commit changes”, and you're good to go.

Want help adding shields (like license, Node version, etc.) or turning this into a published CLI tool next?
