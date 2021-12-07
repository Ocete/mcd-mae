all: Ejer6.pdf

Ejer6.pdf: Ejer6.tex clean
	-pdflatex --shell-escape Ejer6.tex
	-pdflatex --shell-escape Ejer6.tex
	$(MAKE) clean

clean:
	rm -f *.aux *.blg *.log *.bbl *.toc *.out *.bcf *.xml *.gz
	rm -rf _minted-main

sesgo:
	-pdflatex --shell-escape sesgo/sesgo.tex
