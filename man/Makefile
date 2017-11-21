
man_pages := $(patsubst %.1.md,man1/%.1.gz,$(wildcard *.1.md))

all: $(man_pages)

clean:
	rm -f $(man_pages)

# Compile a man page from Markdown using pandoc.
# Don't use 'smart' extension, as it turns double dashes into an en-dash,
# which isn't good for command line option docs.
man1/%.1: %.1.md man1
	pandoc $< -s -f markdown-smart -t man -o $@

# Zip up the compiled man page.
%.1.gz: %.1
	gzip -f9 $<

man1:
	mkdir -p man1
