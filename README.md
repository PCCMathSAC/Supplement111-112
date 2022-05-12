# PCC MTH 111-112 Supplement

This project is a supplement to the college algebra and trigonometry textbook used by Portland Community College.
To view HTML, PDF, and EPUB output, visit [spot.pcc.edu/math/supplement111-112](https://spot.pcc.edu/math/supplement111-112/).

## Building Output Yourself

These instructions should work of a Linux or Mac OS.
For Windows, more may be required.

1. Install [LaTeX](https://www.latex-project.org/get/), including `xelatex`. You may already have it; run `xelatex --version` to check. If your LaTeX version is old, you might not be able to build certain features of this project. Notably, the graphs. Consider updating your LaTeX installation.
2. Install the [PreTeXt Command Line Interface](https://github.com/PreTeXtBook/pretext-cli/) according to the "Installing Python" and "Installing PreTeXt-CLI" sections.
3. Clone this repository with `cd; git clone https://github.com/PCCMathSAC/Supplement111-112`
4. Change directory: `cd Supplement111-112`
5. Run `pretext build -d html`.  If you have a compilation error, it could be that your LaTeX installation was unable to build the diagrams. Attempting to build the diagrams is what the `-d` indicates. So you could try again with `pretext build html` and you might get HTML output without the graphs. (After the first time, you may leave off the `-d` unless you want to rebuild images for some reason.)
6. Run `pretext view html` and then in a web browser go to `http://localhost:8000`
7. To make and view the PDF, similarly run `pretext build pdf` and then `pretext view pdf`. If you had trouble making the images for HTML, then you will hit the same obstacles when making PDF output.

The PreTeXt CLI does not (at this time) build EPUB output. Building EPUB can be done with direct use of [PreTeXt](https://github.com/PreTeXtBook/pretext). These instructions will be updated once the CLI can build EPUB output.
