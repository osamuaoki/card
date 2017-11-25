TEXFILES = $(wildcard *.tex)
PSFILES = $(patsubst %.tex,%.ps,$(TEXFILES))

all: $(PSFILES)	

%.ps: %.dvi
	dvips $<

%.dvi: %.tex
	latex $<
	latex $<

clean:
	-rm *.aux *.dvi *.log *.ps card.eps


