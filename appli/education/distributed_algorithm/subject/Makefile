NAME = TP-DistribAlg-2016
PDFS = $(patsubst %,%.pdf,$(NAME))
PDFFLAGS = -halt-on-error -file-line-error
all: $(PDFS)

$(PDFS): %.pdf: %.tex
	pdflatex $(PDFFLAGS) $*.tex
	pdflatex $(PDFFLAGS) $*.tex
	pdflatex $(PDFFLAGS) $*.tex

clean:
	$(RM) *.log *.aux *.out

realclean: clean
	$(RM) $(PDFS)
