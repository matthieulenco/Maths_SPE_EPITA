# LaTeX Setup and Compilation Guide

This guide explains how to set up LaTeX on **VS Code** and **Linux**, and how to compile your `.tex` documents efficiently.

---

## 1. On VS Code

1. **Install the Extension**: `LaTeX Workshop`

2. **Keyboard Shortcuts / Actions**:
   - `Ctrl + S` → Save (automatic compilation)
   - `Ctrl + Alt + V` → View the compiled PDF side by side with the source code
   - `Ctrl + Alt + B` → Compile manually

---

## 2. On Linux (Debian)

1. **Install `latexmk`**:
```bash
sudo apt update
sudo apt install latexmk
```

2. **Common Commands of `latexmk`**:
```bash
latexmk -c               # remove temp files like .aux, .log, .toc
latexmk -C               # remove all including the PDF
latexmk -pdf yourfile.tex # generally used for the final compile
latexmk -pdf -pvc yourfile.tex # used for continuous compile
latexmk -pdf -view=okular yourfile.tex  # view PDF in a specific viewer (Linux)
latexmk -help           # list all available options
```

