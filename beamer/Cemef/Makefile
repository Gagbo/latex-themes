filename = sample
ALL: $(filename).pdf show

pdf: $(filename).pdf

%.pdf: %.tex *.sty Makefile
	pdflatex  $< && pdflatex  $<

show: $(filename).pdf
	okular $(filename).pdf

clean:
	  rm -f *.aux	*.bbl	*.blg	*.log	$(filename).pdf 
