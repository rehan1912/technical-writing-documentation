# LaTeX Documentation

## 1. Introduction to LaTeX

LaTeX is a high-quality document preparation system used for creating professional documents. It is widely used in academic writing, scientific research, technical reports, books, articles, and mathematical publications.

LaTeX is based on the TeX typesetting system. Unlike traditional word processors, LaTeX allows users to write documents using commands and structured markup.

It is especially useful for documents containing mathematical equations, references, tables, figures, and complex formatting.

## 2. Features of LaTeX

Some important features of LaTeX are:

- **Professional formatting:** Produces well-structured and professionally formatted documents.
- **Mathematical typesetting:** Supports complex mathematical equations and symbols.
- **Automatic numbering:** Automatically numbers chapters, sections, figures, tables, and equations.
- **Cross-referencing:** Allows references to sections, equations, tables, and figures.
- **Bibliography management:** Supports citations and reference lists.
- **Portability:** LaTeX source files can be compiled on different operating systems.
- **Consistency:** Maintains consistent formatting throughout a document.

## 3. Installation of LaTeX

To use LaTeX, a distribution and an editor are generally required.

### Popular LaTeX Distributions

1. **TeX Live:** A widely used LaTeX distribution available for Windows, Linux, and macOS.
2. **MiKTeX:** A popular LaTeX distribution mainly used on Windows.
3. **MacTeX:** A LaTeX distribution designed for macOS.

### Popular LaTeX Editors

- TeXstudio
- TeXworks
- Visual Studio Code
- Overleaf (online LaTeX editor)

TeXstudio can be used to write, edit, and compile LaTeX documents.

## 4. Basic Structure of a LaTeX Document

A basic LaTeX document contains a preamble and a document environment.

Example:

```latex
\\documentclass{article}

\\usepackage{amsmath}

\\title{My First LaTeX Document}
\\author{Student}
\\date{November 2026}

\\begin{document}

\\maketitle

\\section{Introduction}

This is my first LaTeX document.

\\end{document}
```

### Explanation of Commands

- `\\documentclass{article}`: Defines the type of document.
- `\\usepackage{amsmath}`: Includes additional mathematical features.
- `\\title{}`: Defines the document title.
- `\\author{}`: Specifies the author's name.
- `\\date{}`: Sets the document date.
- `\\begin{document}`: Starts the main document.
- `\\maketitle`: Displays the title, author, and date.
- `\\end{document}`: Ends the document.

## 5. Document Classes

The `\\documentclass` command specifies the type of document.

Common document classes include:

| Document Class | Purpose |
|---|---|
| article | Articles and short reports |
| report | Long reports and projects |
| book | Books and longer documents |
| letter | Formal letters |
| beamer | Presentations |

Example:

```latex
\\documentclass[12pt,a4paper]{article}
```

Here:
- `12pt` specifies the font size.
- `a4paper` specifies the paper size.
- `article` specifies the document type.

## 6. Sections and Subsections

LaTeX provides commands to organize documents into sections and subsections.

Example:

```latex
\\section{Introduction}

\\subsection{Background}

\\subsubsection{History}
```

Important sectioning commands:

- `\\part{}`
- `\\chapter{}`
- `\\section{}`
- `\\subsection{}`
- `\\subsubsection{}`

Note: The `article` class does not support the `\\chapter{}` command.

## 7. Mathematical Equations

One of the most important features of LaTeX is its ability to create mathematical expressions.

### Inline Mathematics

Inline equations are written using `\\( ... \\)`.

Example:

```latex
The equation is \\(a^2+b^2=c^2\\).
```

### Display Mathematics

Display equations appear separately from normal text.

Example:

```latex
\\[
a^2+b^2=c^2
\\]
```

### Numbered Equations

The `equation` environment automatically numbers equations.

```latex
\\begin{equation}
E=mc^2
\\end{equation}
```

### Fractions

```latex
\\[
\\frac{a+b}{c}
\\]
```

### Square Roots

```latex
\\[
\\sqrt{x^2+y^2}
\\]
```

### Summation

```latex
\\[
\\sum_{i=1}^{n} i
\\]
```

## 8. Lists in LaTeX

LaTeX supports different types of lists.

### Unordered List

The `itemize` environment creates bullet points.

```latex
\\begin{itemize}
    \\item LaTeX
    \\item Beamer
    \\item Doxygen
\\end{itemize}
```

### Ordered List

The `enumerate` environment creates numbered lists.

```latex
\\begin{enumerate}
    \\item Introduction
    \\item Main Content
    \\item Conclusion
\\end{enumerate}
```

## 9. Tables in LaTeX

The `tabular` environment is used to create tables.

Example:

```latex
\\begin{tabular}{|c|c|}
\\hline
Name & Marks \\\\
\\hline
Student A & 85 \\\\
Student B & 90 \\\\
\\hline
\\end{tabular}
```

Explanation:

- `c` represents center alignment.
- `l` represents left alignment.
- `r` represents right alignment.
- `&` separates columns.
- `\\\\` ends a row.
- `\\hline` creates a horizontal line.

## 10. Adding Figures and Images

The `graphicx` package is used to insert images into a document.

Example:

```latex
\\usepackage{graphicx}

\\begin{figure}[h]
    \\centering
    \\includegraphics[width=0.5\\textwidth]{image.png}
    \\caption{Sample Image}
    \\label{fig:sample}
\\end{figure}
```

Explanation:

- `\\usepackage{graphicx}` loads image support.
- `\\includegraphics` inserts an image.
- `width` controls image size.
- `\\caption` adds a figure caption.
- `\\label` creates a reference label.

## 11. Labels and References

Labels and references help connect different parts of a document.

Example:

```latex
\\section{Introduction}
\\label{sec:intro}

Refer to Section~\\ref{sec:intro}.
```

The `\\label{}` command assigns a label, while `\\ref{}` refers to its number.

## 12. Page Formatting

LaTeX provides commands for page formatting.

Examples:

```latex
\\documentclass[12pt,a4paper]{article}

\\usepackage[margin=1in]{geometry}

\\usepackage{setspace}

\\onehalfspacing
```

- `geometry` controls page margins.
- `\\onehalfspacing` sets one-and-a-half line spacing.
- `\\singlespacing` sets single line spacing.
- `\\doublespacing` sets double line spacing.

## 13. Advantages of LaTeX

1. Produces high-quality documents.
2. Handles complex mathematical equations efficiently.
3. Automatically manages numbering and references.
4. Supports large documents.
5. Provides consistent formatting.
6. Supports bibliography and citation management.

## 14. Applications of LaTeX

LaTeX is commonly used in:

- Research papers and journals.
- Academic assignments.
- Technical reports.
- Books and textbooks.
- Mathematical and scientific publications.
- Conference papers and presentations.

## 15. Conclusion

LaTeX is a powerful document preparation system that helps users create professional and structured documents. Its mathematical typesetting, automatic numbering, referencing, and formatting capabilities make it an important tool for academic and technical writing.

Learning LaTeX provides a strong foundation for preparing research papers, technical reports, and professional documents.