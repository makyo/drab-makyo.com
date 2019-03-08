.PHONY: all
all: signed-will.md.asc will.pdf

signed-will.md.asc: will.md
	gpg -o signed-will.md.asc -sa will.md

will.pdf: will.md
	pandoc --wrap=none -o will-contents.tex will.md
	perl -pi.bak -e 's/section\{/section*{/' will-contents.tex
	xelatex will.tex
	xelatex will.tex
