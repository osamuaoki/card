all: card.ps
clean:
	$(RM) card.aux card.dvi card.log card.ps

%.ps: %.dvi
	dvips $<

%.dvi: %.tex
	latex $<
