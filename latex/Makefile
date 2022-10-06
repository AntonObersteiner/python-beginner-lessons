#src=$(ls -w1 | egrep "[0-9][0-9]_.+\.tex")
tex=xelatex
#quiet= > /dev/null
src= \
	01_getting_started.tex \
	02_grundlagen_typen_IO.tex \
	03_object_orientation.tex \
	04_object_orientation_module.tex \
	06_matplotlib.tex \
	07_dictionaries.tex \
	08_shortest_path.tex \
	09_files.tex
pdf=$(src:.tex=.pdf)

all:
	for p in $(pdf); do $(MAKE) $$p; done
echo:
	@echo "src: " $(src)
	@echo "pdf: " $(pdf)
# %.pdf: ../%.tex Makefile
# 	$(tex) $< $(quiet)
clean:
	rm -f *.aux *.fdb_latexmk *.fls *.log *.out *.synctex.gz *.toc *.nav *.snm *.bbl *.blg *.run.xml *.bcf *.vrb

01_getting_started.pdf: 01_getting_started.tex Makefile
	$(tex) 01_getting_started.tex $(quiet)
02_grundlagen_typen_IO.pdf: 02_grundlagen_typen_IO.tex Makefile
	$(tex) 02_grundlagen_typen_IO.tex $(quiet)
03_object_orientation.pdf: 03_object_orientation.tex Makefile
	$(tex) 03_object_orientation.tex $(quiet)
04_object_orientation_module.pdf: 04_object_orientation_module.tex Makefile
	$(tex) 04_object_orientation_module.tex $(quiet)
06_matplotlib.pdf: 06_matplotlib.tex Makefile
	$(tex) 06_matplotlib.tex $(quiet)
07_dictionaries.pdf: 07_dictionaries.tex Makefile
	$(tex) 07_dictionaries.tex $(quiet)
08_shortest_path.pdf: 08_shortest_path.tex Makefile
	$(tex) 08_shortest_path.tex $(quiet)
09_files.pdf: 09_files.tex Makefile
	$(tex) 09_files.tex $(quiet)
