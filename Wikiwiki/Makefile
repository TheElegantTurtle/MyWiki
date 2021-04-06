WIKI=$(shell find . -iname "*.wiki")

MARKDOWN=$(WIKI:.wiki=.md)

.PHONY = all clean
all: $(MARKDOWN)

%.md: %.wiki
	pandoc --from vimwiki --to markdown $< -o $@

clean:
	rm $(MARKDOWN)
