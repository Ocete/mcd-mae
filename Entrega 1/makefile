all: Ejercicios.pdf

Ejercicios.pdf: Ejercicios.tex clean
	-pdflatex --shell-escape Ejercicios.tex
	$(MAKE) clean

clean:
	rm -f *.aux *.blg *.log *.bbl *.toc *.out *.bcf *.xml *.gz
	rm -rf _minted-main

complex:
		pdflatex --shell-escape main.tex
		bibtex main
		pdflatex --shell-escape main.tex
		pdflatex --shell-escape main.tex
		cp main.pdf ../thesis.pdf
		$(MAKE) clean
