pdf: pdf_harvard pdf_apa

pdf_harvard:
	pdflatex -shell-escape main_harvard.tex && \
	bibtex main_harvard && \
	pdflatex -shell-escape main_harvard.tex && \
	pdflatex -shell-escape main_harvard.tex

pdf_apa:
	pdflatex -shell-escape main_apa.tex && \
	bibtex main_apa && \
	pdflatex -shell-escape main_apa.tex && \
	pdflatex -shell-escape main_apa.tex

clear:
	rm -f *.aux \
	*.bbl \
	*.blg \
	*.log \
	*.aux

svg_png:
	convert -density 1200 -resize 500x500 img/logomerito.svg img/logomerito.png
