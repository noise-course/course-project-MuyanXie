extract_comments:
	tshark -r traffic.pcapng -T fields -E header=y -e frame.number -e frame.comment \
	| cut -f1,2 \
	| tr '\t' ',' \
	> extracted.csv
