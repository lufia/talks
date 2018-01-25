TARG=\
	proc.png\
	par.png\
	on.png\
	off.png\

PLANTUML=plantuml

all: $(TARG)

%.png: %.spuml
	$(PLANTUML) $<

%.spuml: %.puml
	iconv -f UTF-8 -t SJIS $< >$@

clean:
	rm -f $(TARG) *.spuml
