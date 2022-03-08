# PCC MTH 111-112 Supplement

This project is a supplement to the college algebra and trigonometry textbook used by Portland Community College.
To view HTML, PDF, and EPUB output, visit [spot.pcc.edu/math/supplement111-112](https://spot.pcc.edu/math/supplement111-112/).

## Building Output Yourself

These instructions should work of a Linux or Mac OS.
For Windows, more may be required.

1. Install [LaTeX](https://www.latex-project.org/get/), including `xelatex`. You may already have it; run `xelatex --version` to check.
2. Install the [PreTeXt Command Line Interface](https://github.com/PreTeXtBook/pretext-cli/) according to the "Installing Python" and "Installing PreTeXt-CLI" sections.
3. Clone this repository with `cd; git clone https://github.com/PCCMathSAC/Supplement111-112`
4. Change directory: `cd Supplement111-112`
5. Run `pretext build -d html`.  (After the first time, you may leave off the `-d` unless you want to rebuild images.)
6. Run `pretext view html` and then in a web browser go to `http://localhost:8000`
7. To make and view the PDF, similarly run `pretext build pdf` and then `pretext view pdf`


