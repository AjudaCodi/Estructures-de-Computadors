all:
	tbl ../motor/lola.tr | eqn | troff -ms | grops > tbl.ps
	ps2pdf tbl.ps

a:
	tbl ../motor/lola.tr | eqn | troff -ms | gropdf > tbl.pdf

debugControl:
	tbl ../motor/lola.tr > preEQN
	eqn preEQN > pretroff
	troff pretroff > troff.troff
	gropdf troff.troff > tbl.pdf
