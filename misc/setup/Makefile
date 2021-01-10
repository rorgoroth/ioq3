VERSION=4.1.1
RELEASE=git

all:
	VERSION=$(VERSION) RELEASE=$(RELEASE) ./doit

sign:
	for i in *.run; do \
		gpg -bao $$i.asc $$i; \
	done

clean:
	rm -rf *.run image defines.m4

.PHONY: all sign clean
