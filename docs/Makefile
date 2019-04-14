all: cleanall Linux.pdf view

Linux.pdf: Linux.tex
	/usr/bin/pdflatex Linux
	/usr/bin/pdflatex Linux
	/usr/bin/pdflatex Linux
	/usr/bin/pdflatex Linux

view: Linux.pdf
	xpdf -fullscreen Linux.pdf

clean:
	rm -f *.toc *.snm *.out *.nav *.log *.aux *.vrb *~

cleanall: clean
	rm -rf *.pdf
