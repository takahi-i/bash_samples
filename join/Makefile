.PHONEY: join join_flush_inperfect
SHELL = /bin/bash

join:
	join -t "," nationals_en.txt nationals_ja.txt

join_flush_inperfect:
	join -a 2 -t "," -e "----" -o 2.2,1.2 nationals_en.txt nationals_ja.txt

clean:
	rm *.sorted
