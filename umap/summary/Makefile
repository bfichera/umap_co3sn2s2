.PHONY: main clean FORCE

SRC_DIR := .
OUTDIR := .
AUXDIR := .build
LATEXMK := latexmk
PDFLATEX := lualatex -interaction nonstopmode


main: summary.pdf

summary.pdf: FORCE
	$(LATEXMK) -lualatex="$(PDFLATEX)" -output-directory="$(OUTDIR)" -aux-directory="$(AUXDIR)" -pdf summary.tex
clean:
	$(LATEXMK) -output-directory="$(OUTDIR)" -aux-directory="$(AUXDIR)" -c -pdf summary.tex
