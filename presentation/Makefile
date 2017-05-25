# Directories
OUT_DIR=texout
IN_DIR=input/content

# The latex main document
TEX_MAIN=main

# PDF-file name
PDF_TITLE=compiler-backdoor

# Makefile specific.
.PHONY: main.pdf all clean

all: main.pdf

# Main latexmk rule.
main.pdf: $(TEX_MAIN).tex $(IN_DIR)/*
			latexmk -pdf -jobname=$(PDF_TITLE) \
				-outdir=$(OUT_DIR) \
				$(TEX_MAIN).tex

clean:
	rm -f $(OUT_DIR)/*

