all:
	tbl ../motor/lola.tbl | eqn | troff -ms | grops > tbl.ps
	ps2pdf tbl.ps

a:
	tbl ../motor/lola.tbl | eqn | troff -ms | gropdf > tbl.pdf

debugControl:
	tbl ../motor/lola.tbl > pretroff
	troff pretroff > troff.troff
	gropdf troff.troff > tbl.pdf
