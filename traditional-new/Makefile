TEXFILES = $(wildcard *.tex)
PSFILES = $(patsubst %.tex,%.ps,$(TEXFILES))
PDFFILES = $(patsubst %.tex,%.pdf,$(TEXFILES))

all: $(PDFFILES)	

%.ps: %.dvi
	dvips $<

%.dvi: %.tex
	latex $<
	latex $<

%.pdf: %.dvi
	dvipdfmx $<


clean:
	-rm *.aux *.dvi *.log *.ps *.pdf card.eps


