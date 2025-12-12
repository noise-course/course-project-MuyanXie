extract_comments:
	tshark -r data/traffic.pcapng -T fields -E header=y -e frame.number -e frame.comment \
    | cut -f1,2 \
    | tr '\t' ',' \
    > data/extracted.csv

compile_pdf:
	pandoc Research_Proposal.md -o Research_Proposal.pdf -V geometry:margin=1in

html:
	sphinx-build -b html . _build/html	