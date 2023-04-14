GRAPHVIZ = $(wildcard graphviz/*.dot)
GRAPHVIZ_SVGS = $(patsubst graphviz/%.dot, figures/%.svg, $(GRAPHVIZ))
GRAPHVIZ_PNGS = $(patsubst graphviz/%.dot, figures/%.png, $(GRAPHVIZ))


all: diagrams report.pdf

diagrams: $(GRAPHVIZ_SVGS) $(GRAPHVIZ_PNGS)

report.pdf: report.md diagrams
	# run on lab pc or install pandoc and a LaTeX distribution
	pandoc -d ./report.yaml

figures/%.svg: graphviz/%.dot
	dot -Tsvg $< > $@

figures/%.png: graphviz/%.dot
	dot -Tpng $< > $@

clean: 
	rm -rf report.pdf
