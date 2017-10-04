# Useful-Bash-ShortCuts
ShortCuts For Processing RNAseq Data

#generate multiple fastq files from .sra


ls *.sra | xargs -I {} -P 5 -n 1 path/to/fastq/dump --split-3 {} 

#indexing multiple .sorted.bam files
ls *.sorted.bam | xargs -n1 -P5 /usr/local/samtools/1.3.1/bin/samtools index
