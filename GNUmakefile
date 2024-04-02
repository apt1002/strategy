# Build as HTML
# Uses GNU Make features, hence named "GNUmakefile"

# An HTML file for each markdown file, except that README.md→index.html
all: $(filter-out README.html,index.html $(patsubst %.md,%.html,$(wildcard *.md)))

index.html: README.md GNUmakefile
	markdown $< > $@ && \
	rpl 'href="(.*)\.md"' 'href="\2.html"' $@

%.html: %.md GNUmakefile
	markdown $< > $@ && \
	rpl 'href="(.*)\.md"' 'href="\2.html"' $@
