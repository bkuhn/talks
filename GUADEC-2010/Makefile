# Makefile for SFLC Presentation
#
#  There are two settings that the user should be concerned with:
#      PRESENTATION_BASE, and SFLC_REPOSITORY_PATH.  Details on those are below.
#
#  Once those variables are set properly, just typing "make" should get you
#  a PDF, Postscript, and HTML version of your paper.

# You can change the PRESENTATION_BASE below, or if you like, or set it as
# an environment variable before you type make.

ifndef PRESENTATION_BASE
PRESENTATION_BASE=gplv3
endif

DO_INCREMENTAL_POINTS = -i -s

PATH := $(PATH):/usr/share/tex4ht


TEXINPUTS := $(SFLC_WHITEPAPER_TEX_PATH):$(SFLC_TEX_PATH):$(TEXINPUTS)::
TEX4HTINPUTS := /etc/tex4ht:$(SFLC_WHITEPAPER_TEX_PATH):$(SFLC_TEX_PATH):$(TEX4HTINPUTS)::
T4HTINPUTS := /etc/tex4ht:$(SFLC_WHITEPAPER_TEX_PATH):$(SFLC_TEX_PATH):$(T4HTINPUTS)::

PANDOC=/usr/bin/pandoc
TEX4HT=tex4ht
T4HT=t4ht
PDFLATEX = pdflatex
LATEX = latex
BIBTEX = bibtex
FIG2DEV = fig2dev
DVIPS=dvips

PDF_FIGS = $(SFLC_LOGO_PDF)

all:	err $(PRESENTATION_BASE).pdf $(PRESENTATION_BASE).ps $(PRESENTATION_BASE).html
all:	$(PRESENTATION_BASE).html

.SUFFIXES: .fig .postscript .eps .pdf .pstex_t .pstex .ps .dvi .tex

.postscript.pdf:
	ps2pdf $< $@

.postscript.eps:
	ps2epsi $< $@

.dvi.ps:
	$(DVIPS) $< -o $@

.tex.dvi:
	$(LATEX) $<

.fig.pdf:
	$(FIG2DEV) -L pdf -p "portrait" -c $< > $@

.fig.pstex_t:
	$(FIG2DEV) -L pstex_t $< > $@

.fig.pstex:
	$(FIG2DEV) -L pstex $< > $@

$(PRESENTATION_BASE).pdf: $(PDF_FIGS) $(PRESENTATION_BASE).markdown $(SFLC_WHITEPAPER_CLASS_FILE)
	$(PANDOC) -S -s -f markdown -t latex $(PRESENTATION_BASE).markdown -o $(PRESENTATION_BASE).tex
	$(PDFLATEX)  $(PRESENTATION_BASE).tex
	$(PDFLATEX)  $(PRESENTATION_BASE).tex

$(PRESENTATION_BASE).html: $(PRESENTATION_BASE).markdown
	$(PANDOC) $(DO_INCREMENTAL_POINTS) -S -C ./ui/bkuhn/header.html -f markdown -t s5 $(PRESENTATION_BASE).markdown -o $(PRESENTATION_BASE).html

$(PRESENTATION_BASE).dvi: $(PRESENTATION_BASE).tex $(EPS_FIGS) $(SFLC_WHITEPAPER_CLASS_FILE)
	$(LATEX)  $(PRESENTATION_BASE).tex
	$(LATEX)  $(PRESENTATION_BASE).tex

clean:
	/bin/rm -f $(PRESENTATION_BASE).ps $(PRESENTATION_BASE).pdf $(PRESENTATION_BASE).log texput.log $(PRESENTATION_BASE).lg $(PRESENTATION_BASE).tmp $(PRESENTATION_BASE).xref *.4ct *.4tc *.aux *.dvi $(PRESENTATION_BASE)*.html *.idv *.lg *.tmp $(PRESENTATION_BASE).css $(PRESENTATION_BASE).log $(PRESENTATION_BASE).out $(PRESENTATION_BASE)-js.* $(PRESENTATION_BASE).tex

err: ; $(ERR)
