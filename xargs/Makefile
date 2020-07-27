.PHONEY:cp clean

SHELL = /bin/bash

cp:
	find . -name "*.txt" | xargs -p -I{} cp {} {}.bak

clean:
	rm *.bak
