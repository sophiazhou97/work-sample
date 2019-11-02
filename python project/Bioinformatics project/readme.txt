Bioinformatics genome project

This project aims to find the donor genome by aligning the reads from the donor genome to the reference genome.

basic_hasher.py: 
Align all the reads to the most likely positions in the reference genome. It takes in a reference genome, a set of reads and an output file and outputs the reads aligned to the reference genome into the output file.

complex_pileup.py: 
Takes in aligned reads and an output file and outputs the SNPs and indels called based on the aligned reads. It uses an edit distance approach to call variants.  
You can test the code by 
python3 basic_hasher.py -g practice_E_1/ref_practice_E_1_chr_1.txt  -r practice_E_1/reads_practice_E_1_chr_1.txt -o test_hasher.txt
python3 complex_pileup.py -a test_hasher.txt -o test_pileup.txt -t practice_E_1_chr_1
