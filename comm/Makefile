.PHONEY: sort
.PHONEY: compare
SHELL = /bin/bash

sort:
	cat sample1.txt | sort > sample1.sorted
	cat sample2.txt | sort > sample2.sorted

compare: sort
	comm sample1.sorted sample2.sorted

compare_without_temp_file:
	comm <(sort sample1.txt) <(sort sample2.txt)

clean:
	rm *.sorted
