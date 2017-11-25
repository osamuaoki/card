# 

all: card.pdf
clean:
	$(RM) card.aux card.dvi card.log card.ps card.pdf

%.ps: %.dvi
	dvips $<

%.dvi: %.tex
	latex $<

%.pdf: %.ps
	ps2pdf $<
