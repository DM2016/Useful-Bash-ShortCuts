# Useful-Bash-ShortCuts
ShortCuts For Processing RNAseq Data

#generate multiple fastq files from .sra
ls *.sra | xargs -I {} -P 5 -n 1 /panfs/pan1.be-md.ncbi.nlm.nih.gov/product_manager_research_projects/Diego/allelic_imbalance_project/sratoolkit.2.8.2-1-centos_linux64/bin/fastq-dump.2.8.2 --split-3 {}
