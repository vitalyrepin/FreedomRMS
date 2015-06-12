# Main input (w/o extension)
MAIN_FNAME=handbook
# Additional files the main input file depends on
ADDDEPS=fourfreedoms.tex quiz1.tex quiz2.tex quiz3.tex quiz4.tex quiz5.tex

IMAGES=

GOALS = $(MAIN_FNAME).pdf
DVIFILES = $(MAIN_FNAME).dvi

COPY = if test -r $*.toc; then cp $*.toc $*.toc.bak; fi

main:           $(DVIFILES)

all:            $(GOALS)

DEPS = 	$(MAIN_FNAME).tex $(ADDDEPS)


$(MAIN_FNAME).dvi: $(DEPS) $(patsubst %.png,%.eps,$(IMAGES))
$(MAIN_FNAME).pdf: $(DEPS) $(IMAGES)


%.dvi:          %.tex
		latexmk $<

%.png:  %.dia
	dia -e $@ $<

%.png: %.pic
	pic2plot -T png $< > $@

%.ps: %.pic
	pic2plot -T ps $< > $@

%.eps: %.ps
	ps2eps $<

%.eps:  %.dia
	dia -e $@ $<

%.eps:  %.dot
	dot -Tps $< -o $@

%.pdf:  %.eps
	epstopdf $<

%.eps: %.png
	convert $< $@

%.pdf:          %.tex
# http://tex.stackexchange.com/questions/67859/errors-in-latexmk-with-use-of-auto-pst-pdf-and-hyperref
		latexmk -e "\$$hash_calc_ignore_pattern{'pdf'} = '^/(CreationDate|ModDate|ID) ';" -pdf -pdflatex="pdflatex --shell-escape  %O  %S" $<

clean:
		latexmk -c
		$(RM) -f *.bbl *.qsl *.sol \
		*.aux *.log *.bbl *.blg *.brf *.cb *.ind *.idx *.ilg  \
		*.inx *.ps *.dvi *.pdf *.toc *.out *.lot *.lof *.eps *.fls *.fdb_latexmk

