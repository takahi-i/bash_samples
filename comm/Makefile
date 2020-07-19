.PHONEY: sort
.PHONEY: compare

sort:
	cat sample1.txt | sort > sample1.sorted
	cat sample2.txt | sort > sample2.sorted

compare: sort
	comm sample1.sorted sample2.sorted

clean:
	rm *.sorted
