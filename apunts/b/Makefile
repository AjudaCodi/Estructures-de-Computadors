all: lola.pdf

lola.pdf: lola.dvi
	dvipdf lola.dvi

lola.dvi:
	latex ../motor/lola.tex

b:clear all

clear:
	rm -f *.dvi *.pdf
