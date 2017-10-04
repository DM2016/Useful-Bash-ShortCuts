# Useful-Bash-ShortCuts
ShortCuts For Processing RNAseq Data

#generate multiple fastq files from .sra


ls *.sra | xargs -I {} -P 5 -n 1 path/to/fastq/dump --split-3 {} 
