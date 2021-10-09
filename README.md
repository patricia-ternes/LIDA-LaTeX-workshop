<!-- PROJECT SHIELDS -->
<p align="center">
    <a href="https://github.com/patricia-ternes/LIDA-LaTeX-workshop/graphs/contributors" alt="Contributors">
        <img src="https://img.shields.io/github/contributors/patricia-ternes/LIDA-LaTeX-workshop?color=%2366FFC3&logo=GitHub&logoColor=%2366FFC3&style=for-the-badge" /></a>
     <a href="https://github.com/patricia-ternes/LIDA-LaTeX-workshop/blob/main/LICENSE" alt="License">
        <img src="https://img.shields.io/github/license/patricia-ternes/LIDA-LaTeX-workshop?color=FFB3BC&style=for-the-badge" /></a>
    <a href="https://lida.leeds.ac.uk/"  alt="LIDA page">
        <img src="https://img.shields.io/badge/-🌐LIDA-black.svg?style=for-the-badge&logo=🌐&colorB=555&logoColor=99F4FB" /></a>
</p>

<!-- PROJECT LOGO -->
<br />
<p align="center">
    <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/latex/latex.png" alt="Logo" width="15% id="logo">
    <h1 align="center">Intro to LaTeX Workshop</h1>
    <h2 align="center">Leeds Institute for Data Analytics (LIDA)</h2>
</p>

## Author

* Dr Patricia Ternes
  * Research Fellow, School of Geography, University of Leeds, UK
  * [More information](https://patricia-ternes.github.io/)

## Introduction

### What is LaTeX

*"LaTeX, which is pronounced «Lah-tech» or «Lay-tech» (to rhyme with «blech» or «Bertolt Brecht»), is a document preparation system for high-quality typesetting."* 

[Definition from here](https://www.latex-project.org/)

### LaTeX features

* Typesetting journal articles, technical reports, books, and slide presentations.
* Control over large documents containing sectioning, cross-references, tables and figures.
* Typesetting of complex mathematical formulas.
* Advanced typesetting of mathematics with AMS-LaTeX.
* Automatic generation of bibliographies and indexes.
* Multi-lingual typesetting.
* Inclusion of artwork, and process or spot colour.
* Using PostScript or Metafont fonts.

[Definition from here](https://www.latex-project.org/)

### Learning curve

![learning](inputs/figures/fig1.png)

### What I can do with LaTeX?

* [Book](https://www.overleaf.com/latex/templates/tagged/book)
* [Figures, diagrams and plots](https://texample.net/tikz/examples/)
* [Homework Assignment](https://www.overleaf.com/latex/templates/tagged/homework)
* [Paper](https://www.overleaf.com/latex/templates/tagged/academic-journal)
* [Poster](https://www.overleaf.com/latex/templates/tagged/poster)
* [Presentation](https://www.overleaf.com/latex/templates/tagged/presentation)
* [Thesis](https://www.overleaf.com/latex/templates/tagged/thesis)

## Overleaf

[Overleaf](www.overleaf.com/) is a collaborative online LaTeX editor

![overleaf overview](inputs/figures/fig2.png)

### First project

After creating an account, a page with the option `Create First Project` will appear (see image bellow). To create your first `Project` just click on the button, chose one template (here, the `Blank Project`) and give a name for your project.

![first project](inputs/figures/fig3.png)

The next screen is the `Projec` page, see bellow:

![project screen](inputs/figures/fig4.png)

This screen is divided in three columns, from left to right:

1. Files
2. Text source
3. Output

Note that you can resize, minimize and maximize columns.

### Text source

The `Overleaf` automatically adds some elements to your code, even if you start with a blank project. So let's understand these elements.

#### Preamble

Everything from line 1 up to line 7 is part of the `Preamble`.

*The [`preamble`](https://latex.wikia.org/wiki/LaTeX_preamble) is the first section of an input file, before the text of the document itself, in which you tell LaTeX the type of document, and other information LaTeX will need to format the document correctly.*

The general syntax of a LaTeX document is

```latex
\documentclass{class}
   … your preamble goes here …

\begin{document}
   … your text goes here …
\end{document}
```

#### Document classes

> Line 1: `\documentclass{article}`

*When processing an input file, LaTeX needs to know which layout standard to use. Here, the class parameter for the command `\documentclass` specifies the layout to use for the document. It is recommended to put this declaration at the very beginning. Some standard classes are:*

* **article**: For articles in scientific journals, presentations, short reports, program documentation, invitations, ...
* **report**: For longer reports containing several chapters, small books, thesis, ...
* **book**: For books.
* **letter**: For writing letters.
* **beamer**: For writing presentations (see LaTeX/Presentations).

[See more about Document classes here](https://en.wikibooks.org/wiki/LaTeX/Document_Structure#Document_classes)