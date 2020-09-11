COMPILE_TEX = latexmk -xelatex

.PHONY: all clean purge

all: presentation.pdf

clean:
	latexmk -c
	rm -f *.bbl *.nav *.snm *.vrb

purge: clean
	latexmk -C

%.pdf: %.tex
	$(COMPILE_TEX) $<
