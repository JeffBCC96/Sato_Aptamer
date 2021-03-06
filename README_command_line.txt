Instruction of Aptamer Design


1. In order to run Aptamer design successfully, a suitable environment is required. Please install the following tools at first: 
		--- Vienna RNA
		--- SPARCS
		--- NUPACK   


2. Run the python script: 

	option 1: Run it with a fasta file/ gene bank file/ Gene ID
			  Command: python APD.py NM_001294338 
		    	      
	option 2: Run it with a name (you provided) and a sequence
			  Command: python APD.py name ACTGCACG...
			  
	Folder ¡°name¡± contains the following outputs: 
		- Final result of designed aptamers (final_result)
		- Blast result of the aptamers (info_species)
		- Failed aptamers with reasons (failed_aptamers)
		- Original input file (xx.fa/xx.gb)
		- Input sequence (yourSeq.fa)
		- Dinucleotide random sequences (name.fa)
		- Uniform random sequences (name_ran.fa)
		- Predicted segments (segmentsfile_name.txt)
		- Z-score plot for dinucleotide modle (name_zplot.png)
		- Z-score plot for uniform modle (name_zplotRan.png)



3. Run with options:
	If you want to use RNA alignment function to design aptamers unique to each of the similar RNAs, please follow the example here. 

	python APD.py RNA_seq1 RNA_seq2 Seqname_1 Seqname_2 -a

	Here RNA_seq1 means the first RNA sequence: AGTCGATCGTCTA¡­
	     RNA_seq2 means the second RNA sequence: AGTCGATCGGGTG¡­
             Seqname_1 and Seqname_2 are the names for sequence 1 and sequence 2 
	     which are optional. The default names are ¡®seq1¡¯, ¡®seq2¡¯ 


