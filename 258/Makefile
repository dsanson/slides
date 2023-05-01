ROOT = $(shell git rev-parse --show-toplevel)
SOURCES = $(wildcard *.md)
TARGETS=$(SOURCES:.md=.html)

%.html: %.md $(ROOT)/extras/slides-defaults.yml $(ROOT)/extras/screencast.revealjs
	pandoc $< -o $@ --defaults $(ROOT)/extras/slides-defaults.yml

all: $(TARGETS)
