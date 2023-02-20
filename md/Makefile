NAME=geometria_algebra
compile:
	latexmk -c
	zathura $(NAME).pdf&disown
	latexmk -pdf -pvc -xelatex -interaction=nonstopmode -file-line-error $(NAME).tex
indent:
	latexindent -s -w $(NAME).tex
clean:
	latexmk -c

