ROOT = $(shell git rev-parse --show-toplevel)
SOURCES = $(wildcard *.md)
TARGETS=$(SOURCES:.md=.html)

%.html: %.md $(ROOT)/extras/slides-defaults.yml slides-defaults.yml $(ROOT)/extras/screencast.revealjs
	mmdc -i $< -o $<-tmp.md
	pandoc $<-tmp.md -o $@ --defaults $(ROOT)/extras/slides-defaults.yml --defaults slides-defaults.yml
	rm $<-tmp.md

all: $(TARGETS)
