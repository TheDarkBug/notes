clean:
	rm *.aux *.fdb_latexmk *.fls *.log *.out *.synctex* *.toc

compile:
	pdflatex -shell-escape -synctex=1 -interaction=nonstopmode -file-line-error -recorder geometria_algebra.tex | grep ".*:[0-9]*:.*"
