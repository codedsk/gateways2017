PROJECT = gateways2017_webapps

${PROJECT}.pdf: ${PROJECT}.tex
	texi2pdf ${PROJECT}.tex

all: pdf
pdf: ${PROJECT}.pdf
	cp ${PROJECT}.pdf gateways2017_hz_web_apps_`date "+%Y%m%d"`.pdf

#spellcheck:
#	for i in *.tex; do aspell --mode=tex -c ${i}; done

clean:
	rm -rf *.aux *.log *-converted-to.pdf \
           ${PROJECT}.4ct \
           ${PROJECT}.4tc \
           ${PROJECT}.aux \
           ${PROJECT}.css \
           ${PROJECT}.dvi \
           ${PROJECT}.idv \
           ${PROJECT}.lg \
           ${PROJECT}.log \
           ${PROJECT}.lov \
           ${PROJECT}.lot \
           ${PROJECT}.lof \
           ${PROJECT}.tmp \
           ${PROJECT}.toc \
           ${PROJECT}.xref \
           bibliography.bbl \
           bibliography.blg \
           ${PROJECT}-blx.bib \
           ${PROJECT}.bbl \
           ${PROJECT}.blg \
           ${PROJECT}.run.xml \

distclean: clean
	rm -rf ${PROJECT}.pdf ${PROJECT}.html ${PROJECT}.txt
