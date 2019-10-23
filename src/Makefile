main=compression_pipeline

all: cleanall $(main).pdf view

$(main).pdf: $(main).tex conclusion.tex  ftk.tex  pipeline.tex  references.tex  timing.tex
	/usr/bin/pdflatex $(main)
	/usr/bin/pdflatex $(main)
	/usr/bin/pdflatex $(main)
	/usr/bin/pdflatex $(main)
	mv $(main).pdf ../
view: $(main).pdf
	acroread ../$(main).pdf

clean:
	rm -f *.toc *.snm *.out *.nav *.log *.aux *.vrb *~ *.pdf

cleanall: clean
	rm -rf ../*.pdf
