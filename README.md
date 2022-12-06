# Processes to analyze and understand structural variants

## Description

This repository contains a python program to help process and analyze structural variants that occur in species. It can be applied to any species as long as the input is of the correct format (working with vcf and fasta files). This repository also contains output of Blastn program runs (in the form of txt and xml files) and fasta files that contain the relevant variants (by frequency) for sub genus populations of a species. The results of the 
Blast program runs are named by the sub population that was both the query and subject of the run. For example, if the file is named results_African_Ancestry.xml then this file contains the output of a blast run aligning the sequences belonging to the African Ancestry population against each other. The species for which there is data include:
- human
- cow
- pig
- horse
- chicken

The filtered vcf files are filtered by SVTYPE='DEL'. If you wish to look at a different type of variant this can be changed by refiltering the original vcf files which are contained in each species folder by desired variant type using the command line arugments found in the "Full Workflow" section of the python notebook.

Finally, this repository contains a writeup of some of the findings of the project.

The python progarm is in the file called SV_generralized.ipynb 

## Links to helpful sites <br> 
Sequence Archive Run Browser
- https://trace.ncbi.nlm.nih.gov/Traces/?view=run_browser&display=metadata

1000 Genomes Database of Genome Samples/1000 Genomes Homepage
- https://www.internationalgenome.org/data
- https://www.internationalgenome.org/data-portal/sample

BLAST in python
- https://pypi.org/project/pyblastbio/
- https://www.tutorialspoint.com/biopython/biopython_overview_of_blast.htm
- https://hossainlab.github.io/PY4B/notebooks/07-DNA%20Sequence%20Statistics.html

Building a blast db locally
- https://www.ncbi.nlm.nih.gov/books/NBK569841/

Running BLASTn from command line
- https://www.ncbi.nlm.nih.gov/books/NBK569856/
- https://open.oregonstate.education/computationalbiology/chapter/command-line-blast/
- https://www.biostars.org/p/160350/

Making db and running blastn
- https://www.ncbi.nlm.nih.gov/books/NBK569856/
- https://www.metagenomics.wiki/tools/blast/blastn-output-format-6

Salmon paper on SVs
- https://www.nature.com/articles/s41467-020-18972-x

General how BLAST works and its output
- https://cs.calvin.edu/activities/blasted/other/BLAST.html
- https://resources.qiagenbioinformatics.com/manuals/clcgenomicsworkbench/650/Explanation_BLAST_output.html
- https://www.ncbi.nlm.nih.gov/books/NBK1734/
- https://guides.lib.berkeley.edu/ncbi/blast

