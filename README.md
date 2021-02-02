## SVision

SVision is a deep learning-based structural variants caller that takes aligned reads or contigs as input. 
Especially, SVision implements a targeted multi-objects recognition framework, detecting and characterizing both simple and
complex structural variants from three-channel similarity images.

Please check the wiki page for more details. 

===================================
## Install and run


#### Install SVision from source
Step1: Create a new environment with conda

Step2: Install required packages:
		conda install pysam
		conda install tensorflow
		conda install opencv-python
	

Step3: Install source code
		git ....
		cd SVision
		pip install .



===================================
Change Log:
2020.7.16
    Fix a bug when discern major and minor segments at src/analyze_reads.py line 20

2020.7.17 SVision v1.0.2
    Filter cluster with wrong cords

2020.7.20 SVision v1.0.3
    Add log file

2020.7.28 SVision v1.1.0
    Add shift operation

2020.8.10 SVision v1.1.1
    Modify SV and CSV's definition

2020.8.12 SVision v1.1.2
    Fix bug when meeting chrUn_JTFH01001938v1_decoy

2020.8.26 SVision v1.1.3
    add refine mode

2020.8.26 SVision v1.1.4
    report DNA repair mechanism

2020.9.17 SVision v1.1.5
    process_cigars() in collect_signatures.py affect the  breakpoints' precision of short (about 50bp) DEL and INS

2020.10.18 SVision v1.1.6
    Motify mechanism if conditions
    Add GT, DV, DF output

2020.11.16 SVision v1.2
    Fig Bug when dealing minimap2-align, which SA tag has wrong CIGAR
    Add Graph representation
    Add a prameter for detecting from contigs

2021.1.3 SVision v1.2.1
    fix bug: ins length in detailed bkps
# Non-use
# 2020.10.7 SVision v1.2.0
#    add mechanism as a parameter. and the mechanism includes TE, VNTR, MMBIR, NHEJ, NAHR et. al