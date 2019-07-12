# Context

When you are doing your thesis, you are dreaming of the day you will start to write this manuscript. Is it this day for you? Good! Now the questions are _How to write this thesis?_ and _What should it look like?_. To the first question, I would say that currently LaTeX is the "best" solution. To the second one, you can find plenty of LaTeX style over Internet.

When I tried to find the perfect LaTeX style, I found out that most of LaTeX styles for thesis were just modified (and bugged) versions of the LaTeX book class. So, I decided to start from scratch. The book class is pretty nice but, like everybody, I wanted to modify marges, the style of part/chapter/section, etc. I realize that most of these modifications can be done directly using specific LaTeX packages instead of modifying the book class. I decided to gather all my modifications in a unique file named `style.tex`.

I propose a template and not just a LaTeX style because after compiling it, you will already have an empty version of your thesis. The code is simple, well commented, and can easily be modified without being a LaTeX expert.

After compiling this template, one is supposed to get a file that looks like [this PDF file.](thesis_template.pdf)

# What you will find in the template

The LaTeX thesis template contains everything you need to start your thesis: a cover page, the table of content, how to write an equation, insert pictures, cite a paper, use correctly PDF link, list of tables and figures, etc.Here is the list of the LaTeX files provided:

- `manuscript.tex` - main file
- `preambule.tex`- define the LaTeX evironment and include basic packages
- `style.tex` - modify of the book class using appropriate packages
- `cover.tex` - cover page
- `acknowledgments.tex`
- `introduction.tex`
- `chapter_01.tex`
- `chapter_02.tex`
- `chapter_03.tex`
- `chapter_04.tex`
- `conclusion.tex`
- `annexe_01.tex`
- `annexe_02.tex`
- `bibliography.bib` - bibliography file

If one does not include the `style.tex` file in the `manuscrit.tex` file, the thesis will use the default book class style without any modification. Therefore, one is sure to never break the book class.


# Template compilation

You have to choose if you prefer to compile the template using LaTeX or PDFLaTeX (which have to be installed). I would recommand the second option because then you can use PNG, JPEG, and PDF images in your thesis which is very convenient. Using LaTeX, you must use EPS images. Anyway, in the folder figures I provide you all the necessary images to compile the template using LaTeX or PDFLaTeX.

**Compiling using PDFLaTeX**

In a terminal, type the following commands:

```
% pdflatex manuscript.tex
% pdflatex manuscript.tex
% bibtex   manuscript.aux
% pdflatex manuscript.tex
% pdflatex manuscript.tex
```

**Compiling using LaTeX**

In a terminal, type the following commands:

```
% latex  manuscript.tex
% latex  manuscript.tex
% bibtex manuscript.aux
% latex  manuscript.tex
% latex  manuscript.tex
```