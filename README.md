# mmdConv

mmdConv is a command-line tool for converting Mermaid `.mmd` files into `SVG`, `PNG`, or `PDF` formats.

## Purpose

This tool streamlines the Mermaid rendering process, offering convenient control over styles and layout direction without needing to memorize long `mmdc` command-line options. It’s ideal for generating architecture, flow, or data diagrams quickly.

## Installation

Requires Node.js. To install:

```bash
git clone https://github.com/bongshinc/mmdConv.git
cd mmdConv
npm install
chmod +x convert.sh
```

## System Requirements

Linux systems require these libraries for headless Chromium (used by Puppeteer):

```bash
sudo apt install -y \
  libasound2t64 \
  libnss3 \
  libatk-bridge2.0-0 \
  libxss1 \
  libasound2 \
  fonts-liberation \
  libu2f-udev \
  libgbm1
```

## Usage

### Bash script

```bash
./convert.sh -i diagram.mmd
./convert.sh -i diagram.mmd -f png
./convert.sh -i diagram.mmd -f pdf -o output.pdf
```

### Node.js script

```bash
node mmdConv.js -i diagram.mmd -f svg -d td
```

Options:
- `-i` input file (required)
- `-f` output format (`svg`, `png`, `pdf`)
- `-o` output filename (optional)
- `-d` layout direction (`td`, `lr`, `bt`, `rl`)

### Test Example

```bash
./convert.sh -i examples/book-manager.mmd
```

## License

Distributed under the MIT License. See the `LICENSE` file for details.
