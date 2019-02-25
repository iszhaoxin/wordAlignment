TEX = pdflatex
BIBTEX = bibtex
DVIPDF = dvipdfmx

BIB = emnlp2017.bib
SRC = emnlp2017.tex
MAIN= $(SRC:.tex=)
DVI = $(SRC:.tex=.dvi)
PDF = $(SRC:.tex=.pdf)

all: pdf clean

pdf: 
	$(TEX) $(MAIN)
	$(BIBTEX) $(MAIN)
	$(TEX) $(MAIN)	
	$(TEX) $(MAIN)

clean:
	rm -f *.bbl *.blg *.aux *.log *.dvi *.toc *.lot *.lof *.out