NAME=db
compile: clean
	latexmk -pdf -quiet -xelatex -interaction=nonstopmode -file-line-error $(NAME).tex
debug: clean
	zathura $(NAME).pdf&disown
	latexmk -pdf -pvc -xelatex -file-line-error $(NAME).tex
indent:
	latexindent -s -w $(NAME).tex
clean:
	latexmk -c

