#🧠 mmdConv – Convert Mermaid Diagrams with Ease
A lightweight CLI tool for transforming Mermaid .mmd files into SVG, PNG, or PDF. Whether you’re documenting architecture, workflows, or data models, mmdConv helps you output clean, styled diagrams—without memorizing mmdc flags.

##📚 Table of Contents
- System Requirements
- Installation
- Usage
- Configuration
- Examples
- Contribution
- License
- Contact
- Changelog

##⚙️ System Requirements
Linux users should install these system libraries to run Puppeteer:

<details> <summary>📦 OS-level Dependencies (Ubuntu/Debian)</summary>

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

##🛠️ Installation
Clone the repository:

```bash
git clone https://github.com/bongshinc/mmdConv.git
cd mmdConv
Install dependencies:

```bash
npm install
Make the Bash script executable:

```bash
chmod +x convert.sh

##🚀 Usage
🔹 Using the Bash Script
```bash
./convert.sh -i example.mmd
./convert.sh -i diagram.mmd -f png
./convert.sh -i flow.mmd -f pdf -o output-diagram.pdf
If -i is omitted, the script will prompt for the file interactively.

##🔹 Using the Node.js Script
```bash
node mmdConv.js -i input.mmd -f svg -d td
Flags:
- -i — Input .mmd file (required)
- -f — Format (svg, png, pdf), default is svg
- -o — Output file path (optional)
- -d — Graph direction (td, lr, bt, rl)

##🎨 Configuration
diagram-style.css — Set global font styles (e.g., bold, font-size)

puppeteer-config.json — Controls mmdc headless settings (e.g., --no-sandbox)

Customize these files to change how your output diagrams appear.

##🧪 Examples
Example file:

examples/book-manager.mmd
To render it:

bash
./convert.sh -i examples/book-manager.mmd

##🤝 Contribution
Contributions are welcome! Feel free to:
Fork this project
Suggest improvements or fixes via pull requests
Report issues in the Issues tab
Please follow basic code formatting conventions and keep pull requests focused.

##🧷 Badges & Links
Coming soon: shields for Node version, license, and project status. For now, check out Mermaid CLI Docs.

##🪪 License
Distributed under the MIT License. Free to use, modify, and distribute—with credit.

##📫 Contact
Questions or suggestions? Open an issue or reach out via GitHub: @bongshinc

##📝 Changelog
See CHANGELOG.md (coming soon) for version history and patch notes.
