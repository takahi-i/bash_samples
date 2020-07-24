.PHONEY: conv join select clean
SHELL = /bin/bash

conv:
	iconv -f EUCJP -t UTF8 nationals_en.txt  > nationals_en.utf8
	iconv -f EUCJP -t UTF8 nationals_ja.txt  > nationals_ja.utf8

select:
	cut -d "," -f 1,2 nationals_en.utf8 > nationals_en.cut
	cut -d "," -f 1,2 nationals_ja.utf8 > nationals_ja.cut

join:
	join -t "," nationals_en.cut nationals_ja.cut > ml_input_data.txt

clean:
	rm *.utf8
	rm *.cut
	rm ml_input_data.txt
