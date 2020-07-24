.PHONEY:cp
.PHONEY:clean
SHELL = /bin/bash

cp:
	find . -name "*.txt" | xargs -I{} cp {} {}.bak

clean:
	rm *.sorted
