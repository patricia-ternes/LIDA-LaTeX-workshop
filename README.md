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

## General LaTeX syntax

The `Overleaf` automatically adds some elements to your code, even if you start with a blank project. So let's understand these elements.

### Preamble

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

The `documentclass` is the first command of a LaTeX document, and identifies the type of document contained in the input file (from [here](https://latex.wikia.org/wiki/List_of_LaTeX_commands#documentclass_command)). The general syntax is

```latex
\documentclass[options]{class}
```

Some standard classes are:

* **article**: For articles in scientific journals, presentations, short reports, program documentation, invitations, ...
* **report**: For longer reports containing several chapters, small books, thesis, ...
* **book**: For books.
* **letter**: For writing letters.
* **beamer**: For writing presentations (see LaTeX/Presentations).

[See more about document classes here](https://en.wikibooks.org/wiki/LaTeX/Document_Structure#Document_classes)

The most common options for the generic document classes are:

 * **Main font size**: `10pt, 11pt, 12pt` (default: `10pt`)
 * **Paper size**: `a4paper, letterpaper, a5paper, b5paper, executivepaper, legalpaper` (default: `letterpaper`*)
 * **Number of columns**: `onecolumn, twocolumn` (default: `onecolumn`)

[See more about document classes options here](https://en.wikibooks.org/wiki/LaTeX/Document_Structure#Document_classes)

#### Packages

> Line 2: `\usepackage[utf8]{inputenc}` 

While writing your document, you will probably find that there are some areas where basic LaTeX cannot solve your problem. If you want to include graphics, colored text or source code from a file into your document, you need to enhance the capabilities of LaTeX. Such enhancements are called packages (from [here](https://en.wikibooks.org/wiki/LaTeX/Document_Structure#Packages)). The `usepackage` command tells LaTeX to load packages of environments, commands, and symbols for specific purposes (from [here](https://latex.wikia.org/wiki/Usepackage_(LaTeX_command))).  The general syntax is

```latex
\usepackage[options]{package}
```

The most common packages are:

* `inputenc`: input encoding
* `amsmath`, `amsfonts`: contains a comprehensive set of mathematical symbols; particularly handy for rendering matrices
* `graphicx`: to include graphics (images)
* `xcolor`: to use colours in a wide variety of ways, including rgb, cmyk, hsb
* `fancyhdr`: useful for customizing the headers and footers in your document
* `hyperref`: to automatically insert hyperlinks into the document

#### Standard titles

> Line 4: `\title{ }`

> Line 5: `\author{ }`

> Line 6: `\date{ }`

The standard classes provide four storing commands that are used to automatically create the title. The storing commands are

* **\title**
* **\author**
* **\thanks**: footnote
* **\date**

> Line 12: `maketitle`

The title is created inside the text area through the command `maketitle`

### Text

```latex
\begin{document}
   … your text goes here …
\end{document}
```

#### Sectioning commands

The commands for inserting sections are fairly intuitive. Of course, certain commands are appropriate to different document classes. For example, a book has chapters but an article doesn't (from [here](https://en.wikibooks.org/wiki/LaTeX/Document_Structure#Sectioning_commands)). Some examples:

* `\chapter{chapter name}`: only books and reports
* `\section{section name}`: not in letters
* `\subsection{subsection name}`: not in letters
* `\subsubsection{subsubsection name}`: not in letters
* `\paragraph{paragraph content}`: not in letters

The `\appendix` macro can be used to indicate that following sections or chapters are to be numbered as appendices. For example:

```latex
\section{first section}
    ... some text ...

\section{second section}
    ... some text ...

\appendix
\section{first appendix}
    ... some text ...

\section{second appendix}
    ... some text ...
```

#### Table of contents

All auto-numbered headings get entered in the Table of Contents (also for list and figures) automatically. If you want to display the tables of content, just add the command.

* `\listoffigures`
* `\listoftables`
* `\tableofcontents`

