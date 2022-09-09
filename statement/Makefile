DOCNAME=statement


all:
	pdflatex $(DOCNAME)
	bibtex $(DOCNAME)
	pdflatex $(DOCNAME)
	pdflatex $(DOCNAME)
	#evince $(DOCNAME).pdf&

spellcheck:
	@for f in `find . -iname '*.tex'` ; do \
		aspell --home-dir=. --personal=dictionary.txt -t -c $$f ; \
	done


clean:
	rm -f *.aux *.log *.bbl *.blg
