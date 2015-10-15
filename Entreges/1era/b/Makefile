all: myclear lola.pdf

d: entrega.pdf
entrega.pdf: entrega.dvi
	dvipdf entrega.dvi
entrega.dvi: entrega.toc
	latex ../motor/entrega.tex
entrega.toc:
	latex ../motor/entrega.tex

lola.pdf: completa.pdf reduida.pdf taulacompleta.pdf taulareduida.pdf instruccio.pdf
	pdflatex ../motor/lola.tex
completa.pdf: completa.dvi
	dvipdf completa.dvi
completa.dvi:
	latex ../taules/completa.tex
reduida.pdf: reduida.dvi
	dvipdf reduida.dvi
reduida.dvi:
	latex ../taules/reduida.tex
taulacompleta.pdf: taulacompleta.dvi
	dvipdf taulacompleta.dvi
taulacompleta.dvi:
	latex ../taules/taulacompleta.tex
taulareduida.pdf: taulareduida.dvi
	dvipdf taulareduida.dvi
taulareduida.dvi:
	latex ../taules/taulareduida.tex
instruccio.pdf: instruccio.dvi
	dvipdf instruccio.dvi
instruccio.dvi:
	latex ../taules/instruccio.tex


clear: rclear
	rm -f *.dvi *.pdf
rclear:
	rm *.aux *.log -f
myclear:
	rm instruccio.* taul* -f
