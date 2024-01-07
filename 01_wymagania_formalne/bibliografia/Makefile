pdf:
	pdflatex -shell-escape main_harvard.tex && \
	bibtex main_harvard && \
	pdflatex -shell-escape main_harvard.tex && \
	pdflatex -shell-escape main_harvard.tex

clear:
	rm -f main_harvard.aux \
	main_harvard.bbl \
	main_harvard.blg \
	main_harvard.log \
	main_harward.aux

svg_png:
	convert -density 1200 -resize 500x500 img/logomerito.svg img/logomerito.png
