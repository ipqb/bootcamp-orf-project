SOURCES=Makefile orf_project.tex
TEXNAME=orf_project
LATEX=pdflatex -halt-on-error -shell-escape

all: pdf
pdf: $(TEXNAME).pdf
$(TEXNAME).pdf: $(TEXNAME).tex $(SOURCES)
	$(LATEX) $(TEXNAME)
	$(LATEX) $(TEXNAME)
	$(LATEX) $(TEXNAME)
rerun: $(TEXNAME).tex $(SOURCES)
	$(LATEX) $(TEXNAME)
cleancache:
	rm -f $(TEXNAME).blg $(TEXNAME).bbl $(TEXNAME).aux $(TEXNAME).log $(TEXNAME).nav
clean:
	rm -f *.o \#* *~ nn $(TEXNAME).aux $(TEXNAME).log $(TEXNAME).out *.pyg *.toc $(TEXNAME).bbl $(TEXNAME).blg $(TEXNAME).nav $(TEXNAME).snm $(TEXNAME)-blx.bib $(TEXNAME).run.xml $(TEXNAME).vrb missfont.log
	touch $(TEXNAME).tex
