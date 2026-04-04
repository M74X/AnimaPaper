# Publishing Guide

## PDF Generation

### Requirements
```bash
sudo apt install python3-pip texlive-full texlive-fonts-extra pandoc -y
```

### Command
```bash
pandoc <series>/<paper>/WHITE_PAPER.md \
  -o <series>/<paper>/output.pdf \
  --pdf-engine=xelatex \
  -V documentclass=article \
  -V geometry:margin=1in \
  -V fontsize=11pt \
  -V mainfont="TeX Gyre Termes" \
  -V sansfont="TeX Gyre Heros" \
  -V monofont="TeX Gyre Cursor" \
  -V linestretch=1.15 \
  -V colorlinks=true \
  -V linkcolor=NavyBlue \
  -V urlcolor=NavyBlue \
  -V toccolor=black \
  --highlight-style=tango \
  --toc \
  --number-sections
```

## Zenodo Publishing
- Upload PDF to https://zenodo.org
- Update README.md master index with DOI
