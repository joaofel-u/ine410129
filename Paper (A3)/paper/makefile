LATEX = latexmk
LATEX_FLAGS = -shell-escape -e "\$$pdflatex=q/pdflatex -synctex=1 -interaction=nonstopmode/" -pdf

all:
	pdflatex -interaction=nonstopmode main.tex ; \
	bibtex main; \
	pdflatex -interaction=nonstopmode main.tex ;\
	pdflatex -interaction=nonstopmode main.tex ; \

clean:
	rm -f *.aux *.bbl *.bcf *.blg
	rm -f *.fls *.log *.out *.xml
	rm -f *.toc *.fdb_latexmk *.gz
	rm -f *.glo *.ist *.acn *.spl
	rm -f *-blx.bib *.snm *.nav
