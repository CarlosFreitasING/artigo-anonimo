Project README

This workspace contains an academic article prepared with the Springer
Lecture Notes in Computer Science (LNCS) LaTeX format.

Main document

- anonymous-article.tex : Main manuscript source file
- anonymous-article.pdf : Compiled PDF output

Bibliography

- mybibliography.bib : BibTeX database with all references
- splncs04.bst : LNCS BibTeX style

Important support files

- llncs.cls : LNCS document class
- appendixA.tex : Appendix content included by the manuscript
- PRISMA.jpg : Figure used in the paper
- llncsdoc.pdf : LNCS class documentation

How to compile (BibTeX workflow)

Run the following commands in this folder:

1. pdflatex -interaction=nonstopmode anonymous-article.tex
2. bibtex anonymous-article
3. pdflatex -interaction=nonstopmode anonymous-article.tex
4. pdflatex -interaction=nonstopmode anonymous-article.tex

Notes

- The project is configured to use BibTeX, not a manually written bibliography.
- Citation ordering/compression is handled in the LaTeX source using the
  cite package.
- Generated files (.aux, .bbl, .blg, .log) can be regenerated at any time
  from anonymous-article.tex and mybibliography.bib.
