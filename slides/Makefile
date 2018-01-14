NAME=GANs
TEX=xelatex
BIB=biber

.PHONY: all clean

all: $(NAME).pdf

%.pdf: %.tex Content.tex %.bib
	$(TEX) $*.tex
	$(BIB) $*.bcf
	$(TEX) $*.tex

clean:
	rm -f *.aux *.bcf *.log *.xml *.toc *.nav *.bbl *.blg *.out *.snm
