all: lola.pdf


lola.pdf: completa.pdf reduida.pdf
	pdflatex ../motor/lola.tex
completa.pdf: completa.dvi
	dvipdf completa.dvi
completa.dvi:
	latex ../taules/completa.tex
reduida.pdf: reduida.dvi
	dvipdf reduida.dvi
reduida.dvi:
	latex ../taules/reduida.tex


clear: rclear
	rm -f *.dvi *.pdf
rclear:
	rm *.aux *.log
